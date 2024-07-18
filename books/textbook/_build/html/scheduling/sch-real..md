---
tip: translate by baidu@2024-07-18 13:07:04
docsearch:language: en
lang: en
title: 10.4. Scheduling in the real world --- Introduction to Operating Systems
viewport:
  - width=device-width, initial-scale=1.0
  - width=device-width, initial-scale=1
  - width=device-width, initial-scale=1
---

# Scheduling in the real world

## Contents

# [10.4. ] {.section-number}Scheduling in the real world[\#](#scheduling-in-the-real-world "Link to this heading") {.headerlink}

We briefly review some of the real world scheduling issues and approaches from a Linux perspective.

> 我们从 Linux 的角度简要回顾了一些现实世界中的调度问题和方法。

::: {#multi-cpu-scheduling .section}

## [10.4.1. ] {.section-number}Multi-CPU scheduling[\#](#multi-cpu-scheduling "Link to this heading") {.headerlink}

Today almost all systems have multiple CPUs. Early multi-CPU systems looked something like [[Fig. 10.10]{.std .std-numref}](#smp-hw){.reference .internal} below. If you compare with the simple computer picture we showed in the past ([[Fig. 2.1]{.std .std-numref}](../intro/purpose.html#simplecomputer-fig){.reference .internal}), there are just a modest number of CPUs accessing both the memory and I/O buses.

> 如今，几乎所有的系统都有多个 CPU。早期的多 CPU 系统看起来像下面的[[图 10.10]{.std.std-numref}]（#smp-hw）{.reference.internal}。如果你与我们过去展示的简单计算机图片（[[图 2.1]{.std.std-numref}]（../intro/epurpose.html#simplecomputer-Fig）{.reference.internal}）相比，只有少量 CPU 同时访问内存和 I/O 总线。

![[Fig. 10.10 ]{.caption-number}[Early multiprocessors]{.caption-text}[#](#smp-hw "Link to this image"){.headerlink}](../_images/SMP.png){style="width: 50%;"}

The easiest solution, and the one first adopted by most operating systems to support these computers, was to have a single runqueue in the kernel. This is both simple, and fair, since whatever algorithm you apply for scheduling selects the best task to run irrespective of which CPU becomes available.

> 最简单的解决方案，也是大多数操作系统首次采用的支持这些计算机的解决方案是在内核中有一个运行队列。这既简单又公平，因为无论你应用什么算法进行调度，都会选择最好的任务来运行，而不管哪个 CPU 可用。

Unfortunately, today's systems look more like [[Fig. 10.11]{.std .std-numref}](#numa-hw){.reference .internal}. They have memory controllers and I/O controllers in _sockets_, which is really just a processor chip. The sockets have a large number of CPUs (or cores) each with their own caches, and a shared cache per socket. Memory is directly attached to one of the sockets, and all accesses from other sockets have to go through it; leading to Non-Uniform Memory Access (NUMA).

> 不幸的是，今天的系统看起来更像[[图 10.11]{.std.std-numref}]（#numa-hw）{.reference.internal}。它们在*sockets*中有内存控制器和 I/O 控制器，这实际上只是一个处理器芯片。套接字有大量的 CPU（或内核），每个 CPU 都有自己的缓存，每个套接字都有一个共享缓存。内存直接连接到其中一个插槽，其他插槽的所有访问都必须通过它；导致非统一存储器访问（NUMA）。

![[Fig. 10.11 ]{.caption-number}[Todays Multiprocessors]{.caption-text}[#](#numa-hw "Link to this image"){.headerlink}](../_images/NUMA.png){style="width: 50%;"}

In today's systems a shared runqueue results in terrible performance. First, if you have hundreds of cores, the run queue itself becomes a bottleneck since only one CPU at a time can add or remove tasks from the queue. Second, with today's large caches, you often want to run a task on the same CPU it ran on recently to reduce cache misses. Third, modern systems are NUMA, or Non Unform Memory Access (NUMA), and you want to run a task on a CPU near the memory allocated to it.

> 在当今的系统中，共享运行队列会导致糟糕的性能。首先，如果你有数百个内核，运行队列本身就会成为瓶颈，因为一次只有一个 CPU 可以在队列中添加或删除任务。其次，对于当今的大型缓存，您通常希望在最近运行的同一 CPU 上运行任务，以减少缓存未命中。第三，现代系统是 NUMA，即非不规则内存访问（NUMA），您希望在分配给它的内存附近的 CPU 上运行任务。

Most systems have a seperate run queue per CPU, and use some algorithm to shift tasks from one CPU to another if the imbalance between the CPUs becomes too large. The simplest algorithm, called take, has any CPU that becomes idle look at the load on the other CPUs to try to steal work. You can see [here](https://elixir.bootlin.com/linux/latest/source/kernel/sched/fair.c#L11206){.reference .external} the current code in Linux for the load_balancer that is called whenever a runqueue is empty and periodically to re-balance work across the runqueus.

> 大多数系统每个 CPU 都有一个单独的运行队列，如果 CPU 之间的不平衡变得太大，就会使用一些算法将任务从一个 CPU 转移到另一个 CPU。最简单的算法称为 take，它可以让任何空闲的 CPU 查看其他 CPU 的负载，试图窃取工作。你可以看到[这里](https://elixir.bootlin.com/linux/latest/source/kernel/sched/fair.c#L11206){.reference.external}Linux 中 load_balancer 的当前代码，每当运行队列为空时调用该代码，并定期在运行队列之间重新平衡工作。
> :::

::: {#scheduling-in-linux .section}

## [10.4.2. ] {.section-number}Scheduling in Linux[\#](#scheduling-in-linux "Link to this heading") {.headerlink}

Given the enormous number of platforms Linux runs on, that covers everything from Batch scheduling HPC systems, to desktops, to embedded real time, the scheduling system has had to become incredibly adaptable. You can find out a huge amount about it from the man page:

> 考虑到 Linux 运行的平台数量巨大，涵盖了从批处理调度 HPC 系统到台式机再到嵌入式实时的所有内容，调度系统必须变得非常具有适应性。你可以在手册页上找到大量关于它的信息：

::: {.cell .tag_output_scroll .tag_remove-input .docutils .container}
::: {.cell_output .docutils .container}
:::
:::

Several snippets we would like to draw your attention to that relate strongly to the materials we have presented:

> 我们想提请您注意与我们提供的材料密切相关的几个片段：

- Processes scheduled under one of the real-time policies (SCHED_FIFO, SCHED_RR) have a sched_priority value in the range 1 (low) to 99 (high). (As the numbers imply, real-time threads always have higher priority than normal threads.) Conceptually, the scheduler maintains a list of runnable threads for each possible sched_priority value. In order to determine which thread runs next, the scheduler looks for the non empty list with the highest static priority and selects the thread at the head of this list.

> -在其中一个实时策略（SCHED_FIFO、SCHED_RR）下调度的进程的 SCHED_priority 值在 1（低）到 99（高）的范围内。（正如数字所暗示的那样，实时线程总是比普通线程具有更高的优先级。）从概念上讲，调度器为每个可能的 sched_priority 值维护一个可运行线程的列表。为了确定下一个运行哪个线程，调度器会查找具有最高静态优先级的非空列表，并选择该列表开头的线程。

- All scheduling is preemptive: if a thread with a higher static priority becomes ready to run, the currently running thread will be preempted and returned to the wait list for its static priority level. The scheduling policy determines the ordering only within the list of runnable threads with equal static priority.

> -所有调度都是抢占式的：如果具有较高静态优先级的线程准备运行，则当前运行的线程将被抢占并返回到其静态优先级的等待列表中。调度策略仅确定具有相等静态优先级的可运行线程列表中的顺序。

- Linux supports a number of policies that might sound familiar that can be specified on a per-task basis:

> -Linux 支持许多听起来很熟悉的策略，这些策略可以在每个任务的基础上指定：

- SCHED_FIFO: tasks will immediately preempt any currently running SCHED_OTHER, SCHED_BATCH, or SCHED_IDLE thread. SCHED_FIFO is a simple scheduling algorithm without time slicing.

> -SCHED_FIFO：任务将立即抢占任何当前正在运行的 SCHED_OTHER、SCHED_BATH 或 SCHED_IDLE 线程。SCHED_FIFO 是一种没有时间切片的简单调度算法。

- SCHED_RR: Round-robin scheduling - incorporates a quantum.

- SCHED_DEADLINE: Sporadic task model deadline scheduling; period real time tasks, where user specifies the period, expected Runtime, and Deadline

> -SCHED_DEADLINE：零星任务模型截止日期调度；周期实时任务，其中用户指定周期、预期运行时间和截止日期

- SCHED_OTHER (or SCHED_NORMAL): Default Linux time-sharing scheduling the standard Linux time-sharing scheduler that is intended for all threads that do not require the special real-time mechanisms. One can use **nice** to specify, depending on the schedular, the relative importance of different tasks.

> -SCHED_OTHER（或 SCHED_NORMAL）：默认的 Linux 分时调度——标准的 Linux 分时间调度程序，适用于不需要特殊实时机制的所有线程。根据日程安排，可以使用**nice**指定不同任务的相对重要性。

- SCHED_BATCH: This policy will cause the scheduler to always assume that the thread is CPU-intensive.

> -SCHED_BATCH：此策略将导致调度程序始终假设线程是 CPU 密集型的。

- SCHED_IDLE: This policy is used for running jobs at extremely low priority.

Only privaledged tasks can set static prioritis; appropriate for single user systems where someone can specify the absolute priority of different work. The RLIMIT_RTTIME resource limit to set a ceiling on the CPU time that a real-time process may consume in order to gaurantee that real time tasks cannot cause starvation.

> 只有隐藏的任务才能设置静态优先级；RLIMIT_RTTIME 资源限制，为实时进程可能消耗的 CPU 时间设定上限，以确保实时任务不会导致饥饿。

Prior to kernel version 2.6.23, the normal scheduler for Linux combined priority queues with a heuristic that altered a process's priority based on the amount of a time slice it used. CPU-bound processes would consume their entire slice and would drop in priority. Conversely, I/O-bound processes would often block before consuming an entire time slice and so their priority would be increased. This was meant to allow for interactive processes to stay in the high priority queues and batch processing jobs (really anything that was CPU-bound) to drop. This scheduler had a number of heuristics that were used in decision making that were also exposed as tunable parameters, but the biggest feature it boasted was that it had O(1) run time. In other words, the time to select the next process was constant, regardless of how many runnable processes there were in the system. This is basically a varient of the [[MLF]{.std .std-ref}](sch-prio.html#cont-scheduling-scheduling-policies-mlf){.reference .internal} we have discussed.

> 在内核版本 2.6.23 之前，Linux 的常规调度程序将优先级队列与启发式方法相结合，该启发式方法根据进程使用的时间片数量改变进程的优先级。CPU 受限的进程将消耗其整个切片，并降低优先级。相反，I/O 受限的进程在消耗整个时间片之前通常会阻塞，因此它们的优先级会提高。这意味着允许交互式进程留在高优先级队列中，并删除批处理作业（实际上是任何 CPU 受限的作业）。该调度器有许多用于决策的启发式方法，这些方法也被公开为可调参数，但它最大的特点是它有 O（1）的运行时间。换句话说，无论系统中有多少可运行的进程，选择下一个进程的时间都是恒定的。这基本上是我们讨论过的[[MLF]{.std.std-ref}]（sch prio.html#cont 调度策略 MLF）{.reference.internal}的变体。

The completely fair scheduler was a from-scratch redesign of the Linux scheduler; it did away with priority queues and with all[[\[]{.fn-bracket}1[\]]{.fn-bracket}](#notall){#id1 .footnote-reference .brackets role="doc-noteref"} heuristics and tunables found in the O(1) scheduler. CFS introduced keeping a counter for the amount of runtime each task has received and this counter is used to decide on the next task to run. Instead of priority queues CFS places all tasks in a red-black tree sorted on their accumulated runtime with tasks on the left having less accumulated run time than tasks on the right. When the system needs a new task to run, the left most task is selected. This change allows CFS to completely avoid the starvation of CPU bound tasks that could occur with the previous scheduler.

> 完全公平的调度器是 Linux 调度器的从头开始重新设计；它取消了优先级队列和所有[[\[]{.fn-bracket}1[\]]{.fn 括号}]（#notall）{#id1.脚注引用.carbles role=“doc noteref”}O（1）调度器中的启发式和可调参数。CFS 引入了为每个任务接收到的运行时间量保留一个计数器，该计数器用于决定下一个要运行的任务。CFS 将所有任务放置在红黑树中，而不是优先级队列中，按照其累积的运行时间进行排序，左侧的任务的累积运行时间比右侧的任务少。当系统需要运行新任务时，会选择最左侧的任务。这一变化使 CFS 能够完全避免前一个调度程序可能出现的 CPU 受限任务的饥饿。
