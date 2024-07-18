---
tip: translate by baidu@2024-07-18 13:01:41
docsearch:language: en
lang: en
title: 8. Virtualizing the CPU --- Introduction to Operating Systems
viewport:
  - width=device-width, initial-scale=1.0
  - width=device-width, initial-scale=1
  - width=device-width, initial-scale=1
---

# Virtualizing the CPU

# [8. ] {.section-number}Virtualizing the CPU[\#](#virtualizing-the-cpu "Link to this heading") {.headerlink}

When we say "virtualizing" what we mean is actually adding a layer of indirection between the target (in this case the CPU) and the source (the process), enabling multiple processes to take turns using the same CPU; that is time multiplexing the CPU. In order to do this, we will need a way of pausing the execution of a process while another process runs and then resuming execution later without the process having to be aware of this pause, which means we need to capture all of the state that is relevant to a process in one or more data structures we can use to hold them when the process is not active. When the OS changes the active process on a CPU, we call this a **context switch**. To complete a context switch we need to save the CPU state for the process coming off the CPU and then load the state for the incoming process before allowing the CPU to execute the incoming process.

> 当我们说“虚拟化”时，我们的意思实际上是在目标（在这种情况下是 CPU）和源（进程）之间添加一层间接层，使多个进程能够轮流使用同一 CPU；即对 CPU 进行时间复用。为了做到这一点，我们需要一种方法，在另一个进程运行时暂停一个进程的执行，然后稍后恢复执行，而进程不必意识到这种暂停，这意味着我们需要在一个或多个数据结构中捕获与进程相关的所有状态，以便在进程不活动时保存它们。当操作系统更改 CPU 上的活动进程时，我们称之为**上下文切换**。为了完成上下文切换，我们需要保存 CPU 下进程的 CPU 状态，然后在允许 CPU 执行传入进程之前加载传入进程的状态。

Definitions:

- Process: A virtual computer
- Thread: A virtual CPU, where a process has at least one and possibly many
- Task: Term to refer to either process or thread

- Context switching: Switching the processor from running one task to another, i.e., saving the processor registers used by the running task into its thread struc, and loading some other task's registers into the CPU.

> -上下文切换：将处理器从运行一个任务切换到另一个任务，即将运行任务使用的处理器寄存器保存到其线程结构中，并将其他任务的寄存器加载到 CPU 中。

- Scheduling: Deciding which task to run.
- Preemption: Stopping a task to run another one.

