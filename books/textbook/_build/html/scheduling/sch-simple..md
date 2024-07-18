---
docsearch:language: en
lang: en
title: 10.2. Simple Examples of Scheduling Policies --- Introduction to Operating Systems
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
[![Introduction to Operating Systems - Home](../_static/logo.png){.logo__image .only-light}](../intro/pref.html){.navbar-brand .logo}
:::

::: sidebar-primary-item
:::

::: sidebar-primary-item
::: {.bd-toc-item .navbar-nav .active}
-   [Preface](../intro/pref.html){.reference .internal}

[Getting started]{.caption-text}

-   [1. Introduction](../intro/intro.html){.reference .internal}
-   [2. Purpose of operating systems](../intro/purpose.html){.reference .internal}
-   [3. Operating System Structure & Unix/Linux](../intro/structure.html){.reference .internal}
-   [4. Operating System Abstractions](../intro/abstractions.html){.reference .internal}
-   [5. What you should know](../intro/tools.html){.reference .internal}
    []{.toctree-toggle role="presentation"}
    -   [5.1. The C Programming Language](../intro/tools-c.html){.reference .internal}
    -   [5.2. Shell](../intro/tools-shell.html){.reference .internal}
    -   [5.3. Editors](../intro/tools-editors.html){.reference .internal}
    -   [5.4. Make](../intro/tools-make.html){.reference .internal}
    -   [5.5. Testing](../intro/tools-testing.html){.reference .internal}
    -   [5.6. Git Basics](../intro/tools-git.html){.reference .internal}
    -   [5.7. GDB](../intro/tools-gdb.html){.reference .internal}

[Virtual Processor]{.caption-text}

