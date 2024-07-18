---
docsearch:language: en
lang: en
title: 10.4. Scheduling in the real world --- Introduction to Operating Systems
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
  - [10.3. Scheduling with Priorities](sch-prio.html){.reference .internal}
  - [10.4. Scheduling in the real world](#){.current .reference .internal}
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

- [[ ![JupyterHub logo](../_static/images/logo_jupyterhub.svg) ]{.btn__icon-container} [JupyterHub]{.btn__text-container}](https://jupyterhub-opf-jupyterhub.apps.smaug.na.operate-first.cloud/hub/user-redirect/git-pull?repo=https%3A//github.com/OpenOSOrg/openos&urlpath=lab/tree/openos/content/scheduling/sch-real.ipynb&branch=main "Launch on JupyterHub"){.btn .btn-sm .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
  :::

::: {.dropdown .dropdown-source-buttons}

- [[ ]{.btn__icon-container} [Repository]{.btn__text-container}](https://github.com/OpenOSOrg/openos "Source repository"){.btn .btn-sm .btn-source-repository-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
- [[ ]{.btn__icon-container} [Suggest edit]{.btn__text-container}](https://github.com/OpenOSOrg/openos/edit/main/content/scheduling/sch-real.ipynb "Suggest edit"){.btn .btn-sm .btn-source-edit-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
- [[ ]{.btn__icon-container} [Open issue]{.btn__text-container}](https://github.com/OpenOSOrg/openos/issues/new?title=Issue%20on%20page%20%2Fscheduling/sch-real.html&body=Your%20issue%20content%20here. "Open an issue"){.btn .btn-sm .btn-source-issues-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
  :::

::: {.dropdown .dropdown-download-buttons}

- [[ ]{.btn__icon-container} [.ipynb]{.btn__text-container}](../_sources/scheduling/sch-real.ipynb "Download source file"){.btn .btn-sm .btn-download-source-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}

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

# Scheduling in the real world

::: {#print-main-content}
::: {#jb-print-toc}

<div>

## Contents

</div>

- [10.4.1. Multi-CPU scheduling](#multi-cpu-scheduling){.reference .internal .nav-link}
- [10.4.2. Scheduling in Linux](#scheduling-in-linux){.reference .internal .nav-link}
  :::
  :::
  :::

::: {#searchbox}
:::

::: {#scheduling-in-the-real-world .section .tex2jax_ignore .mathjax_ignore}

# [10.4. ] {.section-number}Scheduling in the real world[\#](#scheduling-in-the-real-world "Link to this heading") {.headerlink}

We briefly review some of the real world scheduling issues and approaches from a Linux perspective.

::: {#multi-cpu-scheduling .section}

## [10.4.1. ] {.section-number}Multi-CPU scheduling[\#](#multi-cpu-scheduling "Link to this heading") {.headerlink}

Today almost all systems have multiple CPUs. Early multi-CPU systems looked something like [[Fig. 10.10]{.std .std-numref}](#smp-hw){.reference .internal} below. If you compare with the simple computer picture we showed in the past ([[Fig. 2.1]{.std .std-numref}](../intro/purpose.html#simplecomputer-fig){.reference .internal}), there are just a modest number of CPUs accessing both the memory and I/O buses.

![[Fig. 10.10 ]{.caption-number}[Early multiprocessors]{.caption-text}[\#](#smp-hw "Link to this image"){.headerlink}](../_images/SMP.png){style="width: 50%;"}

The easiest solution, and the one first adopted by most operating systems to support these computers, was to have a single runqueue in the kernel. This is both simple, and fair, since whatever algorithm you apply for scheduling selects the best task to run irrespective of which CPU becomes available.

Unfortunately, today's systems look more like [[Fig. 10.11]{.std .std-numref}](#numa-hw){.reference .internal}. They have memory controllers and I/O controllers in *sockets*, which is really just a processor chip. The sockets have a large number of CPUs (or cores) each with their own caches, and a shared cache per socket. Memory is directly attached to one of the sockets, and all accesses from other sockets have to go through it; leading to Non-Uniform Memory Access (NUMA).

![[Fig. 10.11 ]{.caption-number}[Todays Multiprocessors]{.caption-text}[\#](#numa-hw "Link to this image"){.headerlink}](../_images/NUMA.png){style="width: 50%;"}

In today's systems a shared runqueue results in terrible performance. First, if you have hundreds of cores, the run queue itself becomes a bottleneck since only one CPU at a time can add or remove tasks from the queue. Second, with today's large caches, you often want to run a task on the same CPU it ran on recently to reduce cache misses. Third, modern systems are NUMA, or Non Unform Memory Access (NUMA), and you want to run a task on a CPU near the memory allocated to it.

Most systems have a seperate run queue per CPU, and use some algorithm to shift tasks from one CPU to another if the imbalance between the CPUs becomes too large. The simplest algorithm, called take, has any CPU that becomes idle look at the load on the other CPUs to try to steal work. You can see [here](https://elixir.bootlin.com/linux/latest/source/kernel/sched/fair.c#L11206){.reference .external} the current code in Linux for the load_balancer that is called whenever a runqueue is empty and periodically to re-balance work across the runqueus.
:::

::: {#scheduling-in-linux .section}

## [10.4.2. ] {.section-number}Scheduling in Linux[\#](#scheduling-in-linux "Link to this heading") {.headerlink}

Given the enormous number of platforms Linux runs on, that covers everything from Batch scheduling HPC systems, to desktops, to embedded real time, the scheduling system has had to become incredibly adaptable. You can find out a huge amount about it from the man page:

::: {.cell .tag_output_scroll .tag_remove-input .docutils .container}
::: {.cell_output .docutils .container}
:::
:::

Several snippets we would like to draw your attention to that relate strongly to the materials we have presented:

- Processes scheduled under one of the real-time policies (SCHED_FIFO, SCHED_RR) have a sched_priority value in the range 1 (low) to 99 (high). (As the numbers imply, real-time threads always have higher priority than normal threads.) Conceptually, the scheduler maintains a list of runnable threads for each possible sched_priority value. In order to determine which thread runs next, the scheduler looks for the non empty list with the highest static priority and selects the thread at the head of this list.
- All scheduling is preemptive: if a thread with a higher static priority becomes ready to run, the currently running thread will be preempted and returned to the wait list for its static priority level. The scheduling policy determines the ordering only within the list of runnable threads with equal static priority.
- Linux supports a number of policies that might sound familiar that can be specified on a per-task basis:

  - SCHED_FIFO: tasks will immediately preempt any currently running SCHED_OTHER, SCHED_BATCH, or SCHED_IDLE thread. SCHED_FIFO is a simple scheduling algorithm without time slicing.
  - SCHED_RR: Round-robin scheduling - incorporates a quantum.
  - SCHED_DEADLINE: Sporadic task model deadline scheduling; period real time tasks, where user specifies the period, expected Runtime, and Deadline
  - SCHED_OTHER (or SCHED_NORMAL): Default Linux time-sharing scheduling the standard Linux time-sharing scheduler that is intended for all threads that do not require the special real-time mechanisms. One can use **nice** to specify, depending on the schedular, the relative importance of different tasks.
  - SCHED_BATCH: This policy will cause the scheduler to always assume that the thread is CPU-intensive.
  - SCHED_IDLE: This policy is used for running jobs at extremely low priority.

Only privaledged tasks can set static prioritis; appropriate for single user systems where someone can specify the absolute priority of different work. The RLIMIT_RTTIME resource limit to set a ceiling on the CPU time that a real-time process may consume in order to gaurantee that real time tasks cannot cause starvation.

Prior to kernel version 2.6.23, the normal scheduler for Linux combined priority queues with a heuristic that altered a process's priority based on the amount of a time slice it used. CPU-bound processes would consume their entire slice and would drop in priority. Conversely, I/O-bound processes would often block before consuming an entire time slice and so their priority would be increased. This was meant to allow for interactive processes to stay in the high priority queues and batch processing jobs (really anything that was CPU-bound) to drop. This scheduler had a number of heuristics that were used in decision making that were also exposed as tunable parameters, but the biggest feature it boasted was that it had O(1) run time. In other words, the time to select the next process was constant, regardless of how many runnable processes there were in the system. This is basically a varient of the [[MLF]{.std .std-ref}](sch-prio.html#cont-scheduling-scheduling-policies-mlf){.reference .internal} we have discussed.

The completely fair scheduler was a from-scratch redesign of the Linux scheduler; it did away with priority queues and with all[[\[]{.fn-bracket}1[\]]{.fn-bracket}](#notall){#id1 .footnote-reference .brackets role="doc-noteref"} heuristics and tunables found in the O(1) scheduler. CFS introduced keeping a counter for the amount of runtime each task has received and this counter is used to decide on the next task to run. Instead of priority queues CFS places all tasks in a red-black tree sorted on their accumulated runtime with tasks on the left having less accumulated run time than tasks on the right. When the system needs a new task to run, the left most task is selected. This change allows CFS to completely avoid the starvation of CPU bound tasks that could occur with the previous scheduler.

---

[[\[]{.fn-bracket}[1](#id1){role="doc-backlink"}[\]]{.fn-bracket}]{.label}

CFS still has a single tunable than can be exposed, but the kernel must be configured with `SCHED_DEBUG`{.docutils .literal .notranslate} selected.
:::
:::

::: prev-next-area
[](sch-prio.html "previous page"){.left-prev}

::: prev-next-info
previous

[10.3. ]{.section-number}Scheduling with Priorities
:::

[](review.html "next page"){.right-next}

::: prev-next-info
next

[11. ]{.section-number}Review Questions
:::
:::
:::

::: {.bd-sidebar-secondary .bd-toc}
::: {.sidebar-secondary-items .sidebar-secondary__inner}
::: sidebar-secondary-item
::: {.page-toc .tocsection .onthispage}
Contents
:::

- [10.4.1. Multi-CPU scheduling](#multi-cpu-scheduling){.reference .internal .nav-link}
- [10.4.2. Scheduling in Linux](#scheduling-in-linux){.reference .internal .nav-link}
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
