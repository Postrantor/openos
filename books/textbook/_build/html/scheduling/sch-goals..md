---
tip: translate by baidu@2024-07-18 13:02:40
docsearch:language: en
lang: en
title: 10.1. Scheduling Goals --- Introduction to Operating Systems
viewport:
  - width=device-width, initial-scale=1.0
  - width=device-width, initial-scale=1
  - width=device-width, initial-scale=1
---

# Scheduling Goals

# [10.1. ] {.section-number}Scheduling Goals[\#](#scheduling-goals "Link to this heading") {.headerlink}

We need to make a scheduling decision whenever a task completes (process or thread exits) or if the task blocks, for example doing I/O. We can make a scheduling decision when a new task is created (i.e., we could choose to switch to the child) when an I/O interrupt occurs that might unblock a task, or if a task has been running for a long time (i.e., the kernel schedules a timer interrupt to preempt the currently running task)

> 每当任务完成（进程或线程退出）或任务阻塞时，我们都需要做出调度决策，例如进行 I/O。当创建新任务时（即，我们可以选择切换到子任务），当发生可能解除阻止任务的 I/O 中断时，或者当任务已经运行了很长时间时（即内核调度计时器中断以抢占当前运行的任务），我们可以做出调度决策

It seems fair to just take turns between different tasks. To understand why scheduling is more complicated, consider [[Fig. 10.1]{.std .std-numref}](#img-vp-cpuvsio){.reference .internal} which shows how two hypothetical tasks would use the CPU if they where running by themselves. One of the tasks is CPU intensive, using the processor for long periods of time, while the other task spends most of its time blocked on I/O. If we just took turns running the different tasks, as soon as task 2 blocks for the first time, task 2 would get the CPU for a long time. Not only is task 2 not getting its fair share of the CPU, but if task 2 was using a disk we are wasting the resources of our computer since if task 2 could get just a little bit of CPU it would be using the disk while task 1 was using the CPU. Also, if task 2 was, for example, running emacs, every time the user typed a key emacs take a long time to respond since it wouldn't get run again until task 1, which is perhaps spending hours on bitcoin mining, stopped running.

> 在不同的任务之间轮流似乎是公平的。要理解为什么调度更复杂，请考虑[[图 10.1]{.std.std-numref}]（#img vp-cpuvsio）{.reference.internal}，它显示了两个假设的任务在单独运行时将如何使用 CPU。其中一个任务是 CPU 密集型的，需要长时间使用处理器，而另一个任务的大部分时间都被阻塞在 I/O 上。如果我们只是轮流运行不同的任务，一旦任务 2 第一次阻塞，任务 2 就会长时间占用 CPU。任务 2 不仅没有得到公平的 CPU 份额，而且如果任务 2 使用的是磁盘，我们就是在浪费计算机的资源，因为如果任务 2 只能得到一点点 CPU，它就会在任务 1 使用 CPU 的同时使用磁盘。此外，例如，如果任务 2 正在运行 emacs，那么每次用户键入一个关键 emacs 都需要很长时间才能响应，因为直到任务 1 停止运行，它才会再次运行，而任务 1 可能需要花费数小时进行比特币挖矿。

![[Fig. 10.1 ]{.caption-number}[Figure shows how two tasks would use the CPU if they where running by themselves. Task 1 is a CPU intensive, wanting to use the CPU for long periods of time, while Task 2 is IO intensive, blocking frequently to interact with some I/O device.]{.caption-text}[#](#img-vp-cpuvsio "Link to this image"){.headerlink}](../_images/cpuvsio.png){style="width: 80%;"}

Scheduling policies may aim for different goals, for example, a system may try to give all tasks an equal share of the CPU. They may also try to implement some kind of policy, for example, students should only get to use the CPU whenever professors don't need it. Or, they might try to maximize the number of tasks that complete per unit time, or minimize how long tasks take on average. They can also try to schedule the CPU in such a fashion to maximize the utilization of all the resources of the computer; e.g., run I/O intensive tasks whenever they are not blocked so they will keep the I/O devices busy. On the other hand, as we have discussed, context switching can be expensive, so if you are constantly preempting the running process you are wasting many resources. This is all complicated by the fact that the system may not know how long tasks will take, if they are I/O or CPU intensive, etc... Perhaps you can understand why researchers have published thousands and thousands of papers on different scheduling polices over the years. To make things worse, while we are focused here on scheduling the CPU, as we will see later, to achieve any goal one needs to also schedule memory and even the disk head; achieving an end-to-end goal for a

> 调度策略可能针对不同的目标，例如，系统可能会尝试为所有任务分配相等的 CPU 份额。他们也可能试图实施某种政策，例如，学生应该只在教授不需要的时候使用 CPU。或者，他们可能会试图最大限度地增加每单位时间完成的任务数量，或者尽量减少任务的平均耗时。他们还可以尝试以这样的方式调度 CPU，以最大限度地利用计算机的所有资源；例如，只要 I/O 密集型任务未被阻止，就运行这些任务，这样它们将使 I/O 设备保持忙碌。另一方面，正如我们所讨论的，上下文切换可能代价高昂，因此如果你不断抢占正在运行的进程，你会浪费很多资源。这一切都很复杂，因为系统可能不知道任务需要多长时间，如果它们是 I/O 或 CPU 密集型的，等等……也许你能理解为什么研究人员多年来发表了成千上万篇关于不同调度策略的论文。更糟糕的是，当我们在这里专注于调度 CPU 时，正如我们稍后将看到的，要实现任何目标，还需要调度内存，甚至磁盘头；实现一个端到端的目标

Applications and/or systems can care about:

- **Turnaround time**: The time from when a task entered the system until it was done.
- **Throughput**: The rate that tasks complete at.
- **Response time**: How long does it take for an application to respond to external events.

- **Fairness**: How fairly are the resources of the computer shared between the tasks, e.g., if we have two tasks do they both get equal shares of the CPU.

> -**公平性**：任务之间共享计算机资源的公平程度，例如，如果我们有两个任务，它们是否都获得了相等的 CPU 份额。

- **Predictability**: The guarantees on run time that a task can get.

- **Starvation**: Is it possible for some tasks to never run when the demand on the system is high.

> -**饥饿**：当系统需求很高时，某些任务是否可能永远不会运行。

These requirements are often in tension with each other and designing a scheduling algorithm is an act of balancing trade offs for the requirements of the OS.

> 这些要求往往相互矛盾，设计调度算法是平衡操作系统要求的一种行为。

We should note that these metrics are generally not just about the scheduling, for example, response time depends not just on how long after a resource is available does the scheduler take to context switch to the right task, but also how long that task takes to execute once it is scheduled to respond to the request. Also, the time the task takes depends not only on its processing requirements, but also how much of its state is in the CPU caches, if any of its state needs to be brought in from disk, etc... its complicated.

> 我们应该注意到，这些指标通常不仅仅是关于调度的，例如，响应时间不仅取决于资源可用后调度器需要多长时间才能将上下文切换到正确的任务，还取决于任务在计划响应请求后需要多长时间来执行。此外，任务所需的时间不仅取决于其处理要求，还取决于其状态在 CPU 缓存中的占比，是否需要从磁盘引入任何状态等……这很复杂。

With cloud computing, we have switched from caring about average response time, to tail latency. In the cloud, a request may hit hundreds of computers, and we care about [\\(99.9\\%\\)]{.math .notranslate .nohighlight} tail latency, i.e., the response time for all but [\\(0.1%\\)]{.math .notranslate .nohighlight} of the requests, since if even [\\(1\\%\\)]{.math .notranslate .nohighlight} of the requests hit a slow computer the aggregate request will be slow. While it would be nice if one could guarantee the latency of [\\(100\\%\\)]{.math .notranslate .nohighlight} of the requests, that is likely too expensive.

> 借助云计算，我们已经从关注平均响应时间转向关注尾部延迟。在云中，一个请求可能会攻击数百台计算机，我们关心[\\（99.9\\%\\）]{.math.notranslate.noheight}尾部延迟，即除[\\。虽然如果能保证请求的[\\（100\\%\\）]{.math.notranslate.nohighlight}的延迟就好了，但这可能太贵了。

General purpose systems typically have limited information about the real needs of the applications, and implement complex schedulers that try to do a good job of tradeing off between different goals we have discussed above. However a great deal of attention in scheduling has been spent on special purpose systems where more information is available, including:

> 通用系统通常对应用程序的实际需求信息有限，并实现复杂的调度器，这些调度器试图在我们上面讨论的不同目标之间很好地进行权衡。然而，在调度中，大量的注意力都花在了可以获得更多信息的专用系统上，包括：

- **Real time**: Real time systems are used in a wide class of applications from industrial controls to vehicle management to robotics. Predictability is a key requirement in each of these cases. Think of the program or programs responsible for managing an airplane in flight. The developers make decisions for the software with a guarantee that certain calculations can be made at least N times a second. If this requirement is not met, we start seeing bad and possibly dangerous behavior. Such systems typically require users to specify how long tasks will take and the relative priority of different tasks so that the system can preempting lower priority work whenever a high priority task becomes available.

> -**实时**：实时系统用于从工业控制到车辆管理再到机器人的广泛应用。在每种情况下，可预测性都是一个关键要求。想想负责管理飞行中的飞机的程序。开发人员为软件做出决策，并保证某些计算每秒至少可以进行 N 次。如果不满足这一要求，我们就会开始看到不良和可能危险的行为。这样的系统通常要求用户指定任务需要多长时间以及不同任务的相对优先级，以便系统可以在高优先级任务可用时抢占较低优先级的工作。

- **Batch**: These are systems where the user submits jobs without any further interaction until the job completes. Early mainframes where all based on batch processing, where users submitted jobs with punch cards. Today, most high performance computing systems, where jobs consume enormous resources and run for long periods of time, use batch processing to enable the very expensive resources of the computer to be used efficiently. These systems typically run tasks to completion to avoid any overhead of preemption and require users to specify how long tasks will run so they can schedule all the required resources.

> -**批处理**：在这些系统中，用户在作业完成之前无需任何进一步交互即可提交作业。早期的大型机都是基于批处理的，用户用穿孔卡片提交作业。如今，大多数高性能计算系统，其中作业消耗大量资源并长时间运行，都使用批处理来有效地利用计算机的昂贵资源。这些系统通常将任务运行到完成，以避免任何抢占开销，并要求用户指定任务将运行多长时间，以便他们可以调度所有所需的资源。

While general purpose operating systems cannot achieve the efficiency or predictability of specialized systems, they do need to support some applications with different requirements. As we will see, they provide mechanisms, such as priority, to provide some control over the scheduling of applications. While historically large HPC machines and embedded devices relied on special purpose systems, today specialized configurations of Linux has captured more and more of the requirements of these systems.

> 虽然通用操作系统无法达到专用系统的效率或可预测性，但它们确实需要支持一些具有不同要求的应用程序。正如我们将看到的，它们提供了优先级等机制，以对应用程序的调度提供一些控制。虽然历史上大型 HPC 机器和嵌入式设备依赖于专用系统，但如今 Linux 的专用配置已经满足了这些系统越来越多的需求。
> :::