-   [6. Introduction](intro.html){.reference .internal}
-   [7. The Process: A virtual Computer](process.html){.reference .internal}
-   [8. Virtualizing the CPU](virtual.html){.reference .internal}
-   [9. The Thread: A Virtual CPU](threads.html){.reference .internal}
-   [10. Scheduling](scheduling.html){.reference .internal}
    []{.toctree-toggle role="presentation"}
    -   [10.1. Scheduling Goals](sch-goals.html){.reference .internal}
    -   [10.2. Simple Examples of Scheduling Policies](#){.current .reference .internal}
    -   [10.3. Scheduling with Priorities](sch-prio.html){.reference .internal}
    -   [10.4. Scheduling in the real world](sch-real.html){.reference .internal}
-   [11. Review Questions](review.html){.reference .internal}

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

-   [[ ![JupyterHub logo](../_static/images/logo_jupyterhub.svg) ]{.btn__icon-container} [JupyterHub]{.btn__text-container}](https://jupyterhub-opf-jupyterhub.apps.smaug.na.operate-first.cloud/hub/user-redirect/git-pull?repo=https%3A//github.com/OpenOSOrg/openos&urlpath=lab/tree/openos/content/scheduling/sch-simple.ipynb&branch=main "Launch on JupyterHub"){.btn .btn-sm .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
:::

::: {.dropdown .dropdown-source-buttons}

-   [[ ]{.btn__icon-container} [Repository]{.btn__text-container}](https://github.com/OpenOSOrg/openos "Source repository"){.btn .btn-sm .btn-source-repository-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
-   [[ ]{.btn__icon-container} [Suggest edit]{.btn__text-container}](https://github.com/OpenOSOrg/openos/edit/main/content/scheduling/sch-simple.ipynb "Suggest edit"){.btn .btn-sm .btn-source-edit-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
-   [[ ]{.btn__icon-container} [Open issue]{.btn__text-container}](https://github.com/OpenOSOrg/openos/issues/new?title=Issue%20on%20page%20%2Fscheduling/sch-simple.html&body=Your%20issue%20content%20here. "Open an issue"){.btn .btn-sm .btn-source-issues-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
:::

::: {.dropdown .dropdown-download-buttons}

-   [[ ]{.btn__icon-container} [.ipynb]{.btn__text-container}](../_sources/scheduling/sch-simple.ipynb "Download source file"){.btn .btn-sm .btn-download-source-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
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
# Simple Examples of Scheduling Policies

::: {#print-main-content}
::: {#jb-print-toc}
<div>

## Contents

</div>

-   [10.2.1. First Come, First Served (FCFS)](#first-come-first-served-fcfs){.reference .internal .nav-link}
    -   [10.2.1.1. Tradeoffs](#tradeoffs){.reference .internal .nav-link}
-   [10.2.2. Shortest Job First (SJF)](#shortest-job-first-sjf){.reference .internal .nav-link}
    -   [10.2.2.1. Tradeoffs](#id1){.reference .internal .nav-link}
-   [10.2.3. Round Robin](#round-robin){.reference .internal .nav-link}
    -   [10.2.3.1. Tradeoffs](#id2){.reference .internal .nav-link}
:::
:::
:::

::: {#searchbox}
:::

::: {#simple-examples-of-scheduling-policies .section .tex2jax_ignore .mathjax_ignore}
[]{#cont-scheduling-scheduling-policies}

# [10.2. ]{.section-number}Simple Examples of Scheduling Policies[\#](#simple-examples-of-scheduling-policies "Link to this heading"){.headerlink}

Now that we have a collection of requirements, let's look at a few simple possibilities.

Definitions: We use some previously introduced terms, and add a few more:

-   **Context switch**: Switching the CPU from running one task to another, i.e., saving the processor registers used by the running task into its thread struc, and loading some other task's registers into the CPU.

-   **Preemption**: Stopping a task to run another one.

-   **Response time**: How long does it take for an application to respond to external events.

-   **Quantum** or **Time slice**: The amount of time that a task is allowed to run before the kernel preempts it to run another.

::: {#first-come-first-served-fcfs .section}
## [10.2.1. ]{.section-number}First Come, First Served (FCFS)[\#](#first-come-first-served-fcfs "Link to this heading"){.headerlink}

The simplest scheduling policy just processes each task to completion in the order that they arrived. Just like waiting in line at the local government office, each process gets into a queue and the processor executes the first process in that queue until it completes. Then we repeat the same.

One problem with the FCFS policy is that it can result in poor average turnaround time. Let us consider a situation with three tasks that arrive at around the same start time with the run time shown in the table below:

::: pst-scrollable-table-container
  Task   Start   Runtime (min)
  ------ ------- ---------------
  A      \~0     6
  B      \~0     2
  C      \~0     1
:::

If they are run in the order A, B, C, they will execute on the processor as shown below.

![[Fig. 10.2 ]{.caption-number}[FIFO with tasks run in order A, then B, then C]{.caption-text}[\#](#vp-sched-fifo "Link to this image"){.headerlink}](../_images/FIFO-1.png)

So the average turnaround time is: [\\((6 + 8 + 9)/3 = 7.7 min\\)]{.math .notranslate .nohighlight}

On the other hand, if the tasks are run in the order C, B, A, they will execute on the processor as shown below.

![[Fig. 10.3 ]{.caption-number}[FIFO with tasks run in order C, then B, then A]{.caption-text}[\#](#vp-sched-fifo2 "Link to this image"){.headerlink}](../_images/FIFO-2.png)

So the average turnaround time is: [\\((1 + 3 + 9)/3 = 4.7 min\\)]{.math .notranslate .nohighlight}

We see here that when short tasks are processed after long tasks the long ones have a major impact on the short ones, while if the order is reversed, the impact on the long tasks running after the short ones is much less.

::: {#tradeoffs .section}
### [10.2.1.1. ]{.section-number}Tradeoffs[\#](#tradeoffs "Link to this heading"){.headerlink}

-   **Requirements:**

    -   requires no information from user

-   **The Good:**

    -   a very simple algorithm; can make sense for Batch since there is no context switching

-   **The Bad:**

    -   Poor average turnaround time

    -   Not appropriate for response time sensitive since they don't get to run until all tasks ahead of them have completed and no mechanism to support real time workloads

    -   Doesn't do anything to maintain high utilization of non-CPU resources
:::
:::

::: {#shortest-job-first-sjf .section}
## [10.2.2. ]{.section-number}Shortest Job First (SJF)[\#](#shortest-job-first-sjf "Link to this heading"){.headerlink}

For some systems, for example Batch, we know a-priori how long a task will take. Hence, rather than running them in the order they arrived, we can sort them based on how long the tasks will take and always run the shortest tasks first to get the better turnaround time shown in [[Fig. 10.3]{.std .std-numref}](#vp-sched-fifo2){.reference .internal}. This policy is called shortest job first, and will always yield the optimal turnaround time.

Let us, however, consider the case below, where tasks A and B arrive at time 0, and tasks C, D, and E arrive at time 3.

::: pst-scrollable-table-container
  Task   Start   Runtime (min)
  ------ ------- ---------------
  A      0       2
  B      0       4
  C      3       1
  D      3       1
  E      3       1
:::

If we run jobs to completion we will get the following:

![[Fig. 10.4 ]{.caption-number}[SJF without preemption]{.caption-text}[\#](#vp-sched-sjf1 "Link to this image"){.headerlink}](../_images/SJF-1.png)

So the average turnaround time is: [\\((2+6+(7-3)+(8-3)+(9-3))/5 = 4.6 min\\)]{.math .notranslate .nohighlight}

If we instead preempt B to run the new jobs who's time is shorter than B's remaining time, we get the following execution:

![[Fig. 10.5 ]{.caption-number}[SJF with preemption]{.caption-text}[\#](#vp-sched-sjf2 "Link to this image"){.headerlink}](../_images/SJF-2.png)

With a shorter average turnaround time of [\\((2+(4-3)+(5-3)+(6-3)+9)/5 = 3.4\\)]{.math .notranslate .nohighlight}

This demonstrates the value of preemption, where we can stop long running tasks to get short ones in and out of the system quickly.

To understand the major problem with Shortest Job consider what happens if one minute tasks continue to arrive every minute starting at minute 4. B will never complete, or in scheduling terminology, it will *starve* even though the system is processing work as fast as it is arriving. **Starvation** is a major problem with a pure shortest job first algorithm.

::: {#id1 .section}
### [10.2.2.1. ]{.section-number}Tradeoffs[\#](#id1 "Link to this heading"){.headerlink}

-   **Requirements:**

    -   requires knowledge of task run time

-   **The Good:**

    -   Optimizes turn around time

    -   Great for Batch

-   **The Bad:**

    -   Not appropriate for response time sensitive that perform I/O

    -   Can result in starvation

    -   Doesn't do anything to maintain high utilization of non-CPU resources
:::
:::

::: {#round-robin .section}
## [10.2.3. ]{.section-number}Round Robin[\#](#round-robin "Link to this heading"){.headerlink}

With SJF, we found that if we preempt a long running task when a short one arrives, we can improve turn around time. In many environments, we don't know how long a task will take, and, rather than just using the CPU, many tasks switch back and forth between using the CPU and doing I/O.

We illustrated in [[Fig. 10.1]{.std .std-numref}](sch-goals.html#img-vp-cpuvsio){.reference .internal} how a CPU and I/O intensive application might use the CPU. For such tasks, if we can make sure that CPU intensive tasks don't block I/O intensive ones for too long, the system will enable the I/O intensive ones to better use the I/O devices while the CPU intensive task has only modest impact from the short periods of time that the I/O intensive ones use it. Also, if a user is interacting with the I/O intensive one, e.g. running emacs, the *Response Time* is less affected by the CPU intensive applications.

The *Round Robin* algorithm builds a simple FIFO run queue of tasks in the ready state much like the FIFO algorithm described earlier. When a task starts running it is given a fixed amount of time to run, often called a *Quantum* or *Time slice*. When the quantum expires the OS does a context switch to the next task in the queue and adds the previously running task at the back of the queue.

Let us consider a situation with three tasks shown in the table below:

::: pst-scrollable-table-container
  Task   Start    Runtime
  ------ -------- ---------
  A      0        6
  B      0.0001   2
  C      0.0002   1
:::

Assuming the units are in seconds, let us assume that the quantum is also (unrealistically) 1 second. In that case, a round robin scheduler will run tasks as shown in [[Fig. 10.6]{.std .std-numref}](#vp-sched-rr){.reference .internal} below:

![[Fig. 10.6 ]{.caption-number}[Round Robin scheduling, where every task executes for a quantum of time.]{.caption-text}[\#](#vp-sched-rr "Link to this image"){.headerlink}](../_images/RR.png)

The average turnaround time of this round robin schedule is [\\((3 + 5 + 9)/3 = 5.6\\)]{.math .notranslate .nohighlight}. We can see that it is terrible compared to SJF, but much better than the worst FIFO case.

The preemptive scheduling models introduces a new parameter we need to set: the length of the quantum. We have to weigh the cost of changing processes against the interactivity requirements when deciding on the length of a time we will run CPU intensive tasks. You want to pick a time large enough that you are **amortizing** the cost of a context switch; if you picked a time that was a few hundred computer cycles you would be spending most of your time context switching. On the other hand, if you it is too long, interactive tasks would get terrible response rate.

Let us assume that the quantum is, say 10msec, a number much larger than the time for a context switch but reasonable to not add much delay to tasks that interact with humans. Also, we will assume that we can ignore the context switching time. We can represent what happens is shown below:

![[Fig. 10.7 ]{.caption-number}[Round Robin scheduling, with a reasonable quantum.]{.caption-text}[\#](#vp-sched-rr2 "Link to this image"){.headerlink}](../_images/RR2.png)

For the first three seconds, all three tasks share the CPU. Assuming that each gets an equal share, C will have had a full second of compute time after three seconds and it will be done. From seconds 3-5 the CPU is shared by tasks A and B, where each get half of it. After 5 seconds, B will have had two full seconds of compute time, and A will have the CPU to itself from that point forward.

::: {#id2 .section}
### [10.2.3.1. ]{.section-number}Tradeoffs[\#](#id2 "Link to this heading"){.headerlink}

-   **Requirements:**

    -   requires no knowledge of task run time

-   **The Good:**

    -   Simplest preemptive algorithm, better for response time than any non-preemptive one

    -   Does better for non-CPU resource use than any non-preemptive algorithm

-   **The Bad:**

    -   Can still result in poor response time with many CPU intensive tasks

    -   Poor turnaround time

    -   Bad for batch since constant context switching, and real time since difficult to make any prediction on how long tasks will take
:::
:::
:::

::: prev-next-area
[](sch-goals.html "previous page"){.left-prev}

::: prev-next-info
previous

[10.1. ]{.section-number}Scheduling Goals
:::

[](sch-prio.html "next page"){.right-next}

::: prev-next-info
next

[10.3. ]{.section-number}Scheduling with Priorities
:::
:::
:::

::: {.bd-sidebar-secondary .bd-toc}
::: {.sidebar-secondary-items .sidebar-secondary__inner}
::: sidebar-secondary-item
::: {.page-toc .tocsection .onthispage}
Contents
:::

-   [10.2.1. First Come, First Served (FCFS)](#first-come-first-served-fcfs){.reference .internal .nav-link}
    -   [10.2.1.1. Tradeoffs](#tradeoffs){.reference .internal .nav-link}
-   [10.2.2. Shortest Job First (SJF)](#shortest-job-first-sjf){.reference .internal .nav-link}
    -   [10.2.2.1. Tradeoffs](#id1){.reference .internal .nav-link}
-   [10.2.3. Round Robin](#round-robin){.reference .internal .nav-link}
    -   [10.2.3.1. Tradeoffs](#id2){.reference .internal .nav-link}
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
