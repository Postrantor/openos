---
tip: translate by baidu@2024-07-18 12:58:46
docsearch:language: en
lang: en
title: 10.3. Scheduling with Priorities --- Introduction to Operating Systems
viewport:
  - width=device-width, initial-scale=1.0
  - width=device-width, initial-scale=1
  - width=device-width, initial-scale=1
---

# Scheduling with Priorities

## Contents

# [10.3. ] {.section-number}Scheduling with Priorities[\#](#scheduling-with-priorities "Link to this heading") {.headerlink}

We first discuss scheduling with fixed priorites for real time, and then how priorities can be used dynamically to support an interactive system.

> 我们首先讨论实时固定优先级的调度，然后讨论如何动态使用优先级来支持交互式系统。

## [10.3.1. ] {.section-number}Fixed Priority[\#](#fixed-priority "Link to this heading") {.headerlink}

The core idea behind priority scheduling is that some processes may be more important than others and should be given access to the CPU first. For example, one reasonable assumption might be that tasks of students should only run if there are no tasks from professors. To implement this policy, the OS maintains two or more priority queues which hold tasks assigned to the corresponding priority. Runnable processes in a lower priority queue are only run if there are none in a higher priority queues. Figure [[Fig. 10.8]{.std .std-numref}](#priority-sched){.reference .internal} shows a simple example of a system with 4 priority queues. In this snapshot, the next process to be given CPU time will be the first process in the priority 4 queue. Assuming no additions, the processes in queue 3 will not run until all of the ones in 4 have completed.

> 优先级调度背后的核心思想是，一些进程可能比其他进程更重要，应该首先访问 CPU。例如，一个合理的假设可能是，只有当教授没有任务时，学生的任务才应该运行。为了实施此策略，操作系统维护两个或多个优先级队列，这些队列保存分配给相应优先级的任务。只有当高优先级队列中没有可运行的进程时，低优先级队列中的可运行进程才会运行。图[[图 10.8]{.std.std numref}]（#priority sched）{.reference.internal}显示了一个具有 4 个优先级队列的系统的简单示例。在此快照中，下一个需要 CPU 时间的进程将是优先级 4 队列中的第一个进程。假设没有添加，队列 3 中的进程将不会运行，直到 4 中的所有进程都完成。

![[Fig. 10.8 ]{.caption-number}[A simple example of a system with 5 priority queues and runnable processes in several of the queues.]{.caption-text}[#](#priority-sched "Link to this image"){.headerlink}](../_images/Priority.png)

Let us consider a situation with three tasks shown in the table below:

::: pst-scrollable-table-container
Task Start Runtime Priority

---

A 0 6 1
B 1 2 3
C 2 2 3
D 3 1 5
:::

In that case, a priority scheduler will run tasks as shown in [[Fig. 10.9]{.std .std-numref}](#vp-sched-pr){.reference .internal} below:

> 在这种情况下，优先级调度器将运行如下[[图 10.9]{.std.std-numref}]（#vp-scched-pr）{.reference.internal}所示的任务：

![[Fig. 10.9 ]{.caption-number}[Priority scheduling, where every task executes for a quantum of time.]{.caption-text}[#](#vp-sched-pr "Link to this image"){.headerlink}](../_images/Priority-tl.png)

A runs by itself until B becomes ready to run. We then preempt A after it has accumulated one second of run time, and context switch to B since it is higher priority. When C starts running, it is the same priority as B, so they share the CPU (i.e., we switch back and forth between them every quantum). At time 3, D enters with the highest priority, and we stop running B and C to just run it. At that point, B has accumulated 1.5 sec of runtime, and C has accumulated .5 seconds. Once D is done, we again share the CPU using round robin between B and C, until B has accumulated its full 2 seconds of runtime, after which we can use the CPU just for running C. Finally, at second 6, all the other tasks are done and A, the lowest priority task, can be run until it completes. The average turnaround time here is [\\(((4-3) + (5-1) + (6-2) + 11)/4 = 5\\)]{.math .notranslate .nohighlight} seconds.

> A 自己跑，直到 B 准备好跑。然后，在 A 累积了一秒钟的运行时间后，我们抢占它，并将上下文切换到 B，因为它具有更高的优先级。当 C 开始运行时，它与 B 具有相同的优先级，因此它们共享 CPU（即，我们在每个量子之间来回切换）。在时间 3，D 以最高优先级进入，我们停止运行 B 和 C 来运行它。此时，B 已经累积了 1.5 秒的运行时间，C 已经累积了 0.5 秒。D 完成后，我们再次使用轮询在 B 和 C 之间共享 CPU，直到 B 累积了整整 2 秒的运行时间，之后我们可以只使用 CPU 运行 C。最后，在第 6 秒，所有其他任务都完成了，最低优先级的任务 A 可以运行直到完成。这里的平均周转时间为[\\（（4-3）+（5-1）+（6-2）+11）/4=5\\）]秒。

Note, one challenge with a fixed priority scheme is that low priority work can starve if there is always higher priority work entering the system.

> 请注意，固定优先级方案的一个挑战是，如果总是有更高优先级的工作进入系统，低优先级的工作可能会饿死。

::: {#tradeoffs .section}

### [10.3.1.1. ] {.section-number}Tradeoffs[\#](#tradeoffs "Link to this heading") {.headerlink}

- **Requirements:**

  - User must specify priority of high priority work

- **The Good:**

  - Supports real time for high priority

- **The Bad:**

  - Bad for tasks that alternate between I/O and CPU
  - Doesn't do anything to maintain high utilization of non-CPU resources
  - Poor turnaround time
  - Wouldn't use for batch
  - Can result in Starvation
    :::
    :::

::: {#variable-priority-or-multilevel-feedback .section}
[]{#cont-scheduling-scheduling-policies-mlf}

## [10.3.2. ] {.section-number}Variable Priority or Multilevel feedback[\#](#variable-priority-or-multilevel-feedback "Link to this heading") {.headerlink}

While round robin does a better job than run to completion it doesn't do a good job for I/O bound tasks. If there are many CPU intensive tasks. Consider the case of 100 CPU intensive tasks that each consume their full quantum of, say, 10msec. If the I/O intensive task only runs for a few usec, and then does some quick I/O, it might have to wait for [\\(10msec \* 100 = 1 sec\\)]{.math .notranslate .nohighlight} before it gets to run again. What we really want to do is to prioritize I/O intensive tasks. Unfortunately, we don't know which tasks are CPU or I/O intensive a-priori, and further a task may go back and forth between being CPU and I/O intensive.

> 虽然循环比运行到完成做得更好，但它对 I/O 受限的任务做得不好。如果有许多 CPU 密集型任务。考虑 100 个 CPU 密集型任务的情况，每个任务消耗其全部时间，比如 10 毫秒。如果 I/O 密集型任务只运行几次 usec，然后进行一些快速 I/O，则可能需要等待[\\（10msec\*100=1 秒\\）]{.math.notranslate.nohighlight}才能再次运行。我们真正想做的是优先处理 I/O 密集型任务。不幸的是，我们事先不知道哪些任务是 CPU 或 I/O 密集型的，而且一个任务可能会在 CPU 和 I/O 密集型之间来回切换。

A very popular scheduling algorithm for this is called **Multilevel** feedback. It assumes the same kind of data structure shown in [[Fig. 10.9]{.std .std-numref}](#vp-sched-pr){.reference .internal}. One simple varient of the algorithm is:

> 一种非常流行的调度算法称为**多级**反馈。它假设与[[图 10.9]{.std.std-numref}]（#vp-scched-pr）{.reference.internal}中所示的数据结构相同。该算法的一个简单变体是：

- When a task first starts running, we assume it is I/O intensive, and add it to the highest priority queue.

> -当任务首次开始运行时，我们假设它是 I/O 密集型的，并将其添加到最高优先级队列中。

- if a task consumes an entire quantum, we assume it is more CPU intensive, and decrease its priority by one before adding it to the runqueue.

> -如果一个任务消耗了整个量子，我们假设它的 CPU 密集度更高，并在将其添加到运行队列之前将其优先级降低 1。

- If a task performs I/O before its quantum expires, when it becomes runnable we increase its priority (up to the highest level) before adding it to the runqueue.

> -如果一个任务在其数量到期之前执行 I/O，当它变得可运行时，我们会在将其添加到运行队列之前增加其优先级（最高级别）。

- To avoid starvation, we periodically move all the tasks to the highest priority queue.

Note, a system can support both fixed priorities, e.g., for real time tasks, and a range of priorities for dealing with general purpose tasks.

> 请注意，系统既可以支持固定优先级（例如实时任务），也可以支持处理通用任务的一系列优先级。

::: {#id1 .section}

### [10.3.2.1. ] {.section-number}Tradeoffs[\#](#id1 "Link to this heading") {.headerlink}

- **Requirements:**

  - requires no knowledge of task run time

- **The Good:**

  - Good for interactive tasks and maintaining high utilization of non-cpu resources

- **The Bad:**

  - Bad for real time and batch

  - While it can deal with starvation by periodically moving tasks to high priority queue, this is a bit of a hack rather than an intrinsic part of the algorithm.

> -虽然它可以通过定期将任务移动到高优先级队列来处理饥饿问题，但这有点像黑客攻击，而不是算法的固有部分。

    :::
    :::
    :::
