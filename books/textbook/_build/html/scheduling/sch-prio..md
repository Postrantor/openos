---
docsearch:language: en
lang: en
title: 10.3. Scheduling with Priorities --- Introduction to Operating Systems
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

- [Preface](../intro/pref.html){.reference .internal}

[Getting started]{.caption-text}

- [1. Introduction](../intro/intro.html){.reference .internal}
- [2. Purpose of operating systems](../intro/purpose.html){.reference .internal}
- [3. Operating System Structure & Unix/Linux](../intro/structure.html){.reference .internal}
- [4. Operating System Abstractions](../intro/abstractions.html){.reference .internal}
- [5. What you should know](../intro/tools.html){.reference .internal}
  []{.toctree-toggle role="presentation"}
  - [5.1. The C Programming Language](../intro/tools-c.html){.reference .internal}
  - [5.2. Shell](../intro/tools-shell.html){.reference .internal}
  - [5.3. Editors](../intro/tools-editors.html){.reference .internal}
  - [5.4. Make](../intro/tools-make.html){.reference .internal}
  - [5.5. Testing](../intro/tools-testing.html){.reference .internal}
  - [5.6. Git Basics](../intro/tools-git.html){.reference .internal}
  - [5.7. GDB](../intro/tools-gdb.html){.reference .internal}

[Virtual Processor]{.caption-text}

