---
tip: translate by baidu@2024-07-18 13:05:07
docsearch:language: en
lang: en
title: "7. The Process: A virtual Computer --- Introduction to Operating Systems"
viewport:
  - width=device-width, initial-scale=1.0
  - width=device-width, initial-scale=1
  - width=device-width, initial-scale=1
---

# The Process: A virtual Computer

## Contents

# [7. ] {.section-number}The Process: A virtual Computer[\#](#the-process-a-virtual-computer "Link to this heading") {.headerlink}

A process is a virtual computer than encapsulates CPU state for execution context, a virtual memory abstraction of massive contiguous memory that starts at address `0x0`{.docutils .literal .notranslate}, and state needed to interact with other processes and read/write state from file system.

> 进程是一种虚拟计算机，它封装了执行上下文的 CPU 状态，是从地址“0x0”{.docutils.literal.notranslate}开始的大量连续内存的虚拟内存抽象，以及与其他进程交互所需的状态和从文件系统读/写状态。

::: {#the-interface .section}

## [7.1. ] {.section-number}The interface[\#](#the-interface "Link to this heading") {.headerlink}

The key system calls in traditional Unix related to processes are:

- `pid = fork(void)`{.docutils .literal .notranslate}: Create a child process that is a duplicate of the parent; return 0 in child, and `PID`{.docutils .literal .notranslate} of child in parent.

> -`pid=fork（void）`{.docutils.literal.notranslate}：创建一个与父进程重复的子进程；在子节点中返回 0，在父节点中返回子节点的 PID{.docutils.literal.notranslate}。

- `exit(status)`{.docutils .literal .notranslate}: Terminate the calling process and record the status passed in for others.

> -`exit（status）`{.docutils.literal.notranslate}：终止调用进程并记录传递给其他进程的状态。

- `pid = waitpid(cpid, *status...)`{.docutils .literal .notranslate}: Wait for specified child process `cpid`{.docutils .literal .notranslate} to complete (or change state), fill `*status`{.docutils .literal .notranslate} with the status passed on child's exit, and garbage collect any kernel resources; return the `PID`{.docutils .literal .notranslate} of the child process that exited (or changed state).

> -`pid=waitpid（cpid，*status…）`{.docutils.literal.notranslate}:等待指定的子进程`cpid`{.docuutils.literal.notranslate}完成（或更改状态），在子进程退出时用传递的状态填充`*state`{.dokutils.literal.notranslate}，并垃圾回收任何内核资源；返回退出（或更改状态）的子进程的“PID”{.docutils.literal.notranslate}。

- `err = execve(program, arguments, environment)`{.docutils .literal .notranslate}: executing the file `program`{.docutils .literal .notranslate} with specified arguments and environment information

> -`err=execve（程序、参数、环境）`｛.docutils.literal.notranslate｝：使用指定的参数和环境信息执行文件`program`｛.dokutils.literal.notranslate}

The `fork`{.docutils .literal .notranslate} system call duplicates the calling process (referred to as the _parent_) into a new _child_ process, where the only difference that enables the parent and child to distinguish themself is the return value. You can think of this logically as creating a copy of all the process memory, copying the CPU state, and copying the file descriptor table (while incrementing reference counts on all the files pointed to by the file descriptor table).

> `fork`{.docutils.literal.notranslate}系统调用将调用进程（称为*parent*）复制到一个新的*child*进程中，其中使父进程和子进程能够区分自己的唯一区别是返回值。从逻辑上讲，您可以将其视为创建所有进程内存的副本、复制 CPU 状态和复制文件描述符表（同时递增文件描述符表格指向的所有文件的引用计数）。

A process has a large amount of state associated with it. Linux implements `fork`{.docutils .literal .notranslate} in a library on top of the lower level `clone`{.docutils .literal .notranslate} call that lets the calling program control what part of the state is copied to the child. As we will see, this enables the same system call to be used to both create processes, and create threads within those processes.

