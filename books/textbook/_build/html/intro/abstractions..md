---
docsearch:language: en
lang: en
title: 4. Operating System Abstractions --- Introduction to Operating Systems
viewport:
- width=device-width, initial-scale=1.0
- width=device-width, initial-scale=1
- width=device-width, initial-scale=1
---

::: {#pst-skip-link .skip-link .d-print-none}
[Skip to main content](#main-content)
:::

::: {#pst-scroll-pixel-helper}
:::

Back to top

::: search-button__wrapper
::: search-button__overlay
:::

::: search-button__search-container
[[Ctrl]{.kbd .kbd-shortcut__modifier}+[K]{.kbd}]{.search-button__kbd-shortcut}
:::
:::

::: {.pst-async-banner-revealer .d-none}
:::

::: {.bd-header .navbar .navbar-expand-lg .bd-navbar .d-print-none}
:::

::: bd-container
::: {.bd-container__inner .bd-page-width}
::: {.bd-sidebar-primary .bd-sidebar}
::: {.sidebar-header-items .sidebar-primary__section}
:::

::: {.sidebar-primary-items__start .sidebar-primary__section}
::: sidebar-primary-item
[![Introduction to Operating Systems - Home](../_static/logo.png){.logo__image .only-light}](pref.html){.navbar-brand .logo}
:::

::: sidebar-primary-item
:::

::: sidebar-primary-item
::: {.bd-toc-item .navbar-nav .active}
-   [Preface](pref.html){.reference .internal}

[Getting started]{.caption-text}

-   [1. Introduction](intro.html){.reference .internal}
-   [2. Purpose of operating systems](purpose.html){.reference .internal}
-   [3. Operating System Structure & Unix/Linux](structure.html){.reference .internal}
-   [4. Operating System Abstractions](#){.current .reference .internal}
-   [5. What you should know](tools.html){.reference .internal}
    []{.toctree-toggle role="presentation"}
    -   [5.1. The C Programming Language](tools-c.html){.reference .internal}
    -   [5.2. Shell](tools-shell.html){.reference .internal}
    -   [5.3. Editors](tools-editors.html){.reference .internal}
    -   [5.4. Make](tools-make.html){.reference .internal}
    -   [5.5. Testing](tools-testing.html){.reference .internal}
    -   [5.6. Git Basics](tools-git.html){.reference .internal}
    -   [5.7. GDB](tools-gdb.html){.reference .internal}

[Virtual Processor]{.caption-text}

-   [6. Introduction](../scheduling/intro.html){.reference .internal}
-   [7. The Process: A virtual Computer](../scheduling/process.html){.reference .internal}
-   [8. Virtualizing the CPU](../scheduling/virtual.html){.reference .internal}
-   [9. The Thread: A Virtual CPU](../scheduling/threads.html){.reference .internal}
-   [10. Scheduling](../scheduling/scheduling.html){.reference .internal}
    []{.toctree-toggle role="presentation"}
    -   [10.1. Scheduling Goals](../scheduling/sch-goals.html){.reference .internal}
    -   [10.2. Simple Examples of Scheduling Policies](../scheduling/sch-simple.html){.reference .internal}
    -   [10.3. Scheduling with Priorities](../scheduling/sch-prio.html){.reference .internal}
    -   [10.4. Scheduling in the real world](../scheduling/sch-real.html){.reference .internal}
-   [11. Review Questions](../scheduling/review.html){.reference .internal}

[Virtual Memory]{.caption-text}

-   [12. Introduction](../mm/intro.html){.reference .internal}
-   [13. Memory management before paged virtual memory](../mm/phys-and-seg.html){.reference .internal}
-   [14. Paged Virtual memory](../mm/pagvm.html){.reference .internal}
    []{.toctree-toggle role="presentation"}
    -   [14.1. Abstracting a useful interface for memory management.](../mm/vmabs.html){.reference .internal}
    -   [14.2. Paging](../mm/virt-paging.html){.reference .internal}
    -   [14.3. Page Tables](../mm/page-tables.html){.reference .internal}
    -   [14.4. Memory reclaiming algorithms.](../mm/reclamation.html){.reference .internal}
    -   [14.5. Page Sizes](../mm/page-size.html){.reference .internal}
    -   [14.6. Memory Management Page Faults](../mm/pagefaults.html){.reference .internal}
-   [15. Buffer Cache](../mm/buffer-cache.html){.reference .internal}
-   [16. Memory management in the real world](../mm/realworld.html){.reference .internal}
-   [17. Conclusion](../mm/concl.html){.reference .internal}
-   [18. Review](../mm/review.html){.reference .internal}

[File Systems]{.caption-text}

-   [19. Introduction](../fs/intro.html){.reference .internal}
-   [20. File System Abstraction](../fs/interface.html){.reference .internal}
-   [21. A bit about Disks](../fs/diskhw.html){.reference .internal}
-   [22. Implementation](../fs/impl.html){.reference .internal}
    []{.toctree-toggle role="presentation"}
    -   [22.1. File System Layout](../fs/disklayout.html){.reference .internal}
    -   [22.2. Disk Layout:Tracking Used Space](../fs/dl_track_used.html){.reference .internal}
    -   [22.3. Disk Layout:Tracking Free Space](../fs/dl_track_free.html){.reference .internal}
    -   [22.4. Disk Layout:Implementing Name Space](../fs/dl_name.html){.reference .internal}
    -   [22.5. Disk Layout:Dealing with Failures](../fs/dl_failures.html){.reference .internal}
    -   [22.6. Disk Layout:Examples of Real World File Systems](../fs/dl_ex_exx.html){.reference .internal}
    -   [22.7. Kernel implementation](../fs/kernelimp.html){.reference .internal}
-   [23. Review](../fs/review.html){.reference .internal}

[Concurrency]{.caption-text}

-   [24. Introduction](../sync/sync.html){.reference .internal}
-   [25. Basic Synchronization](../sync/basic.html){.reference .internal}
    []{.toctree-toggle role="presentation"}
    -   [25.1. Cooperating Processes and Inter-process Communication](../sync/sharing.html){.reference .internal}
    -   [25.2. The Critical Section Problem](../sync/criticalsection.html){.reference .internal}
    -   [25.3. Implementing Locks](../sync/locks.html){.reference .internal}
    -   [25.4. Ordering Thread Events](../sync/ordering.html){.reference .internal}
-   [26. Common Concurrency Bugs](../sync/concurrency_bugs.html){.reference .internal}
-   [27. Advanced Synchronization](../sync/advanced.html){.reference .internal}
    []{.toctree-toggle role="presentation"}
    -   [27.1. Read-Dominated Workloads](../sync/readmostly.html){.reference .internal}
    -   [27.2. Challenges of Modern Hardware](../sync/hardware_challenges.html){.reference .internal}
    -   [27.3. Locking in the Linux Kernel](../sync/linux_locking.html){.reference .internal}
-   [28. Review](../sync/review.html){.reference .internal}

[Other Topics]{.caption-text}

-   [29. Input and Output](../devices/devices.html){.reference .internal}
-   [30. More on Disks](../devices/disk2.html){.reference .internal}
-   [31. Virtualization](../virt/virt.html){.reference .internal}
-   [32. Security](../sec/sec.html){.reference .internal}

[Appendices]{.caption-text}

-   [33. How to read this book](../misc/howto.html){.reference .internal}
-   [34. Contributing](../contributing/intro.html){.reference .internal}
    []{.toctree-toggle role="presentation"}
    -   [34.1. Examples](../contributing/examples.html){.reference .internal}
    -   [34.2. Contributors](../contributing/credit.html){.reference .internal}
    -   [34.3. Contributing](../contributing/Contributing.html){.reference .internal}
    -   [34.6. Resources to look at](../contributing/resources.html){.reference .internal}
    -   [34.7. Out of date](../contributing/fix.html){.reference .internal}
-   [35. Bibliography](../misc/bib.html){.reference .internal}
:::
:::
:::

::: {.sidebar-primary-items__end .sidebar-primary__section}
:::

::: {#rtd-footer-container}
:::
:::

::: {#main-content .bd-main role="main"}
::: sbt-scroll-pixel-helper
:::

::: bd-content
::: bd-article-container
::: {.bd-header-article .d-print-none}
::: {.header-article-items .header-article__inner}
::: header-article-items__start
::: header-article-item
[]{.fa-solid .fa-bars}
:::
:::

::: header-article-items__end
::: header-article-item
::: article-header-buttons
::: {.dropdown .dropdown-launch-buttons}

-   [[ ![JupyterHub logo](../_static/images/logo_jupyterhub.svg) ]{.btn__icon-container} [JupyterHub]{.btn__text-container}](https://jupyterhub-opf-jupyterhub.apps.smaug.na.operate-first.cloud/hub/user-redirect/git-pull?repo=https%3A//github.com/OpenOSOrg/openos&urlpath=lab/tree/openos/content/intro/abstractions.ipynb&branch=main "Launch on JupyterHub"){.btn .btn-sm .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
:::

::: {.dropdown .dropdown-source-buttons}

-   [[ ]{.btn__icon-container} [Repository]{.btn__text-container}](https://github.com/OpenOSOrg/openos "Source repository"){.btn .btn-sm .btn-source-repository-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
-   [[ ]{.btn__icon-container} [Suggest edit]{.btn__text-container}](https://github.com/OpenOSOrg/openos/edit/main/content/intro/abstractions.ipynb "Suggest edit"){.btn .btn-sm .btn-source-edit-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
-   [[ ]{.btn__icon-container} [Open issue]{.btn__text-container}](https://github.com/OpenOSOrg/openos/issues/new?title=Issue%20on%20page%20%2Fintro/abstractions.html&body=Your%20issue%20content%20here. "Open an issue"){.btn .btn-sm .btn-source-issues-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
:::

::: {.dropdown .dropdown-download-buttons}

-   [[ ]{.btn__icon-container} [.ipynb]{.btn__text-container}](../_sources/intro/abstractions.ipynb "Download source file"){.btn .btn-sm .btn-download-source-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
-   [ ]{.btn__icon-container} [.pdf]{.btn__text-container}
:::

[ ]{.btn__icon-container}

[]{.fa-solid .fa-list}
:::
:::
:::
:::
:::

::: {#jb-print-docs-body .onlyprint}
# Operating System Abstractions

::: {#print-main-content}
::: {#jb-print-toc}
<div>

## Contents

</div>

-   [4.1. Everything is a file](#everything-is-a-file){.reference .internal .nav-link}
-   [4.2. Process management](#process-management){.reference .internal .nav-link}
    -   [4.2.1. State](#state){.reference .internal .nav-link}
    -   [4.2.2. System calls](#system-calls){.reference .internal .nav-link}
    -   [4.2.3. Examples](#examples){.reference .internal .nav-link}
    -   [4.2.4. Summary](#summary){.reference .internal .nav-link}
-   [4.3. File system](#file-system){.reference .internal .nav-link}
-   [4.4. Changing stdin and stdout](#changing-stdin-and-stdout){.reference .internal .nav-link}
-   [4.5. Pipes](#pipes){.reference .internal .nav-link}
-   [4.6. Signals protecting against dreaded zombies](#signals-protecting-against-dreaded-zombies){.reference .internal .nav-link}
-   [4.7. Conclusion](#conclusion){.reference .internal .nav-link}
:::
:::
:::

::: {#searchbox}
:::

::: {.cell .tag_remove-input .docutils .container}
:::

::: {#operating-system-abstractions .section .tex2jax_ignore .mathjax_ignore}
[]{#cont-gs-abstractions}

# [4. ]{.section-number}Operating System Abstractions[\#](#operating-system-abstractions "Link to this heading"){.headerlink}

UNIX has instilled in generations of engineers a basic aesthetic for how to design and structure complicated collections of software. In particular one learns that the designers of UNIX tried to structure the system around a small core set of ideas, "abstractions", that once understood allows a programmer to understand the rest of the system and how to get things done.

We first describe the fundamental abstraction of [[files]{.std .std-ref}](#cont-gs-abstractions-file){.reference .internal}, which is central to Unix's ability to compose programs together, and how this enables powerful functionality to be implemented in a shell. We then, using a shell as an example, briefly discuss key abstractions and the interfaces a shell uses to control [[processes]{.std .std-ref}](#cont-gs-abstractions-process){.reference .internal}, enable processes to [[communicate]{.std .std-ref}](#cont-gs-abstractions-pipes){.reference .internal}, operate on [[files in a file system]{.std .std-ref}](#cont-gs-abstractions-fs){.reference .internal} and find out what [[happened]{.std .std-ref}](#cont-gs-abstractions-signals){.reference .internal} to processes it started.

::: {#everything-is-a-file .section}
[]{#cont-gs-abstractions-file}

## [4.1. ]{.section-number}Everything is a file[\#](#everything-is-a-file "Link to this heading"){.headerlink}

A core idea of Unix is that everything is a file, where a file is a stream of bytes. As shown in [[Fig. 4.1]{.std .std-numref}](#file-desc){.reference .internal}, the kernel maintains for each process a *file descriptor table*, where a file descriptor is an index into that table that can be used to read or write to a particular file. The system calls that work on all files are:

-   `n = write(desc, buffer, len)`{.docutils .literal .notranslate}: Write `len`{.docutils .literal .notranslate} bytes (or fewer if no more space is available) from `buffer`{.docutils .literal .notranslate} into a stream identified by `desc`{.docutils .literal .notranslate} and return the actual number of bytes written, `n`{.docutils .literal .notranslate}.

-   `n = read(desc, buffer, max)`{.docutils .literal .notranslate}: Read `max`{.docutils .literal .notranslate} bytes (or fewer if no more data is available) from stream identified by `desc`{.docutils .literal .notranslate} into `buffer`{.docutils .literal .notranslate} and return the actual number of bytes read, `n`{.docutils .literal .notranslate}.

To understand how to use these operations, you really need to read the manual. In Linux you can find out about everything using the **man** program. For example, `man 2 write`{.docutils .literal .notranslate} tells you everything about the `write`{.docutils .literal .notranslate} system call:

::: {.margin .admonition .note}
Note

In this case, the *2* refers to the section of the manual for system calls. To find out about the different sections, you, of course, read the manual about the man command.
:::

::: {.cell .tag_output_scroll .tag_remove-input .docutils .container}
::: {.cell_output .docutils .container}
:::
:::

To make files in the file system look like a stream, on each read or write operation, the kernel increases a (per open file) `offset`{.docutils .literal .notranslate} by the amount of data read or written. It turns out that this naturally matches many applications that read or write files in their entirety.

Entries are added to the file descriptor table by operations that open or create a regular file, or create a special file like a network connection or a tty. There are three special file descriptors shown in [[Table 4.1]{.std .std-numref}](#fd-table){.reference .internal}, that programs (and libraries) should use for input, output and errors.

![[Fig. 4.1 ]{.caption-number}[The kernel maintains for each process an array of file descriptors, where a process can read or write to any kind of I/O object that is open in its table.]{.caption-text}[\#](#file-desc "Link to this image"){.headerlink}](../_images/osstructure-fd.drawio.png){style="width: 60%;"}

::: pst-scrollable-table-container
+-------+-----------+------------------------------------------------------+
| Value | Name      | Purpose                                              |
+=======+===========+======================================================+
| 0     | stdin     | standard input; process should read data from here   |
+-------+-----------+------------------------------------------------------+
| 1     | stdout    | standard output; process will write its output here  |
+-------+-----------+------------------------------------------------------+
| 2     | stderr    | standard error; process should write out errors here |
+-------+-----------+------------------------------------------------------+

: [Table 4.1 ]{.caption-number}[Standard well known file descriptors.]{.caption-text}[\#](#fd-table "Link to this table"){.headerlink}
:::

So, for example, the following program echos a string to the terminal, which is the default stream for `stdout`{.docutils .literal .notranslate} and `stdin`{.docutils .literal .notranslate}:

::: {.cell .tag_output_scroll .tag_remove-input .docutils .container}
::: {.cell_output .docutils .container}
:::
:::

While the same program can have its output redirected to a file:

::: {.cell .tag_output_scroll .tag_remove-input .docutils .container}
::: {.cell_output .docutils .container}
:::
:::

And we can see that the contents of this file are the same as what was previously written to the terminal by using the `cat`{.docutils .literal .notranslate} program, which writes the contents of a file to its `stdout`{.docutils .literal .notranslate}, i.e., the terminal:

::: {.cell .tag_output_scroll .tag_remove-input .docutils .container}
::: {.cell_output .docutils .container}
:::
:::

::: {.margin .admonition .note}
Note

This probably seems obvious to a modern reader, i.e., an object-oriented design, where you can do the same operations on any object. However, at the time, it was a radical idea when operating systems had specialized interfaces for files with records, devices such as terminals, etc...
:::

This fundamental idea introduced by UNIX, that you can use the same `read`{.docutils .literal .notranslate} and `write`{.docutils .literal .notranslate} operations on any kind of I/O object, is very powerful. It enables a single program, depending on how it is launched by the shell, to work on data stored in a file system, data entered on a keyboard, or even on data sent over a network by other processes. By introducing the idea of a special file object called a *pipe*, you could allow programs to be combined together to do much more powerful tasks. The **\|** symbol tells the shell to create a pipe that connects the output of one program to the input of the next program. So, let's say we are trying to find all the programs on our computer that have anything to do with perl; the following command will: 1) list the contents of the `/usr/bin/`{.docutils .literal .notranslate} directory, 2) send the output of that listing to a `grep`{.docutils .literal .notranslate} program that searches for the word perl, and 3) send the output of that `grep`{.docutils .literal .notranslate} to a program that counts the number of lines of input received.

::: {.cell .tag_output_scroll .tag_remove-input .docutils .container}
::: {.cell_output .docutils .container}
:::
:::

Today, the idea of *everything is a file* has been taken much further in Linux. Linux now exposes all kinds of information through synthetic file systems, giving users and administrators massive ability to automate. For example, in the `bash`{.docutils .literal .notranslate} shell we are using `$$`{.docutils .literal .notranslate} lets us know the `id`{.docutils .literal .notranslate} of the bash process itself. So, stealing a nice example from [jonathan](https://jappavoo.github.io/UndertheCovers/textbook/unix/shellintro.html#standard-output-and-redirection){.reference .external}, the following command shows a portion of the open file table for the bash process that executes the command:

::: {.cell .tag_remove-input .docutils .container}
::: {.cell_output .docutils .container}
:::
:::

We can see that file descriptors 0, 1 and 2 (`stdin`{.docutils .literal .notranslate}, `stdout`{.docutils .literal .notranslate} and `stderr`{.docutils .literal .notranslate}) all refer to the same file, and we can learn more about this file using another command:

::: {.cell .tag_remove-input .docutils .container}
::: {.cell_output .docutils .container}
:::
:::

Now we can see that our `stdin`{.docutils .literal .notranslate}, `stdout`{.docutils .literal .notranslate}, and `stderr`{.docutils .literal .notranslate} all point to a character special file, which is used to represent a terminal in Unix. We can write to that same special device and it will appear in our terminal.

::: {.cell .tag_remove-input .docutils .container}
::: {.cell_output .docutils .container}
:::
:::

I would strongly encourage reading the shell and Unix sections of [Under the Covers: The Secret Life of Software](https://jappavoo.github.io/UndertheCovers/textbook/intro_tb.html#under-the-covers-the-secret-life-of-software){.reference .external} for a much more detailed coverage of this material. However, hopefully this has given you enough information to understand the power Unix unleashed by introducing polymorphism in the operating system, and creating a shell that enables you to combine all kinds of programs together in complicated ways.

The remainder of this chapter introduces the core abstractions of Unix, and the system calls you use on those examples, all with examples from a shell. By the end of this chapter, you should understand how a shell can start and control the execution of other programs, including how the `stdin`{.docutils .literal .notranslate}, `stdout`{.docutils .literal .notranslate}, and `stderr`{.docutils .literal .notranslate} I/O streams used by a process can be manipulated to enable the seamless composition of programs.
:::

::: {#process-management .section}
[]{#cont-gs-abstractions-process}

## [4.2. ]{.section-number}Process management[\#](#process-management "Link to this heading"){.headerlink}

As discussed [[previously]{.std .std-ref}](structure.html#cont-gs-structure-struc){.reference .internal}, a process is a virtual computer, and the kernel provides each process with: 1) an abstraction of an isolated CPU (while multiplexing the physical CPU between different processes), 2) a *virtual memory* abstraction of massive contiguous memory that starts at address `0x0`{.docutils .literal .notranslate}, and 3) a set of file abstractions that allow the process to persist data and communicate with other processes. After discussing the state maintained by the kernel, we discuss the interfaces the shell (or any application) can use to manipulate processes.

::: {#state .section}
### [4.2.1. ]{.section-number}State[\#](#state "Link to this heading"){.headerlink}

As shown in [[Fig. 4.2]{.std .std-numref}](#img-intro-proc){.reference .internal}, the kernel maintains a table of all processes, indexed by the *process id*, or `PID`{.docutils .literal .notranslate}, to keep track of all the information about each process. This includes a pointer to the file descriptor table (discussed [[earlier]{.std .std-ref}](#file-desc){.reference .internal}), as well as data structures to maintain CPU and memory management state. For CPU state, this includes all the registers that need to be loaded when the process runs.

![[Fig. 4.2 ]{.caption-number}[A process table in the kernel, indexed by PID, points to the file descriptor table, memory management regions, and CPU state.]{.caption-text}[\#](#img-intro-proc "Link to this image"){.headerlink}](../_images/osstructure-proc.drawio.png){style="width: 80%;"}

In today's computers, the address space, or *virtual memory*, of a process is a huge contiguous abstraction of memory that extends across addresses 0 to [\\(2\^{64}-1\\)]{.math .notranslate .nohighlight}. As shown in [[Fig. 4.3]{.std .std-numref}](#img-intro-mmlay){.reference .internal}, it is typically divided into *code* or machine-language instructions (for some reason typically called "text"), *initialized data*, consisting of read-only and read-write initialized data, *initialized-zero data*, called "BSS" for obscure historical reasons, *heap* or dynamically allocated memory, and *stack*. The *memory regions* referred to in [[Fig. 4.3]{.std .std-numref}](#img-intro-mmlay){.reference .internal} keep track of each of these regions.

![[Fig. 4.3 ]{.caption-number}[Virtual memory layout]{.caption-text}[\#](#img-intro-mmlay "Link to this image"){.headerlink}](../_images/trad-addr-space.png){style="width: 45%;"}
:::

::: {#system-calls .section}
[]{#cont-gs-abstractions-process-syscalls}

### [4.2.2. ]{.section-number}System calls[\#](#system-calls "Link to this heading"){.headerlink}

Key system calls in traditional Unix related to processes are:

-   `pid = fork(void)`{.docutils .literal .notranslate}: Create a child process that is a duplicate of the parent; return 0 in child, and `PID`{.docutils .literal .notranslate} of child in parent.

-   `exit(status)`{.docutils .literal .notranslate}: Terminate the calling process and record the status passed in for others.

-   `pid = waitpid(cpid, *status...)`{.docutils .literal .notranslate}: Wait for specified child process `cpid`{.docutils .literal .notranslate} to complete (or change state), fill `*status`{.docutils .literal .notranslate} with the status passed on child's exit, and garbage collect any kernel resources; return the `PID`{.docutils .literal .notranslate} of the child process that exited (or changed state).

-   `err = execve(program, arguments, environment)`{.docutils .literal .notranslate}: executing the file `program`{.docutils .literal .notranslate} with specified arguments and environment information

The `fork`{.docutils .literal .notranslate} system call duplicates the calling process (referred to as the *parent*) into a new *child* process, where the only difference that enables the parent and child to distinguish themself is the return value. You can think of this logically as creating a copy of all the process memory, copying the CPU state, and copying the file descriptor table (while incrementing reference counts on all the files pointed to by the file descriptor table).

Unix maintains a process tree in the kernel, where every process has a parent, and a parent may have many children. For example, below I run the bash shell several times, and then print out the process tree (see `man ps`{.docutils .literal .notranslate} for arguments). You can see that ps is a child of bash, which is a child of bash, and so on.

::: {.cell .tag_remove-input .docutils .container}
::: {.cell_output .docutils .container}
:::
:::

The `exit`{.docutils .literal .notranslate} system call causes the process to complete, passing in a status for the reason and `waitpid`{.docutils .literal .notranslate} waits for a *process* to change state, and if it has exited, returns the status passed in by `exit`{.docutils .literal .notranslate}. While most of the process state is freed (e.g., the file descriptor table and memory regions) by `exit`{.docutils .literal .notranslate}, the process descriptor stays around to keep track of this status information. As a result, if another process does not do a wait on a process, it will become a **zombie** (yes, that is a real Unix term) holding on to a process descriptor in the kernel forever.

The `execve`{.docutils .literal .notranslate} system call executes a new program replacing the memory regions (BSS, text, ...) of the calling process with memory from the file which the `program`{.docutils .literal .notranslate} argument points to. The CPU state is set to pass in the arguments, and the file descriptor table is not modified. Note, `exec`{.docutils .literal .notranslate} will never return unless there was some kind of failure; it is the same process just executing a different program.
:::

::: {#examples .section}
[]{#cont-gs-abstractions-process-example}

### [4.2.3. ]{.section-number}Examples[\#](#examples "Link to this heading"){.headerlink}

Okay let's look at some code to better understand how these process-related system calls are used, starting with `fork()`{.docutils .literal .notranslate}.

::: {#testfork-listing .literal-block-wrapper .docutils .container}
::: code-block-caption
[Listing 4.1 ]{.caption-number}[testfork.c - A simple program to illustrate fork()]{.caption-text}[\#](#testfork-listing "Link to this code"){.headerlink}
:::

::: {.highlight-c .notranslate}
::: highlight
     1#include <sys/types.h>
     2#include <unistd.h>
     3#include <stdio.h>
     4#include <stdlib.h>
     5
     6int
     7main(int argc, char* argv[]) 
     8{
     9  pid_t mypid, cpid, ppid;
    10  cpid = fork();
    11  ppid = getppid();
    12  mypid = getpid();
    13
    14  if (cpid > 0) {
    15    /* Parent code */ 
    16    printf("hello, from parent with pid %d, pid of child is %d\n", mypid, cpid);
    17  } else if (cpid == 0) {
    18    /* Child code */
    19    printf("hello, I am child with pid %d, my parent is %d\n", mypid, ppid);
    20  } else {
    21    perror("fork failed\n");
    22    exit(-1);
    23  }
    24  return 0;
    25} 
:::
:::
:::

The result of running the code in [[Listing 4.1]{.std .std-numref}](#testfork-listing){.reference .internal} is:

::: {.cell .tag_remove-input .docutils .container}
::: {.cell_output .docutils .container}
:::
:::

The parent prints out the child `pid`{.docutils .literal .notranslate} that it gets from `fork`{.docutils .literal .notranslate}, and then its `pid`{.docutils .literal .notranslate} (from calling `getpid()`{.docutils .literal .notranslate}). You can see that these values match the pid that the child gets from `getppid()`{.docutils .literal .notranslate}. Again, please use man to find out about any of these system calls.

To see how one can use the combination of `fork`{.docutils .literal .notranslate} and `exec`{.docutils .literal .notranslate} to start a new program, and wait until that program completes, see [[Listing 4.2]{.std .std-numref}](#doforke-listing){.reference .internal} below. Note that it is an error if the procedure returns from `exec`{.docutils .literal .notranslate}. Also, note that the parent explicitly waits for the `pid`{.docutils .literal .notranslate} of the child returned by fork on line 22, and then returns that status.

::: {#doforke-listing .literal-block-wrapper .docutils .container}
::: code-block-caption
[Listing 4.2 ]{.caption-number}[doforke.c - A simple program to illustrate fork() and exec()]{.caption-text}[\#](#doforke-listing "Link to this code"){.headerlink}
:::

::: {.highlight-default .notranslate}
::: highlight
     1#include <sys/types.h>
     2#include <unistd.h>
     3#include <stdio.h>
     4#include <stdlib.h>
     5#include <sys/wait.h>
     6#include "doforke.h"
     7
     8
     9int
    10do_fork_exec(char *prog, char *const argv[])
    11{
    12  pid_t cpid;
    13  int status=0;
    14  cpid = fork();
    15  if (cpid < 0) {
    16    perror("fork failed\n");
    17    exit(-1);
    18  }
    19
    20  if (cpid != 0) {
    21    // parent code, we need to wait for child
    22    waitpid(cpid,&status,0);
    23  } else {
    24    execve(prog, argv, 0);
    25    perror("should never get here\n");
    26  }
    27  return status;
    28} 
:::
:::
:::
:::

::: {#summary .section}
### [4.2.4. ]{.section-number}Summary[\#](#summary "Link to this heading"){.headerlink}

So, you should now understand the abstraction of a process as a virtual computer, with CPU state and virtual memory. A process (parent) can create another process (child) by calling `fork`{.docutils .literal .notranslate} which causes the kernel to create a child with a duplicate of the CPU state and virtual memory of the parent. The child, like children everywhere, can decide to be different from its parent by `exec`{.docutils .literal .notranslate} of a different program. In that case the kernel looks at the program, and creates a new virtual address space by loading (potentially lazily as we will see) the text, initialized, and uninitialized data segments of the program into memory. You can now see how to implement the core part of any shell, reading from `stdin`{.docutils .literal .notranslate} the names of programs to execute, and creating new processes to execute those programs.
:::
:::

::: {#file-system .section}
[]{#cont-gs-abstractions-fs}

## [4.3. ]{.section-number}File system[\#](#file-system "Link to this heading"){.headerlink}

Normally, the programs to be executed come out of a file system, and we are often using redirection (e.g., `>`{.docutils .literal .notranslate}) to set the input or output of the program into some file in a file system. We will discuss [[later]{.std .std-ref}](../fs/interface.html#cont-fs-interface){.reference .internal} in much more detail the abstractions of a file system, but for now we briefly introduce the key information you need to know. First, it is important to realize that all Unix file systems organize information in a hierarchy as shown in [[Fig. 4.4]{.std .std-numref}](#fs-tree-logical-abs){.reference .internal}.

![[Fig. 4.4 ]{.caption-number}[Logical view: hierarchical file system name space]{.caption-text}[\#](#fs-tree-logical-abs "Link to this image"){.headerlink}](../_images/filesys-tree.png){style="width: 45%;"}

We talked earlier about doing an exec, and with the `execve`{.docutils .literal .notranslate} call above, you need to specify the absolute path name to the program being executed. For example, if you want to run the cat program, the argument to `execve`{.docutils .literal .notranslate} on our system would be `/usr/bin/cat`{.docutils .literal .notranslate}.

You can tell the shell where to search for executable programs by specifying a `PATH`{.docutils .literal .notranslate} *environment variable*. For example, the following `echo`{.docutils .literal .notranslate} tells you the list of directories where the shell should look for executables, such as the program `cat`{.docutils .literal .notranslate}. The subsequent `type`{.docutils .literal .notranslate} command tells you where the shell will find an executable for `cat`{.docutils .literal .notranslate}.

::: {.cell .tag_remove-input .docutils .container}
::: {.cell_output .docutils .container}
:::
:::

Notice that the path to `cat`{.docutils .literal .notranslate} appears in the `PATH`{.docutils .literal .notranslate} variable shown by the `echo`{.docutils .literal .notranslate} command. So, a shell could go through each element of the path environment variable searching for a program. Thankfully, there is a whole family of library calls built on top of the `execve`{.docutils .literal .notranslate} system call that does this work for you (see `execlp`{.docutils .literal .notranslate} from the `man`{.docutils .literal .notranslate} page below, for example).

::: {.cell .tag_output_scroll .tag_remove-input .docutils .container}
::: {.cell_output .docutils .container}
:::
:::

Some of the system calls specific to file systems are:

-   `int desc = open(pathname, O_READ)`{.docutils .literal .notranslate}: Verify that file `name`{.docutils .literal .notranslate} exists and may be read, and then return a *descriptor* which may be used to refer to that file when reading it.

-   `int desc = open(pathname, O_WRITE | flags, mode)`{.docutils .literal .notranslate}: Verify permissions and open `name`{.docutils .literal .notranslate} for writing, creating it (or erasing existing contents) if necessary as specified in `flags`{.docutils .literal .notranslate}. Returns a descriptor which may be used for writing to that file.

-   `close(desc)`{.docutils .literal .notranslate}: stop using this descriptor, decrement reference count in the file, and, if the reference count is zero, free any resources allocated for it.

Every process has associated with it a *current working directory* . If the `pathname`{.docutils .literal .notranslate} argument to `open`{.docutils .literal .notranslate} starts with a `/`{.docutils .literal .notranslate}, then it is an absolute path from the top of the file tree. If it doesn't, then it is interpreted relative to the current working directory. This is convenient, since often you are doing all your work in your own directory, and you don't need to figure out where that is in the whole file system.

The unix command `pwd`{.docutils .literal .notranslate} tells you the current working directory that the shell is currently executing in, e.g.:

::: {.cell .tag_output_scroll .tag_remove-input .docutils .container}
::: {.cell_output .docutils .container}
:::
:::

A `close`{.docutils .literal .notranslate} call tells the kernel you are not using a file anymore, However, the kernel can't free up resources until the reference count goes to zero, since others may be using the same file. On a fork, the kernel increments a reference count on each of the files, since now both the parent and child processes have it open, and both the parent and the child should close the file.
:::

::: {#changing-stdin-and-stdout .section}
## [4.4. ]{.section-number}Changing stdin and stdout[\#](#changing-stdin-and-stdout "Link to this heading"){.headerlink}

So far, we have seen how a shell can start another process (via `fork`{.docutils .literal .notranslate}) and how this child process can start running a different program (via `exec`{.docutils .literal .notranslate}), as well as how to open a file in the file system. Recall that the shell process has file descriptors 0, 1 and 2 (`stdin`{.docutils .literal .notranslate}, `stdout`{.docutils .literal .notranslate} and `stderr`{.docutils .literal .notranslate}) pointing to a character special file that represents a terminal, meaning that its input comes from a user typing characters in the terminal, and its output is displayed in the terminal. Recall also that the open file table is copied to the child process on a `fork`{.docutils .literal .notranslate} and is unchanged by an `exec`{.docutils .literal .notranslate}, so the child process running the new program will also receive its input from, and send its output to, the same terminal.

Now we will see how to support the `<`{.docutils .literal .notranslate} and `>`{.docutils .literal .notranslate} I/O redirection operators in the shell, which allow a process to read its input from a file, or write its output to a file, respectively. All we need to do is get the kernel to change the file descriptor table, so that descriptors 0 or 1 point to the specified input or output files. We can also redirect the standard error output, descriptor 2, to a file in a similar way.

Whenever we need the kernel to do something on behalf of a process, we need a system call, and for this purpose we use the `dup`{.docutils .literal .notranslate} system calls:

-   `err = dup(oldfd)`{.docutils .literal .notranslate} : creates a copy of the file descriptor `oldfd`{.docutils .literal .notranslate}, using the lowest-numbered unused file descriptor for the new descriptor.

-   `err = dup2(oldfd, newfd)`{.docutils .literal .notranslate} : creates a copy of the file descriptor `oldfd`{.docutils .literal .notranslate}, to `newfd`{.docutils .literal .notranslate}; closing `newfd`{.docutils .literal .notranslate} if there is already an entry there.

So, imagine we have the following shell script:

` foo > /tmp/bar`{.docutils .literal .notranslate}

The shell would:

1.  `fork`{.docutils .literal .notranslate} a child process to execute the program `foo`{.docutils .literal .notranslate}

2.  In the child process:

    1.  `open`{.docutils .literal .notranslate} a file called `bar`{.docutils .literal .notranslate} in the directory `/tmp`{.docutils .literal .notranslate}

    2.  use `dup2`{.docutils .literal .notranslate} to modify its `stdout`{.docutils .literal .notranslate} to use the file descriptor returned by the open

    3.  `exec`{.docutils .literal .notranslate} the program `foo`{.docutils .literal .notranslate}

Great, now we know how to write a shell that can start a process that writes data into a file or reads data from a file specified by the user. How do we get programs to talk to each other without staging it through a file?
:::

::: {#pipes .section}
[]{#cont-gs-abstractions-pipes}

## [4.5. ]{.section-number}Pipes[\#](#pipes "Link to this heading"){.headerlink}

A *pipe* is a Unix kernel abstraction to allow communication between processes. A `read`{.docutils .literal .notranslate} of the pipe will return data previously written to it in a first-in-first-out (FIFO) fashion. Pipes are unidirectional communication channels represented by a pair of file descriptors -- data can only be written into one end of the pipe, and read out of the other end. A programmer can create a pipe, and then use operations that change the entries in the file descriptor table to tie the output of one program to the input of another.

A pipe is created with the following system call:

-   `err = pipe(&fdpair[0])`{.docutils .literal .notranslate}: creates a pipe where `fdpair`{.docutils .literal .notranslate} is an array of two file descriptors returned by the kernel.

After this call, `fdpair[0]`{.docutils .literal .notranslate} will have the descriptor for the entry in the file descriptor table for the read end of the pipe, and `fdpair[1]`{.docutils .literal .notranslate} will refer to the write end of the pipe. Data written to the write end of the pipe is buffered by the kernel until it is read from the read end of the pipe. A read from an empty pipe will block until there is some data in it, and will then return the max of the buffered data and the request size of the read.

To see how this is used, look at the following code (stolen from the Linux `man`{.docutils .literal .notranslate} page for `pipe`{.docutils .literal .notranslate}) in [[Listing 4.3]{.std .std-numref}](#pipe-listing){.reference .internal}:

::: {#pipe-listing .literal-block-wrapper .docutils .container}
::: code-block-caption
[Listing 4.3 ]{.caption-number}[pipe.c - A simple program that sends its argument through a pipe.]{.caption-text}[\#](#pipe-listing "Link to this code"){.headerlink}
:::

::: {.highlight-default .notranslate}
::: highlight
     1#include <sys/types.h>
     2#include <sys/wait.h>
     3#include <stdio.h>
     4#include <stdlib.h>
     5#include <unistd.h>
     6#include <string.h>
     7
     8int
     9main(int argc, char *argv[])
    10{
    11  int pipefd[2];
    12  pid_t cpid;
    13  char buf;
    14  
    15  if (argc < 2) {
    16    fprintf(stderr, "Usage: %s <string>\n", argv[0]);
    17    exit(EXIT_FAILURE);
    18  }
    19  
    20  if (pipe(pipefd) == -1) {
    21    perror("pipe");
    22    exit(EXIT_FAILURE);
    23  }
    24  
    25  cpid = fork();
    26  if (cpid == -1) {
    27    perror("fork");
    28    exit(EXIT_FAILURE);
    29  }
    30  
    31  if (cpid == 0) {    /* Child reads from pipe */
    32    // close(pipefd[1]);          /* Close unused write end */
    33    
    34    while (read(pipefd[0], &buf, 1) > 0)
    35      write(STDOUT_FILENO, &buf, 1);
    36    
    37    write(STDOUT_FILENO, "\n", 1);
    38    close(pipefd[0]);
    39    _exit(EXIT_SUCCESS);
    40    
    41  } else {            /* Parent writes argv[1] to pipe */
    42    close(pipefd[0]);          /* Close unused read end */
    43    write(pipefd[1], argv[1], strlen(argv[1]));
    44    close(pipefd[1]);          /* Reader will see EOF */
    45    wait(NULL);                /* Wait for child */
    46    exit(EXIT_SUCCESS);
    47  }
    48}
:::
:::
:::

The child code just sits in a loop reading from the pipe and then writing to `stdout`{.docutils .literal .notranslate} (lines 34-35). The parent just writes its first argument (`argv[1]`{.docutils .literal .notranslate}) to the write side of the pipe (line 43).

Note, on line 32 and line 42, we see that each process closes the side of the pipe they are not using. This is important, since, as mentioned above, the reference counts for all the file descriptors are increased on a fork, so, after the fork both the parent and the child have both the read and write side of the pipe open. The only reason that the child process eventually gets a 0 result on a read (rather than blocking) is because all the references to the write side are closed after the parent executes line 44.

So, imagine we have the following shell script:

` foo | bar`{.docutils .literal .notranslate}

The shell would:

1.  create a pipe

2.  fork a process to execute foo, but before doing the `exec`{.docutils .literal .notranslate} the process should use `dup2`{.docutils .literal .notranslate} to modify its `stdout`{.docutils .literal .notranslate} to be the write side of the pipe

3.  fork a process to execute bar, and that child should use `dup2`{.docutils .literal .notranslate} to modify its `stdin`{.docutils .literal .notranslate} to the read side of the pipe before doing the `exec`{.docutils .literal .notranslate}.

Now we can start two processes, executing different programs, that talk directly to each other through a pipe. These programs don't care that they are talking to each other, they work exactly the same way if they are talking to a terminal, a file or a pipe. Now we have all the pieces to write a shell that can compose different programs to, for example, tell me how many programs in `/usr/bin`{.docutils .literal .notranslate} have something to do with `perl`{.docutils .literal .notranslate}:

::: {.cell .tag_output_scroll .tag_remove-input .docutils .container}
::: {.cell_output .docutils .container}
:::
:::
:::

::: {#signals-protecting-against-dreaded-zombies .section}
[]{#cont-gs-abstractions-signals}

## [4.6. ]{.section-number}Signals protecting against dreaded zombies[\#](#signals-protecting-against-dreaded-zombies "Link to this heading"){.headerlink}

When we talked about processes, we wrote a well-behaved shell that started another process using `fork`{.docutils .literal .notranslate} and then waited for it to finish. What would happen if we didn't wait? Both the shell and the program it started would run at the same time, or at least as we will talk about [[later]{.std .std-ref}](../scheduling/intro.html#cont-vp){.reference .internal}, the kernel causes the hardware to take turns running one and then the other. This is exactly what the symbol `&`{.docutils .literal .notranslate} does, i.e., tells the shell to let the program run in parallel. As an example, if I am building something complicated, I will often do it in parallel while continuing to work on my shell, e.g., the following command runs make, redirecting all its output into the file RES, and then returns control to the user. You can every so often look at RES to see if the make is done.

::: {.cell .tag_output_scroll .tag_remove-input .docutils .container}
::: {.cell_output .docutils .container}
:::
:::

While this is great for the user who can now use the shell to run multiple programs concurrently, there is a problem. If the child finishes, it will exit with its status, but it will become a zombie if the shell never waits for it. After a while, the system will be filled with zombies and come to a grinding halt.

The way Unix deals with this is by sending a signal to a parent process when a child finishes. A signal is, for a virtual computer, similar to what an interrupt is for a physical computer. It tells it that some event happened on the outside world that it might want to know about.

There are a large number of signals the system can tell you about, and you can find out more about all of them with `man 7 signal`{.docutils .literal .notranslate}. In this case, the shell should register a signal handler for the `SIGCHLD`{.docutils .literal .notranslate} signal using the `sigaction`{.docutils .literal .notranslate} system call.

-   sigaction(signum, act, &oldact);

The `act`{.docutils .literal .notranslate} points to a data structure `struct sigaction`{.docutils .literal .notranslate} that describes how the caller wants to handle the signal, including a pointer to a function that will be called when the signal `signum`{.docutils .literal .notranslate} is delivered to the process. If there was previously a handler registered, the `oldact`{.docutils .literal .notranslate} tells the caller what the old action was. This allows the shell to `wait`{.docutils .literal .notranslate} for zombie children in the signal handler function when it receives notification that a child process has exited.
:::

::: {#conclusion .section}
## [4.7. ]{.section-number}Conclusion[\#](#conclusion "Link to this heading"){.headerlink}

This chapter has given you a whirlwind tour of some of the key abstractions of Unix. A process is a virtual computer, with its own virtual CPU and virtual memory. You should know how to create a new process, and tell it to execute a program.

The power of Unix is the idea that we can combine many programs together, using a shell, where the input and output of processes can be set up to be the terminal, files, or pipes. You should have an idea now on some of the key system calls that enable a shell to do this. Later chapters will discuss in much more detail the abstraction of a CPU and how it is scheduled, how memory management works and the system calls you can use to control it, and how file systems work and their system calls.
:::
:::

::: prev-next-area
[](structure.html "previous page"){.left-prev}

::: prev-next-info
previous

[3. ]{.section-number}Operating System Structure & Unix/Linux
:::

[](tools.html "next page"){.right-next}

::: prev-next-info
next

[5. ]{.section-number}What you should know
:::
:::
:::

::: {.bd-sidebar-secondary .bd-toc}
::: {.sidebar-secondary-items .sidebar-secondary__inner}
::: sidebar-secondary-item
::: {.page-toc .tocsection .onthispage}
Contents
:::

-   [4.1. Everything is a file](#everything-is-a-file){.reference .internal .nav-link}
-   [4.2. Process management](#process-management){.reference .internal .nav-link}
    -   [4.2.1. State](#state){.reference .internal .nav-link}
    -   [4.2.2. System calls](#system-calls){.reference .internal .nav-link}
    -   [4.2.3. Examples](#examples){.reference .internal .nav-link}
    -   [4.2.4. Summary](#summary){.reference .internal .nav-link}
-   [4.3. File system](#file-system){.reference .internal .nav-link}
-   [4.4. Changing stdin and stdout](#changing-stdin-and-stdout){.reference .internal .nav-link}
-   [4.5. Pipes](#pipes){.reference .internal .nav-link}
-   [4.6. Signals protecting against dreaded zombies](#signals-protecting-against-dreaded-zombies){.reference .internal .nav-link}
-   [4.7. Conclusion](#conclusion){.reference .internal .nav-link}
:::
:::
:::
:::

::: {.bd-footer-content__inner .container}
::: footer-item
By (see contributing chapter book)
:::

::: footer-item
© Copyright 2022.\
:::

::: footer-item
:::

::: footer-item
:::
:::
:::
:::
:::
