---
tip: translate by baidu@2024-07-18 13:08:50
docsearch:language: en
lang: en
title: 10.2. Simple Examples of Scheduling Policies --- Introduction to Operating Systems
viewport:
  - width=device-width, initial-scale=1.0
  - width=device-width, initial-scale=1
  - width=device-width, initial-scale=1
---

# Simple Examples of Scheduling Policies

## Contents

# [10.2. ] {.section-number}Simple Examples of Scheduling Policies[\#](#simple-examples-of-scheduling-policies "Link to this heading") {.headerlink}

Now that we have a collection of requirements, let's look at a few simple possibilities.

> 现在我们有了一系列需求，让我们来看看一些简单的可能性。

Definitions: We use some previously introduced terms, and add a few more:

- **Context switch**: Switching the CPU from running one task to another, i.e., saving the processor registers used by the running task into its thread struc, and loading some other task's registers into the CPU.

> -**上下文切换**：将 CPU 从运行一个任务切换到另一个任务，即将运行任务使用的处理器寄存器保存到其线程结构中，并将其他任务的寄存器加载到 CPU 中。

- **Preemption**: Stopping a task to run another one.
- **Response time**: How long does it take for an application to respond to external events.

- **Quantum** or **Time slice**: The amount of time that a task is allowed to run before the kernel preempts it to run another.

> -**量子**或**时间片**：一个任务在内核抢占它运行另一个任务之前允许运行的时间量。