> 一个进程有大量与之相关的状态。Linux 在较低级别的 clone 调用之上的库中实现了 fork{.docutils.literal.notranslate}，该调用允许调用程序控制将状态的哪一部分复制到子进程。正如我们将看到的，这使得相同的系统调用既可以用于创建进程，也可以用于在这些进程中创建线程。

Fork is usually quickly followed by a call to `exec`{.docutils .literal .notranslate} to execute a new program. One of the often claimed _elegant_ design decisions of unix is that after a fork, the child has fine grained control to change file descriptor state before calling `exec`{.docutils .literal .notranslate}; that is, the same functionality that is used for normal access to files is used by the shell between fork and exec to set up he child.

> Fork 之后通常会快速调用`exec`{.docutils.literal.notranslate}来执行新程序。unix 经常声称的*elegant*设计决策之一是，在 fork 之后，子级具有细粒度的控制权，可以在调用`exec`{.docutils.literal.notranslate}之前更改文件描述符状态；也就是说，fork 和 exec 之间的 shell 使用与正常访问文件相同的功能来设置子级。

Some of the authors have argued that fork was a clever hack for machines and programs of the 1970s that has long outlived its usefulness and is now a liability [\[[BAKR19](../misc/bib.html#id3 "Andrew Baumann, Jonathan Appavoo, Orran Krieger, and Timothy Roscoe. A fork() in the road. In Proceedings of the Workshop on Hot Topics in Operating Systems, HotOS '19, 14–22. New York, NY, USA, 2019. Association for Computing Machinery. URL: https://doi.org/10.1145/3317550.3321435, doi:10.1145/3317550.3321435."){.reference .internal}\]]{#id1}. Many operating systems provide powerful primitives to control the launching of new programs without an intervening `fork`{.docutils .literal .notranslate}, and fork imposes design constraints and overheads that these alternatives don't have. Even on Linux for many use cases, `posix_spawn`{.docutils .literal .notranslate} combines the functionality of `fork`{.docutils .literal .notranslate} and `exec`{.docutils .literal .notranslate}. However, `posix_spawn`{.docutils .literal .notranslate} is on Linux implemented on top of clone, so it doesn't actually alleviate the author's concerns.

> 一些作者认为，fork 是 20 世纪 70 年代对机器和程序的一种聪明的黑客攻击，早已不再有用，现在是一种负担[\[[BAKR19]（../misc/bib.html#id3”Andrew Baumann，Jonathan Appavoo，Orran Krieger 和 Timothy Roscoe.a fork（）在路上。在《操作系统热点研讨会论文集》中，HotOS'19，14-22。2019 年，美国纽约州纽约市。国际计算机学会网址：https://doi.org/10.1145/3317550.3321435，doi:10.1145/3317550.3321435.“）{.reference.internal}\]]{#id1}。许多操作系统提供了强大的原语来控制新程序的启动，而不需要中间的`fork`{.docutils.literal.notranslate}，fork施加了这些替代方案所没有的设计约束和开销。即使在Linux上的许多用例中，`posix_spawn`{.dokutils.literal.notranslate}也结合了`fork`{.docuutils.literal.notranslate}`和`exec`{.docutils.literary.notranslate}的功能。然而，`posix_spawn`{.dokuutils.notranslate}.s.literal.notranslate}是在clone之上实现的Linux上，因此它实际上并没有减轻作者的担忧。

Heresy "fork is a clever hack that has outlived its usefulness":

The paper "A fork in the road"[\[[BAKR19](../misc/bib.html#id3 "Andrew Baumann, Jonathan Appavoo, Orran Krieger, and Timothy Roscoe. A fork() in the road. In Proceedings of the Workshop on Hot Topics in Operating Systems, HotOS '19, 14–22. New York, NY, USA, 2019. Association for Computing Machinery. URL: https://doi.org/10.1145/3317550.3321435, doi:10.1145/3317550.3321435."){.reference .internal}\]]{#id2}, resulted in thousands and thousands of heated posts on a range of public forums. You can see some of the debate between Orran Krieger and a well known Linux architect Uli Drepper [here](https://www.bu.edu/rhcollab/2019/04/11/a-fork-in-the-road/){.reference .external}, along with links to the public forums. While those of us that wrote the paper still assert `fork`{.docutils .literal .notranslate} is a poor idea, we will use this opportunity to assert that we much prefer Linux to windows and we are in fact not "Microsoft stooges".

> 论文“岔路口”[\[[BAKR19]（../misc/bib.html#id3”Andrew Baumann、Jonathan Appavoo、Orran Krieger 和 Timothy Roscoe.岔路口（）。操作系统热点研讨会论文集，HotOS'19，14-22。2019 年，美国纽约州纽约市。国际计算机学会网址：https://doi.org/10.1145/3317550.3321435，doi:10.1145/3317550.3321435.“）{.reference.internal}\]]{#id2}，在一系列公共论坛上引发了成千上万的激烈帖子。你可以在这里看到Orran Krieger 和著名的 Linux 架构师 Uli Drepper 之间的一些争论(https://www.bu.edu/rhcollab/2019/04/11/a-fork-in-the-road/){.reference.external}，以及公共论坛的链接。虽然我们这些写这篇论文的人仍然认为“fork”{.docutils.literal.notranslate}是一个糟糕的主意，但我们将借此机会断言，我们更喜欢Linux而不是windows，事实上我们不是“微软的傀儡”。

There are actually many more interfaces supported by systems like Linux related to process management. You can, for example, send a signal (e.g., to stop or kill) a process using:

> 实际上，Linux 等系统支持的与进程管理相关的接口要多得多。例如，您可以使用以下命令发送信号（例如停止或终止）进程：

- `kill(pid_t pid, int sig)`{.docutils .literal .notranslate}: Send a signal to a process or group of processes

> -`kill（pid_t pid，int sig）`{.docutils.literal.notranslate}：向一个进程或一组进程发送信号

Some of these interfaces are actual system calls and are in section 2 of the man pages, others are implemented in a library; you can, for example type `man -k exec`{.docutils .literal .notranslate} to find out which man pages relate to exec. If you type `man 3 exec`{.docutils .literal .notranslate} you will find a whole series of higher level functions built on top of `execve`{.docutils .literal .notranslate}.

> 其中一些接口是实际的系统调用，位于手册页的第 2 节中，其他接口在库中实现；例如，您可以键入`man-kexec`{.docutils.literal.notranslate}来找出哪些手册页与 exec 相关。如果你键入“man 3 exec”{.docutils.literal.notranslate}，你会发现一系列构建在“execve”{.dokutils.literal.notranslate}之上的高级函数。
> :::

::: {#process-versus-program .section}

## [7.2. ] {.section-number}Process versus Program[\#](#process-versus-program "Link to this heading") {.headerlink}

It is important to understand the difference between a program and a process. A program is a executable file, generated by a compiler and linker, that can be executed using `exec`{.docutils .literal .notranslate}. The `exec`{.docutils .literal .notranslate} system call then populates the memory region of the process with information pulled out of that program and there can be many processes, by many users, running the same program.

> 了解程序和过程之间的区别很重要。程序是由编译器和链接器生成的可执行文件，可以使用`exec`{.docutils.literal.notranslate}执行。然后，`exec`{.docutils.literal.notranslate}系统调用用从该程序中提取的信息填充进程的内存区域，并且可以有许多用户运行同一程序的许多进程。

To understand how the portions of the executable file are used by the process, consider the following trivial program that runs an infinite loop so we can examine it while it is running.

> 要了解进程如何使用可执行文件的各个部分，请考虑以下运行无限循环的简单程序，以便我们可以在它运行时对其进行检查。

::: {#while-one-listing .literal-block-wrapper .docutils .container}
::: code-block-caption

[Listing 7.1 ]{.caption-number}[wo.c - A simple program that loops forever]{.caption-text}[\#](#while-one-listing "Link to this code"){.headerlink}

> [清单 7.1]{.caption number}[wo.c-一个永远循环的简单程序]{.ception text}[\#]（#其中一个列出了“链接到此代码”）{.headerlink}
> :::

```c
int main() {
 while(1);
}
```

If we compile this program, run it, I can use the synthetic file system "/proc/PID/maps" to ask Linux about what is mapped in different parts of the application address space. Node, in bash the variable `$!`{.docutils .literal .notranslate} is the pid of the last started process.

> 如果我们编译这个程序，运行它，我可以使用合成文件系统“/proc/PID/maps”向 Linux 询问在应用程序地址空间的不同部分映射了什么。Node，在 bash 中的变量`$`{.docutils.literal.notranslate}是最后一个启动进程的 pid。

::: {.admonition .note}
Note

Fields when looking at /proc/PID/maps:

- address: This is the starting and ending address of the region in the process's address space

- permissions - This describes how pages in the region can be accessed. There are four different permissions: read, write, execute, and shared. If a region is not shared, it is private, so a p will appear instead of an s.

> -权限-描述如何访问该区域中的页面。有四种不同的权限：读取、写入、执行和共享。如果一个区域不共享，则它是私有的，因此将显示 p 而不是 s。

- offset - If the region was mapped from a file (using mmap), this is the offset in the file where the mapping begins. If the memory was not mapped from a file, it's just 0.

> -offset-如果区域是从文件映射的（使用 mmap），则这是映射开始的文件中的偏移量。如果内存不是从文件映射的，则只有 0。

- device - If the region was mapped from a file, this is the major and minor device number (in hex) where the file lives.

> -设备-如果该区域是从文件映射的，则这是文件所在的主要和次要设备号（十六进制）。

- inode - If the region was mapped from a file, this is the file number.

- pathname - If the region was mapped from a file, this is the name of the file. Otherwise, for special regions like the heap, stack... this field identifies the use.

> -pathname-如果区域是从文件映射的，则这是文件的名称。否则，对于堆、堆栈等特殊区域。。。此字段标识用途。
> :::

We can see that the first five regions of the process come directly from the file. We can use the `objdump`{.docutils .literal .notranslate} utility to print the different sections of the executable file, as shown below, where the second column `Name`{.docutils .literal .notranslate} describes that part of the file, and the fourth column `VMA`{.docutils .literal .notranslate} is the virtual memory address that should be loaded from the program. If you scroll through that information, you can see that the executable parts of the program (`.init`{.docutils .literal .notranslate}, `.plt `{.docutils .literal .notranslate}and `.text`{.docutils .literal .notranslate}) is loaded into the memory with executable permission. The `.rodata`{.docutils .literal .notranslate} is mapped into memory right after that, etc... All these regions have the **p**, or private, flag set in the permissions on the map, meaning that the operating system is creating a copy of the information from the file, so many processes can run the same program, and any writes they make to the corresponding memory will not be visible to other processes executing the same program.

> 我们可以看到，流程的前五个区域直接来自文件。我们可以使用`objdump`{.docutils.literal.notranslate}实用程序打印可执行文件的不同部分，如下所示，其中第二列`Name`{.dokutils.literal.notranslate}描述了文件的该部分，第四列`VMA`{.docutils.literary.notranslate}是应从程序加载的虚拟内存地址。如果你滚动浏览这些信息，你可以看到程序的可执行部分（“.init”｛.docutils.literal.notranslate｝、“.plt”｛.dokutils.literal.notranslate｝和“.text”｛.docutils.literary.notranslate｝）是以可执行权限加载到内存中的。紧随其后，`.rodata`{.docutils.literal.notranslate}被映射到内存中，以此类推。所有这些区域都在映射的权限中设置了**p**或 private 标志，这意味着操作系统正在从文件中创建信息的副本，因此许多进程可以运行同一程序，并且它们对相应内存的任何写入对于执行同一程序的其他进程都是不可见的。
