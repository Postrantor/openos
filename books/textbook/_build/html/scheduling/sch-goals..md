---
docsearch:language: en
lang: en
title: 10.1. Scheduling Goals --- Introduction to Operating Systems
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
  - [10.1. Scheduling Goals](#){.current .reference .internal}
  - [10.2. Simple Examples of Scheduling Policies](sch-simple.html){.reference .internal}
  - [10.3. Scheduling with Priorities](sch-prio.html){.reference .internal}
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

- [[ ![JupyterHub logo](../_static/images/logo_jupyterhub.svg) ]{.btn__icon-container} [JupyterHub]{.btn__text-container}](https://jupyterhub-opf-jupyterhub.apps.smaug.na.operate-first.cloud/hub/user-redirect/git-pull?repo=https%3A//github.com/OpenOSOrg/openos&urlpath=lab/tree/openos/content/scheduling/sch-goals.ipynb&branch=main "Launch on JupyterHub"){.btn .btn-sm .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
  :::

::: {.dropdown .dropdown-source-buttons}

- [[ ]{.btn__icon-container} [Repository]{.btn__text-container}](https://github.com/OpenOSOrg/openos "Source repository"){.btn .btn-sm .btn-source-repository-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
- [[ ]{.btn__icon-container} [Suggest edit]{.btn__text-container}](https://github.com/OpenOSOrg/openos/edit/main/content/scheduling/sch-goals.ipynb "Suggest edit"){.btn .btn-sm .btn-source-edit-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
- [[ ]{.btn__icon-container} [Open issue]{.btn__text-container}](https://github.com/OpenOSOrg/openos/issues/new?title=Issue%20on%20page%20%2Fscheduling/sch-goals.html&body=Your%20issue%20content%20here. "Open an issue"){.btn .btn-sm .btn-source-issues-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
  :::

::: {.dropdown .dropdown-download-buttons}

- [[ ]{.btn__icon-container} [.ipynb]{.btn__text-container}](../_sources/scheduling/sch-goals.ipynb "Download source file"){.btn .btn-sm .btn-download-source-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}

-  [ ]{.btn__icon-container} [.pdf]{.btn__text-container}
  :::

[ ]{.btn__icon-container}
:::
:::
:::
:::
:::

::: {#jb-print-docs-body .onlyprint}

# Scheduling Goals

::: {#print-main-content}
::: {#jb-print-toc}
:::
:::
:::

::: {#searchbox}
:::

::: {#scheduling-goals .section .tex2jax_ignore .mathjax_ignore}
[]{#cont-scheduling-scheduling-goals}

# [10.1. ] {.section-number}Scheduling Goals[\#](#scheduling-goals "Link to this heading") {.headerlink}

We need to make a scheduling decision whenever a task completes (process or thread exits) or if the task blocks, for example doing I/O. We can make a scheduling decision when a new task is created (i.e., we could choose to switch to the child) when an I/O interrupt occurs that might unblock a task, or if a task has been running for a long time (i.e., the kernel schedules a timer interrupt to preempt the currently running task)

It seems fair to just take turns between different tasks. To understand why scheduling is more complicated, consider [[Fig. 10.1]{.std .std-numref}](#img-vp-cpuvsio){.reference .internal} which shows how two hypothetical tasks would use the CPU if they where running by themselves. One of the tasks is CPU intensive, using the processor for long periods of time, while the other task spends most of its time blocked on I/O. If we just took turns running the different tasks, as soon as task 2 blocks for the first time, task 2 would get the CPU for a long time. Not only is task 2 not getting its fair share of the CPU, but if task 2 was using a disk we are wasting the resources of our computer since if task 2 could get just a little bit of CPU it would be using the disk while task 1 was using the CPU. Also, if task 2 was, for example, running emacs, every time the user typed a key emacs take a long time to respond since it wouldn't get run again until task 1, which is perhaps spending hours on bitcoin mining, stopped running.

![[Fig. 10.1 ]{.caption-number}[Figure shows how two tasks would use the CPU if they where running by themselves. Task 1 is a CPU intensive, wanting to use the CPU for long periods of time, while Task 2 is IO intensive, blocking frequently to interact with some I/O device.]{.caption-text}[\#](#img-vp-cpuvsio "Link to this image"){.headerlink}](../_images/cpuvsio.png){style="width: 80%;"}

Scheduling policies may aim for different goals, for example, a system may try to give all tasks an equal share of the CPU. They may also try to implement some kind of policy, for example, students should only get to use the CPU whenever professors don't need it. Or, they might try to maximize the number of tasks that complete per unit time, or minimize how long tasks take on average. They can also try to schedule the CPU in such a fashion to maximize the utilization of all the resources of the computer; e.g., run I/O intensive tasks whenever they are not blocked so they will keep the I/O devices busy. On the other hand, as we have discussed, context switching can be expensive, so if you are constantly preempting the running process you are wasting many resources. This is all complicated by the fact that the system may not know how long tasks will take, if they are I/O or CPU intensive, etc... Perhaps you can understand why researchers have published thousands and thousands of papers on different scheduling polices over the years. To make things worse, while we are focused here on scheduling the CPU, as we will see later, to achieve any goal one needs to also schedule memory and even the disk head; achieving an end-to-end goal for a

Applications and/or systems can care about:

- **Turnaround time**: The time from when a task entered the system until it was done.
- **Throughput**: The rate that tasks complete at.
- **Response time**: How long does it take for an application to respond to external events.
- **Fairness**: How fairly are the resources of the computer shared between the tasks, e.g., if we have two tasks do they both get equal shares of the CPU.
- **Predictability**: The guarantees on run time that a task can get.
- **Starvation**: Is it possible for some tasks to never run when the demand on the system is high.

These requirements are often in tension with each other and designing a scheduling algorithm is an act of balancing trade offs for the requirements of the OS.

We should note that these metrics are generally not just about the scheduling, for example, response time depends not just on how long after a resource is available does the scheduler take to context switch to the right task, but also how long that task takes to execute once it is scheduled to respond to the request. Also, the time the task takes depends not only on its processing requirements, but also how much of its state is in the CPU caches, if any of its state needs to be brought in from disk, etc... its complicated.

With cloud computing, we have switched from caring about average response time, to tail latency. In the cloud, a request may hit hundreds of computers, and we care about [\\(99.9\\%\\)]{.math .notranslate .nohighlight} tail latency, i.e., the response time for all but [\\(0.1%\\)]{.math .notranslate .nohighlight} of the requests, since if even [\\(1\\%\\)]{.math .notranslate .nohighlight} of the requests hit a slow computer the aggregate request will be slow. While it would be nice if one could guarantee the latency of [\\(100\\%\\)]{.math .notranslate .nohighlight} of the requests, that is likely too expensive.

General purpose systems typically have limited information about the real needs of the applications, and implement complex schedulers that try to do a good job of tradeing off between different goals we have discussed above. However a great deal of attention in scheduling has been spent on special purpose systems where more information is available, including:

- **Real time**: Real time systems are used in a wide class of applications from industrial controls to vehicle management to robotics. Predictability is a key requirement in each of these cases. Think of the program or programs responsible for managing an airplane in flight. The developers make decisions for the software with a guarantee that certain calculations can be made at least N times a second. If this requirement is not met, we start seeing bad and possibly dangerous behavior. Such systems typically require users to specify how long tasks will take and the relative priority of different tasks so that the system can preempting lower priority work whenever a high priority task becomes available.
- **Batch**: These are systems where the user submits jobs without any further interaction until the job completes. Early mainframes where all based on batch processing, where users submitted jobs with punch cards. Today, most high performance computing systems, where jobs consume enormous resources and run for long periods of time, use batch processing to enable the very expensive resources of the computer to be used efficiently. These systems typically run tasks to completion to avoid any overhead of preemption and require users to specify how long tasks will run so they can schedule all the required resources.

While general purpose operating systems cannot achieve the efficiency or predictability of specialized systems, they do need to support some applications with different requirements. As we will see, they provide mechanisms, such as priority, to provide some control over the scheduling of applications. While historically large HPC machines and embedded devices relied on special purpose systems, today specialized configurations of Linux has captured more and more of the requirements of these systems.
:::

::: prev-next-area
[](scheduling.html "previous page"){.left-prev}

::: prev-next-info
previous

[10. ]{.section-number}Scheduling
:::

[](sch-simple.html "next page"){.right-next}

::: prev-next-info
next

[10.2. ]{.section-number}Simple Examples of Scheduling Policies
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