- [6. Introduction](intro.html){.reference .internal}
- [7. The Process: A virtual Computer](process.html){.reference .internal}
- [8. Virtualizing the CPU](virtual.html){.reference .internal}
- [9. The Thread: A Virtual CPU](threads.html){.reference .internal}
- [10. Scheduling](scheduling.html){.reference .internal}
  []{.toctree-toggle role="presentation"}
  - [10.1. Scheduling Goals](sch-goals.html){.reference .internal}
  - [10.2. Simple Examples of Scheduling Policies](sch-simple.html){.reference .internal}
  - [10.3. Scheduling with Priorities](#){.current .reference .internal}
  - [10.4. Scheduling in the real world](sch-real.html){.reference .internal}
- [11. Review Questions](review.html){.reference .internal}

[Virtual Memory]{.caption-text}

- [12. Introduction](../mm/intro.html){.reference .internal}
- [13. Memory management before paged virtual memory](../mm/phys-and-seg.html){.reference .internal}
- [14. Paged Virtual memory](../mm/pagvm.html){.reference .internal}
  []{.toctree-toggle role="presentation"}
  - [14.1. Abstracting a useful interface for memory management.](../mm/vmabs.html){.reference .internal}
  - [14.2. Paging](../mm/virt-paging.html){.reference .internal}
  - [14.3. Page Tables](../mm/page-tables.html){.reference .internal}
  - [14.4. Memory reclaiming algorithms.](../mm/reclamation.html){.reference .internal}
  - [14.5. Page Sizes](../mm/page-size.html){.reference .internal}
  - [14.6. Memory Management Page Faults](../mm/pagefaults.html){.reference .internal}
- [15. Buffer Cache](../mm/buffer-cache.html){.reference .internal}
- [16. Memory management in the real world](../mm/realworld.html){.reference .internal}
- [17. Conclusion](../mm/concl.html){.reference .internal}
- [18. Review](../mm/review.html){.reference .internal}

[File Systems]{.caption-text}

- [19. Introduction](../fs/intro.html){.reference .internal}
- [20. File System Abstraction](../fs/interface.html){.reference .internal}
- [21. A bit about Disks](../fs/diskhw.html){.reference .internal}
- [22. Implementation](../fs/impl.html){.reference .internal}
  []{.toctree-toggle role="presentation"}
  - [22.1. File System Layout](../fs/disklayout.html){.reference .internal}
  - [22.2. Disk Layout:Tracking Used Space](../fs/dl_track_used.html){.reference .internal}
  - [22.3. Disk Layout:Tracking Free Space](../fs/dl_track_free.html){.reference .internal}
  - [22.4. Disk Layout:Implementing Name Space](../fs/dl_name.html){.reference .internal}
  - [22.5. Disk Layout:Dealing with Failures](../fs/dl_failures.html){.reference .internal}
  - [22.6. Disk Layout:Examples of Real World File Systems](../fs/dl_ex_exx.html){.reference .internal}
  - [22.7. Kernel implementation](../fs/kernelimp.html){.reference .internal}
- [23. Review](../fs/review.html){.reference .internal}

[Concurrency]{.caption-text}

- [24. Introduction](../sync/sync.html){.reference .internal}
- [25. Basic Synchronization](../sync/basic.html){.reference .internal}
  []{.toctree-toggle role="presentation"}
  - [25.1. Cooperating Processes and Inter-process Communication](../sync/sharing.html){.reference .internal}
  - [25.2. The Critical Section Problem](../sync/criticalsection.html){.reference .internal}
  - [25.3. Implementing Locks](../sync/locks.html){.reference .internal}
  - [25.4. Ordering Thread Events](../sync/ordering.html){.reference .internal}
- [26. Common Concurrency Bugs](../sync/concurrency_bugs.html){.reference .internal}
- [27. Advanced Synchronization](../sync/advanced.html){.reference .internal}
  []{.toctree-toggle role="presentation"}
  - [27.1. Read-Dominated Workloads](../sync/readmostly.html){.reference .internal}
  - [27.2. Challenges of Modern Hardware](../sync/hardware_challenges.html){.reference .internal}
  - [27.3. Locking in the Linux Kernel](../sync/linux_locking.html){.reference .internal}
- [28. Review](../sync/review.html){.reference .internal}

[Other Topics]{.caption-text}

- [29. Input and Output](../devices/devices.html){.reference .internal}
- [30. More on Disks](../devices/disk2.html){.reference .internal}
- [31. Virtualization](../virt/virt.html){.reference .internal}
- [32. Security](../sec/sec.html){.reference .internal}

[Appendices]{.caption-text}

- [33. How to read this book](../misc/howto.html){.reference .internal}
- [34. Contributing](../contributing/intro.html){.reference .internal}
  []{.toctree-toggle role="presentation"}
  - [34.1. Examples](../contributing/examples.html){.reference .internal}
  - [34.2. Contributors](../contributing/credit.html){.reference .internal}
  - [34.3. Contributing](../contributing/Contributing.html){.reference .internal}
  - [34.6. Resources to look at](../contributing/resources.html){.reference .internal}
  - [34.7. Out of date](../contributing/fix.html){.reference .internal}
- [35. Bibliography](../misc/bib.html){.reference .internal}
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

- [[ ![JupyterHub logo](../_static/images/logo_jupyterhub.svg) ]{.btn__icon-container} [JupyterHub]{.btn__text-container}](https://jupyterhub-opf-jupyterhub.apps.smaug.na.operate-first.cloud/hub/user-redirect/git-pull?repo=https%3A//github.com/OpenOSOrg/openos&urlpath=lab/tree/openos/content/scheduling/sch-prio.ipynb&branch=main "Launch on JupyterHub"){.btn .btn-sm .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
  :::

::: {.dropdown .dropdown-source-buttons}

- [[ ]{.btn__icon-container} [Repository]{.btn__text-container}](https://github.com/OpenOSOrg/openos "Source repository"){.btn .btn-sm .btn-source-repository-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
- [[ ]{.btn__icon-container} [Suggest edit]{.btn__text-container}](https://github.com/OpenOSOrg/openos/edit/main/content/scheduling/sch-prio.ipynb "Suggest edit"){.btn .btn-sm .btn-source-edit-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
- [[ ]{.btn__icon-container} [Open issue]{.btn__text-container}](https://github.com/OpenOSOrg/openos/issues/new?title=Issue%20on%20page%20%2Fscheduling/sch-prio.html&body=Your%20issue%20content%20here. "Open an issue"){.btn .btn-sm .btn-source-issues-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
  :::

::: {.dropdown .dropdown-download-buttons}

- [[ ]{.btn__icon-container} [.ipynb]{.btn__text-container}](../_sources/scheduling/sch-prio.ipynb "Download source file"){.btn .btn-sm .btn-download-source-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}

-  [ ]{.btn__icon-container} [.pdf]{.btn__text-container}
  :::

[ ]{.btn__icon-container}

[]{.fa-solid .fa-list}
:::
:::
:::
:::
:::

::: {#jb-print-docs-body .onlyprint}

# Scheduling with Priorities

::: {#print-main-content}
::: {#jb-print-toc}

<div>

## Contents

</div>

- [10.3.1. Fixed Priority](#fixed-priority){.reference .internal .nav-link}
  - [10.3.1.1. Tradeoffs](#tradeoffs){.reference .internal .nav-link}
- [10.3.2. Variable Priority or Multilevel feedback](#variable-priority-or-multilevel-feedback){.reference .internal .nav-link}
  - [10.3.2.1. Tradeoffs](#id1){.reference .internal .nav-link}
    :::
    :::
    :::

::: {#searchbox}
:::

::: {#scheduling-with-priorities .section .tex2jax_ignore .mathjax_ignore}

# [10.3. ] {.section-number}Scheduling with Priorities[\#](#scheduling-with-priorities "Link to this heading") {.headerlink}

We first discuss scheduling with fixed priorites for real time, and then how priorities can be used dynamically to support an interactive system.

::: {#fixed-priority .section}

## [10.3.1. ] {.section-number}Fixed Priority[\#](#fixed-priority "Link to this heading") {.headerlink}

The core idea behind priority scheduling is that some processes may be more important than others and should be given access to the CPU first. For example, one reasonable assumption might be that tasks of students should only run if there are no tasks from professors. To implement this policy, the OS maintains two or more priority queues which hold tasks assigned to the corresponding priority. Runnable processes in a lower priority queue are only run if there are none in a higher priority queues. Figure [[Fig. 10.8]{.std .std-numref}](#priority-sched){.reference .internal} shows a simple example of a system with 4 priority queues. In this snapshot, the next process to be given CPU time will be the first process in the priority 4 queue. Assuming no additions, the processes in queue 3 will not run until all of the ones in 4 have completed.

![[Fig. 10.8 ]{.caption-number}[A simple example of a system with 5 priority queues and runnable processes in several of the queues.]{.caption-text}[\#](#priority-sched "Link to this image"){.headerlink}](../_images/Priority.png)

Let us consider a situation with three tasks shown in the table below:

::: pst-scrollable-table-container
Task   Start   Runtime   Priority

---

A      0       6         1
B      1       2         3
C      2       2         3
D      3       1         5
:::

In that case, a priority scheduler will run tasks as shown in [[Fig. 10.9]{.std .std-numref}](#vp-sched-pr){.reference .internal} below:

![[Fig. 10.9 ]{.caption-number}[Priority scheduling, where every task executes for a quantum of time.]{.caption-text}[\#](#vp-sched-pr "Link to this image"){.headerlink}](../_images/Priority-tl.png)

A runs by itself until B becomes ready to run. We then preempt A after it has accumulated one second of run time, and context switch to B since it is higher priority. When C starts running, it is the same priority as B, so they share the CPU (i.e., we switch back and forth between them every quantum). At time 3, D enters with the highest priority, and we stop running B and C to just run it. At that point, B has accumulated 1.5 sec of runtime, and C has accumulated .5 seconds. Once D is done, we again share the CPU using round robin between B and C, until B has accumulated its full 2 seconds of runtime, after which we can use the CPU just for running C. Finally, at second 6, all the other tasks are done and A, the lowest priority task, can be run until it completes. The average turnaround time here is [\\(((4-3) + (5-1) + (6-2) + 11)/4 = 5\\)]{.math .notranslate .nohighlight} seconds.

Note, one challenge with a fixed priority scheme is that low priority work can starve if there is always higher priority work entering the system.

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

A very popular scheduling algorithm for this is called **Multilevel** feedback. It assumes the same kind of data structure shown in [[Fig. 10.9]{.std .std-numref}](#vp-sched-pr){.reference .internal}. One simple varient of the algorithm is:

- When a task first starts running, we assume it is I/O intensive, and add it to the highest priority queue.
- if a task consumes an entire quantum, we assume it is more CPU intensive, and decrease its priority by one before adding it to the runqueue.
- If a task performs I/O before its quantum expires, when it becomes runnable we increase its priority (up to the highest level) before adding it to the runqueue.
- To avoid starvation, we periodically move all the tasks to the highest priority queue.

Note, a system can support both fixed priorities, e.g., for real time tasks, and a range of priorities for dealing with general purpose tasks.

::: {#id1 .section}

### [10.3.2.1. ] {.section-number}Tradeoffs[\#](#id1 "Link to this heading") {.headerlink}

- **Requirements:**

  - requires no knowledge of task run time
- **The Good:**

  - Good for interactive tasks and maintaining high utilization of non-cpu resources
- **The Bad:**

  - Bad for real time and batch
  - While it can deal with starvation by periodically moving tasks to high priority queue, this is a bit of a hack rather than an intrinsic part of the algorithm.
    :::
    :::
    :::

::: prev-next-area
[](sch-simple.html "previous page"){.left-prev}

::: prev-next-info
previous

[10.2. ]{.section-number}Simple Examples of Scheduling Policies
:::

[](sch-real.html "next page"){.right-next}

::: prev-next-info
next

[10.4. ]{.section-number}Scheduling in the real world
:::
:::
:::

::: {.bd-sidebar-secondary .bd-toc}
::: {.sidebar-secondary-items .sidebar-secondary__inner}
::: sidebar-secondary-item
::: {.page-toc .tocsection .onthispage}
Contents
:::

- [10.3.1. Fixed Priority](#fixed-priority){.reference .internal .nav-link}
  - [10.3.1.1. Tradeoffs](#tradeoffs){.reference .internal .nav-link}
- [10.3.2. Variable Priority or Multilevel feedback](#variable-priority-or-multilevel-feedback){.reference .internal .nav-link}
  - [10.3.2.1. Tradeoffs](#id1){.reference .internal .nav-link}
    :::
    :::
    :::
    :::

::: {.bd-footer-content__inner .container}
::: footer-item
By (see contributing chapter book)
:::

::: footer-item
© Copyright 2022.
:::

::: footer-item
:::

::: footer-item
:::
:::
:::
:::
:::