::: {#first-come-first-served-fcfs .section}

## [10.2.1. ] {.section-number}First Come, First Served (FCFS)[\#](#first-come-first-served-fcfs "Link to this heading") {.headerlink}

The simplest scheduling policy just processes each task to completion in the order that they arrived. Just like waiting in line at the local government office, each process gets into a queue and the processor executes the first process in that queue until it completes. Then we repeat the same.

> 最简单的调度策略只是按照任务到达的顺序处理每个任务直至完成。就像在当地政府办公室排队一样，每个进程都会进入一个队列，处理器会执行该队列中的第一个进程，直到它完成。然后我们重复同样的事情。

One problem with the FCFS policy is that it can result in poor average turnaround time. Let us consider a situation with three tasks that arrive at around the same start time with the run time shown in the table below:

> FCFS 策略的一个问题是，它可能会导致平均周转时间很短。让我们考虑一种情况，其中三个任务的开始时间与下表所示的运行时间大致相同：

::: pst-scrollable-table-container

```
Task Start Runtime (min)

---

A \~0 6
B \~0 2
C \~0 1
```

:::

If they are run in the order A, B, C, they will execute on the processor as shown below.

> 如果它们按照 A、B、C 的顺序运行，它们将在处理器上执行，如下所示。

![[Fig. 10.2 ]{.caption-number}[FIFO with tasks run in order A, then B, then C]{.caption-text}[#](#vp-sched-fifo "Link to this image"){.headerlink}](../_images/FIFO-1.png)

So the average turnaround time is: [\\((6 + 8 + 9)/3 = 7.7 min\\)]{.math .notranslate .nohighlight}

> 因此，平均周转时间为：[\\（6+8+9）/3=7.7 分钟\\）]{.math.notranslate.noheight}

On the other hand, if the tasks are run in the order C, B, A, they will execute on the processor as shown below.

> 另一方面，如果任务按 C、B、A 的顺序运行，它们将在处理器上执行，如下所示。

![[Fig. 10.3 ]{.caption-number}[FIFO with tasks run in order C, then B, then A]{.caption-text}[#](#vp-sched-fifo2 "Link to this image"){.headerlink}](../_images/FIFO-2.png)

So the average turnaround time is: [\\((1 + 3 + 9)/3 = 4.7 min\\)]{.math .notranslate .nohighlight}

> 因此，平均周转时间为：[\\（1+3+9）/3=4.7 分钟\\）]{.math.notranslate.nohighlight}

We see here that when short tasks are processed after long tasks the long ones have a major impact on the short ones, while if the order is reversed, the impact on the long tasks running after the short ones is much less.

> 我们在这里看到，当短任务在长任务之后处理时，长任务对短任务有重大影响，而如果顺序颠倒，对短任务之后运行的长任务的影响要小得多。

::: {#tradeoffs .section}

### [10.2.1.1. ] {.section-number}Tradeoffs[\#](#tradeoffs "Link to this heading") {.headerlink}

- **Requirements:**

  - requires no information from user

- **The Good:**

  - a very simple algorithm; can make sense for Batch since there is no context switching

- **The Bad:**

  - Poor average turnaround time

  - Not appropriate for response time sensitive since they don't get to run until all tasks ahead of them have completed and no mechanism to support real time workloads

> -不适合响应时间敏感型，因为它们只有在前面的所有任务都完成后才能运行，而且没有支持实时工作负载的机制

- Doesn't do anything to maintain high utilization of non-CPU resources
  :::
  :::

::: {#shortest-job-first-sjf .section}

## [10.2.2. ] {.section-number}Shortest Job First (SJF)[\#](#shortest-job-first-sjf "Link to this heading") {.headerlink}

For some systems, for example Batch, we know a-priori how long a task will take. Hence, rather than running them in the order they arrived, we can sort them based on how long the tasks will take and always run the shortest tasks first to get the better turnaround time shown in [[Fig. 10.3]{.std .std-numref}](#vp-sched-fifo2){.reference .internal}. This policy is called shortest job first, and will always yield the optimal turnaround time.

> 对于某些系统，例如 Batch，我们先验地知道任务需要多长时间。因此，我们可以根据任务需要多长时间对它们进行排序，而不是按照它们到达的顺序运行它们，并且总是先运行最短的任务，以获得更好的周转时间，如[[图 10.3]{.std.std-numref}]（#vp-sched-fifo2）{.reference.internal}所示。这种策略被称为“最短作业优先”，并且总是会产生最佳的周转时间。

Let us, however, consider the case below, where tasks A and B arrive at time 0, and tasks C, D, and E arrive at time 3.

> 然而，让我们考虑下面的情况，任务 A 和 B 在时间 0 到达，任务 C、D 和 E 在时间 3 到达。

::: pst-scrollable-table-container

```
Task Start Runtime (min)

---

A 0 2
B 0 4
C 3 1
D 3 1
E 3 1
```

:::

If we run jobs to completion we will get the following:

![[Fig. 10.4 ]{.caption-number}[SJF without preemption]{.caption-text}[#](#vp-sched-sjf1 "Link to this image"){.headerlink}](../_images/SJF-1.png)

So the average turnaround time is: [\\((2+6+(7-3)+(8-3)+(9-3))/5 = 4.6 min\\)]{.math .notranslate .nohighlight}

> 因此，平均周转时间为：[\\（（2+6+（7-3）+（8-3）/（9-3））/5=4.6 分钟\\）]{.math.notranslate.noheight}

If we instead preempt B to run the new jobs who's time is shorter than B's remaining time, we get the following execution:

> 如果我们抢先 B 运行时间比 B 剩余时间短的新作业，我们会得到以下执行：

![[Fig. 10.5 ]{.caption-number}[SJF with preemption]{.caption-text}[#](#vp-sched-sjf2 "Link to this image"){.headerlink}](../_images/SJF-2.png)

With a shorter average turnaround time of [\\((2+(4-3)+(5-3)+(6-3)+9)/5 = 3.4\\)]{.math .notranslate .nohighlight}

> 平均周转时间更短，为[\\（（2+（4-3）+（5-3）/（6-3）+9）/5=3.4\\）]{.math.notranslate.noheight}

This demonstrates the value of preemption, where we can stop long running tasks to get short ones in and out of the system quickly.

> 这展示了抢占的价值，在抢占中，我们可以停止长时间运行的任务，以便快速将短任务放入和移出系统。

To understand the major problem with Shortest Job consider what happens if one minute tasks continue to arrive every minute starting at minute 4. B will never complete, or in scheduling terminology, it will _starve_ even though the system is processing work as fast as it is arriving. **Starvation** is a major problem with a pure shortest job first algorithm.

> 要了解最短作业的主要问题，请考虑一下，如果从第 4 分钟开始，每分钟都有一分钟的任务到达，会发生什么。B 永远不会完成，或者用调度术语来说，它将*starve*，即使系统处理工作的速度与到达的速度一样快**饥饿**是纯最短作业优先算法的一个主要问题。

::: {#id1 .section}

### [10.2.2.1. ] {.section-number}Tradeoffs[\#](#id1 "Link to this heading") {.headerlink}

- **Requirements:**

  - requires knowledge of task run time

- **The Good:**

  - Optimizes turn around time
  - Great for Batch

- **The Bad:**

  - Not appropriate for response time sensitive that perform I/O
  - Can result in starvation
  - Doesn't do anything to maintain high utilization of non-CPU resources
    :::
    :::

::: {#round-robin .section}

## [10.2.3. ] {.section-number}Round Robin[\#](#round-robin "Link to this heading") {.headerlink}

With SJF, we found that if we preempt a long running task when a short one arrives, we can improve turn around time. In many environments, we don't know how long a task will take, and, rather than just using the CPU, many tasks switch back and forth between using the CPU and doing I/O.

> 通过 SJF，我们发现，如果我们在短任务到达时抢占长时间运行的任务，我们可以缩短周转时间。在许多环境中，我们不知道一个任务需要多长时间，而且，许多任务在使用 CPU 和进行 I/O 之间来回切换，而不仅仅是使用 CPU。

We illustrated in [[Fig. 10.1]{.std .std-numref}](sch-goals.html#img-vp-cpuvsio){.reference .internal} how a CPU and I/O intensive application might use the CPU. For such tasks, if we can make sure that CPU intensive tasks don't block I/O intensive ones for too long, the system will enable the I/O intensive ones to better use the I/O devices while the CPU intensive task has only modest impact from the short periods of time that the I/O intensive ones use it. Also, if a user is interacting with the I/O intensive one, e.g. running emacs, the _Response Time_ is less affected by the CPU intensive applications.

> 我们在[[图 10.1]{.std.std-numref}]（sch-targets.html#img vp-cpuvsio）{.reference.internal}中说明了 CPU 和 I/O 密集型应用程序如何使用 CPU。对于此类任务，如果我们能确保 CPU 密集型任务不会长时间阻塞 I/O 密集型任务，系统将使 I/O 密集型的任务能够更好地使用 I/O 设备，而 CPU 密集型的工作在 I/O 密集型使用它的短时间内只会产生适度的影响。此外，如果用户正在与 I/O 密集型工作交互，例如运行 emacs，则*Response time*受 CPU 密集型应用程序的影响较小。

The _Round Robin_ algorithm builds a simple FIFO run queue of tasks in the ready state much like the FIFO algorithm described earlier. When a task starts running it is given a fixed amount of time to run, often called a _Quantum_ or _Time slice_. When the quantum expires the OS does a context switch to the next task in the queue and adds the previously running task at the back of the queue.

> *Round Robin*算法在就绪状态下构建了一个简单的 FIFO 运行队列，与前面描述的 FIFO 算法非常相似。当任务开始运行时，会给它一个固定的运行时间，通常称为*Quantum*或*time slice*。当量子到期时，操作系统会切换到队列中的下一个任务，并将之前运行的任务添加到队列的后面。

Let us consider a situation with three tasks shown in the table below:

::: pst-scrollable-table-container

```
Task   Start    Runtime

---

A      0        6
B      0.0001   2
C      0.0002   1
```

:::

Assuming the units are in seconds, let us assume that the quantum is also (unrealistically) 1 second. In that case, a round robin scheduler will run tasks as shown in [[Fig. 10.6]{.std .std-numref}](#vp-sched-rr){.reference .internal} below:

> 假设单位是秒，让我们假设量子也是（不切实际地）1 秒。在这种情况下，循环调度程序将运行如下[[图 10.6]{.std.std-numref}]（#vp-scched-rr）{.reference.internal}所示的任务：

![[Fig. 10.6 ]{.caption-number}[Round Robin scheduling, where every task executes for a quantum of time.]{.caption-text}[#](#vp-sched-rr "Link to this image"){.headerlink}](../_images/RR.png)

The average turnaround time of this round robin schedule is [\\((3 + 5 + 9)/3 = 5.6\\)]{.math .notranslate .nohighlight}. We can see that it is terrible compared to SJF, but much better than the worst FIFO case.

> 此循环时间表的平均周转时间为[\\（3+5+9）/3=5.6\\）]{.math.notranslate.nohighlight}。我们可以看到，与圣犹达相比，它很糟糕，但比最糟糕的 FIFO 情况要好得多。

The preemptive scheduling models introduces a new parameter we need to set: the length of the quantum. We have to weigh the cost of changing processes against the interactivity requirements when deciding on the length of a time we will run CPU intensive tasks. You want to pick a time large enough that you are **amortizing** the cost of a context switch; if you picked a time that was a few hundred computer cycles you would be spending most of your time context switching. On the other hand, if you it is too long, interactive tasks would get terrible response rate.

> 抢占式调度模型引入了一个我们需要设置的新参数：量子长度。在决定运行 CPU 密集型任务的时间长度时，我们必须权衡更改流程的成本和交互性要求。你想选择一个足够大的时间，以便**摊销**上下文切换的成本；如果你选择了几百个计算机周期的时间，你的大部分时间都会花在上下文切换上。另一方面，如果你的任务太长，交互式任务的响应率会很低。

Let us assume that the quantum is, say 10msec, a number much larger than the time for a context switch but reasonable to not add much delay to tasks that interact with humans. Also, we will assume that we can ignore the context switching time. We can represent what happens is shown below:

> 让我们假设量子是，比如 10 毫秒，一个比上下文切换时间大得多的数字，但合理的是不会给与人类交互的任务增加太多延迟。此外，我们将假设可以忽略上下文切换时间。我们可以将发生的事情表示如下：

![[Fig. 10.7 ]{.caption-number}[Round Robin scheduling, with a reasonable quantum.]{.caption-text}[#](#vp-sched-rr2 "Link to this image"){.headerlink}](../_images/RR2.png)

For the first three seconds, all three tasks share the CPU. Assuming that each gets an equal share, C will have had a full second of compute time after three seconds and it will be done. From seconds 3-5 the CPU is shared by tasks A and B, where each get half of it. After 5 seconds, B will have had two full seconds of compute time, and A will have the CPU to itself from that point forward.

> 在前三秒，所有三个任务共享 CPU。假设每个人都得到了相等的份额，那么 C 在三秒后将有整整一秒的计算时间，它就会完成。从第 3 秒到第 5 秒，CPU 由任务 A 和 B 共享，每个任务获得一半的 CPU。5 秒后，B 将有整整两秒的计算时间，从那时起，A 将拥有自己的 CPU。

::: {#id2 .section}

### [10.2.3.1. ] {.section-number}Tradeoffs[\#](#id2 "Link to this heading") {.headerlink}

- **Requirements:**

  - requires no knowledge of task run time

- **The Good:**

  - Simplest preemptive algorithm, better for response time than any non-preemptive one
  - Does better for non-CPU resource use than any non-preemptive algorithm

- **The Bad:**

  - Can still result in poor response time with many CPU intensive tasks
  - Poor turnaround time

  - Bad for batch since constant context switching, and real time since difficult to make any prediction on how long tasks will take

> -不利于批处理，因为持续的上下文切换，也不利于实时处理，因为很难预测任务需要多长时间

    :::
    :::
    :::