![[Fig. 8.1 ]{.caption-number}[For each process, a task structure contains information about each of the processes. All processes that are ready to run are on a queue]{.caption-text}[#](#img-vp-proc "Link to this image"){.headerlink}](../_images/vp-osstruc.png){style="width: 60%;"}

We stated [[earlier]{.std .std-ref}](../intro/abstractions.html#cont-gs-abstractions-process){.reference .internal} (see [[Fig. 4.2]{.std .std-numref}](../intro/abstractions.html#img-intro-proc){.reference .internal}) the kernel maintains a table of all processes, indexed by the _process id_, or **pid**, to keep track of all the information about each process. For reasons that will soon make sense, rather than processes, we will refer here to the abstraction that the kernel runs on the processor as a **task**, although feel free to think about a task as being a process for the time being. As shown in [[Fig. 4.2]{.std .std-numref}](../intro/abstractions.html#img-intro-proc){.reference .internal}, the kernel maintains a data structures, we call here a `run queue`{.docutils .literal .notranslate} for scheduling the tasks on the CPU. On a single CPU (actually single core) system, only one task can run at a time, and the kernel is responsible for selecting the task to be run and switching between them.

> 我们声明[[早期]{.std.std-ref}]（../intro/nabstracts.html#cont-abstractions process）{.reference.internal}（参见[[图 4.2]{.sdt.std-numref}]（…./intro/inabstracts.html#img-intro proc）{.requiry.internal}）内核维护一个所有进程的表，由*process id*或**pid**索引，以跟踪每个进程的所有信息。出于很快就会有意义的原因，而不是进程，我们在这里将内核在处理器上运行的抽象称为**任务**，尽管暂时可以将任务视为进程。如[[图 4.2]{.std.std-numref}]（../intro/nabstracts.html#img-intro-proc）{.reference.internal}所示，内核维护着一个数据结构，我们在这里称之为“运行队列”{.docutils.literal.notranslate}，用于在 CPU 上调度任务。在单 CPU（实际上是单核）系统上，一次只能运行一个任务，内核负责选择要运行的任务并在它们之间进行切换。

For each task, the kernel maintains a pointer to the file descriptor table, the memory management data structures (i.e. the map described above) and information about execution state of the task. For example, [[Listing 8.1]{.std .std-numref}](#simple-task-struct){.reference .internal} shows a highly simplified version of the `task_struct`{.docutils .literal .notranslate} data structure used by Linux. The state field indicates if the task is currently running, is blocked for some reason, or is ready and waiting to be run. The thread structure is a place for the kernel to store all the processor registers whenever the task is not running.

> 对于每个任务，内核都维护一个指向文件描述符表、内存管理数据结构（即上述映射）和任务执行状态信息的指针。例如，[[清单 8.1]{.std.std numref}]（#simple task struct）{.reference.internal}显示了 Linux 使用的`task_struct`{.docutils.literal.notranslate}数据结构的高度简化版本。状态字段指示任务当前是否正在运行，是否因某种原因被阻止，或者是否已准备好等待运行。线程结构是内核在任务不运行时存储所有处理器寄存器的地方。

::: {.margin .admonition .note}
Note

What else is there: There is much more state in the task structure including:

> 还有什么：任务结构中还有更多的状态，包括：

- Process ID, User ID, Group ID
- Priority/Scheduling parameters
- Accounting information
- Signal management functions

- Working directory To see the actual data structure, you can use the online browser for the current linux code base, and search for `task_struct`{.docutils .literal .notranslate} at this [link](https://elixir.bootlin.com/linux/latest/source/include/linux/sched.h#L746){.reference .external}.

> -工作目录要查看实际的数据结构，您可以使用当前 linux 代码库的在线浏览器，并在此[链接]上搜索`task_struct`{.docutils.literal.notranslate}(https://elixir.bootlin.com/linux/latest/source/include/linux/sched.h#L746){.reference.external}。
> :::

::: {#simple-task-struct .literal-block-wrapper .docutils .container}
::: code-block-caption

[Listing 8.1 ]{.caption-number}[A highly simplified version of the Linux task struct from the kernel include file linux/sched.h]{.caption-text}[\#](#simple-task-struct "Link to this code"){.headerlink}

> [清单 8.1]｛.caption number｝[来自内核的 Linux 任务结构体的高度简化版本，包括文件 Linux/sched.h]｛.ception text｝[\#]（#简单任务结构体“链接到此代码”）｛.headerlink｝
> :::

```c
struct task_struct {
  // the state of the task: running, blocked, runable
  unsigned int  __state;

  // CPU-specific state of this task
  struct thread_struct            thread;

  // a pointer to the memory management data structures
  struct mm_struct                *mm;

  // Open file information
  struct files_struct             *files;
}
```

[[Fig. 8.2]{.std .std-numref}](#img-vp-states){.reference .internal} shows the three possible states for a task, with all the valid state transitions represented by arrows. A task in the Running state is one that is currently active on a CPU. Processes do many things other than just use the CPU, e.g., they read data from files, communicate with other processes, etc... For example, as I type this, the process is constantly blocked waiting for me to type characters. Some examples of blocking operations are: issuing a read from disk or from a network socket that does not have data ready, issuing a write to a pipe that has no more space to buffer data, trying to acquire certain kinds of resources that are already owned by another process or thread, etc.

> [[图 8.2]{.std.std-numref}]（#img vp-states）{.reference.internal}显示了任务的三种可能状态，所有有效的状态转换都由箭头表示。处于运行状态的任务是 CPU 上当前处于活动状态的任务。进程除了使用 CPU 外，还做许多其他事情，例如，它们从文件中读取数据，与其他进程通信等。例如，当我键入此内容时，进程不断被阻止，等待我键入字符。阻塞操作的一些示例是：从没有准备好数据的磁盘或网络套接字发出读取，向没有更多空间缓冲数据的管道发出写入，尝试获取已由另一个进程或线程拥有的某些类型的资源等。

![[Fig. 8.2 ]{.caption-number}[Task states]{.caption-text}[#](#img-vp-states "Link to this image"){.headerlink}](../_images/ProcessLifecycle.png){style="width: 200pt;"}

In these situations, the process must wait for something external to happen before it can make progress (e.g., data arrives over the network, another process reads some data out of the pipe, the requested resource is released by another process, etc.), and is unable to make use of the CPU until that event occurs. We would be wasting the limited CPU resource if we left such a process on the CPU, and there is no point considering it among the set of runnable processes that we might want to choose next either. Tasks that are waiting for something go into the **Blocked** state, the kernel removes them from the run queue, saves all the processor registers into the thread structure, and then make a **scheduling** decision to select some other process to run from the run queue. The kernel changes the state of the selected task from **Ready** to **Running** and loads its registers from the task structures into the CPU registers.

> 在这些情况下，进程必须等待外部事件发生才能取得进展（例如，数据通过网络到达，另一个进程从管道中读取一些数据，请求的资源由另一个过程释放等），并且在该事件发生之前无法使用 CPU。如果我们把这样的进程留在 CPU 上，我们将浪费有限的 CPU 资源，而且在我们接下来可能想要选择的可运行进程集中考虑它也没有意义。等待的任务进入**阻塞**状态，内核将其从运行队列中删除，将所有处理器寄存器保存到线程结构中，然后做出**调度**决定，从运行队列选择其他进程运行。内核将所选任务的状态从**就绪**更改为**运行**，并将其寄存器从任务结构加载到 CPU 寄存器中。

The process of switching the CPU between two tasks is called a **Context Switch**. Context switches are expensive for two reasons. First, there is overhead to save the state (i.e., CPU registers) of the outgoing process, select the next process to run, and load the state of the incoming task. Second, even though we are saving all the state needed to resume a process, modern processors have several caches (e.g., data and instruction caches, the translation look aside buffer, etc.) that help an application run more quickly. As the application runs, these caches are filled with instructions or data that are related to the executing process. When a new task is placed on a CPU, the contents of these caches are no longer related to the running process, and either need to be cleared by the OS, or need to be replaced by the new process as it executes.

> 在两个任务之间切换 CPU 的过程称为**上下文切换**。上下文切换很昂贵，原因有两个。首先，保存传出进程的状态（即 CPU 寄存器）、选择下一个要运行的进程以及加载传入任务的状态都有开销。其次，尽管我们正在保存恢复进程所需的所有状态，但现代处理器有几个缓存（例如，数据和指令缓存、翻译后备缓冲区等），可以帮助应用程序更快地运行。当应用程序运行时，这些缓存中充满了与执行进程相关的指令或数据。当一个新任务被放置在 CPU 上时，这些缓存的内容不再与正在运行的进程相关，要么需要被操作系统清除，要么需要在新进程执行时被新进程替换。

Once whatever causes the task to be blocked is resolved, the kernel changes the state of the task from **Blocked** to **Ready**, and places the task struct onto the run queue so it can be run the next time there is a scheduling decision to be made.

> 一旦解决了导致任务被阻塞的任何问题，内核就会将任务的状态从**已阻塞**更改为**就绪**，并将任务结构放入运行队列中，以便下次做出调度决策时可以运行。

A task may also transition from the **Running** to the **Ready** state without going through the **Blocked** state. Some tasks may run for a really long time without doing any I/O. This can cause a problem for other tasks that are constantly blocking and doing get their fair share of the processor. To handle this, all systems have hardware timers, where the kernel can configure the timer to cause an interrupt at some future time. When the interrupt occurs, the kernel stops the current task, and makes a scheduling decision to context switch to some other task. This is called **Preemption**, where the kernel stops, or **Preempts** a task to run another one.

> 任务也可能从**运行**转换到**就绪**状态，而不经过**阻塞**状态。有些任务可能会在不进行任何 I/O 的情况下运行很长时间。这可能会给其他不断阻塞的任务带来问题，并导致它们在处理器中获得公平的份额。为了处理这个问题，所有系统都有硬件定时器，内核可以配置定时器在未来的某个时间造成中断。当中断发生时，内核会停止当前任务，并做出调度决策，将上下文切换到其他任务。这被称为**抢占**，其中内核停止，或**抢占**一个任务以运行另一个任务。
> :::
