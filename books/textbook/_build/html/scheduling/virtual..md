---
docsearch:language: en
lang: en
title: 8. Virtualizing the CPU --- Introduction to Operating Systems
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
-   [8. Virtualizing the CPU](#){.current .reference .internal}
-   [9. The Thread: A Virtual CPU](threads.html){.reference .internal}
-   [10. Scheduling](scheduling.html){.reference .internal}
    []{.toctree-toggle role="presentation"}
    -   [10.1. Scheduling Goals](sch-goals.html){.reference .internal}
    -   [10.2. Simple Examples of Scheduling Policies](sch-simple.html){.reference .internal}
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

-   [[ ![JupyterHub logo](../_static/images/logo_jupyterhub.svg) ]{.btn__icon-container} [JupyterHub]{.btn__text-container}](https://jupyterhub-opf-jupyterhub.apps.smaug.na.operate-first.cloud/hub/user-redirect/git-pull?repo=https%3A//github.com/OpenOSOrg/openos&urlpath=lab/tree/openos/content/scheduling/virtual.ipynb&branch=main "Launch on JupyterHub"){.btn .btn-sm .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
:::

::: {.dropdown .dropdown-source-buttons}

-   [[ ]{.btn__icon-container} [Repository]{.btn__text-container}](https://github.com/OpenOSOrg/openos "Source repository"){.btn .btn-sm .btn-source-repository-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
-   [[ ]{.btn__icon-container} [Suggest edit]{.btn__text-container}](https://github.com/OpenOSOrg/openos/edit/main/content/scheduling/virtual.ipynb "Suggest edit"){.btn .btn-sm .btn-source-edit-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
-   [[ ]{.btn__icon-container} [Open issue]{.btn__text-container}](https://github.com/OpenOSOrg/openos/issues/new?title=Issue%20on%20page%20%2Fscheduling/virtual.html&body=Your%20issue%20content%20here. "Open an issue"){.btn .btn-sm .btn-source-issues-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
:::

::: {.dropdown .dropdown-download-buttons}

-   [[ ]{.btn__icon-container} [.ipynb]{.btn__text-container}](../_sources/scheduling/virtual.ipynb "Download source file"){.btn .btn-sm .btn-download-source-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
-   [ ]{.btn__icon-container} [.pdf]{.btn__text-container}
:::

[ ]{.btn__icon-container}
:::
:::
:::
:::
:::

::: {#jb-print-docs-body .onlyprint}
# Virtualizing the CPU

::: {#print-main-content}
::: {#jb-print-toc}
:::
:::
:::

::: {#searchbox}
:::

::: {#virtualizing-the-cpu .section .tex2jax_ignore .mathjax_ignore}
[]{#cont-vp-virt}

# [8. ]{.section-number}Virtualizing the CPU[\#](#virtualizing-the-cpu "Link to this heading"){.headerlink}

When we say "virtualizing" what we mean is actually adding a layer of indirection between the target (in this case the CPU) and the source (the process), enabling multiple processes to take turns using the same CPU; that is time multiplexing the CPU. In order to do this, we will need a way of pausing the execution of a process while another process runs and then resuming execution later without the process having to be aware of this pause, which means we need to capture all of the state that is relevant to a process in one or more data structures we can use to hold them when the process is not active. When the OS changes the active process on a CPU, we call this a **context switch**. To complete a context switch we need to save the CPU state for the process coming off the CPU and then load the state for the incoming process before allowing the CPU to execute the incoming process.

Definitions:

-   Process: A virtual computer

-   Thread: A virtual CPU, where a process has at least one and possibly many

-   Task: Term to refer to either process or thread

-   Context switching: Switching the processor from running one task to another, i.e., saving the processor registers used by the running task into its thread struc, and loading some other task's registers into the CPU.

-   Scheduling: Deciding which task to run.

-   Preemption: Stopping a task to run another one.

![[Fig. 8.1 ]{.caption-number}[For each process, a task structure contains information about each of the processes. All processes that are ready to run are on a queue]{.caption-text}[\#](#img-vp-proc "Link to this image"){.headerlink}](../_images/vp-osstruc.png){style="width: 60%;"}

We stated [[earlier]{.std .std-ref}](../intro/abstractions.html#cont-gs-abstractions-process){.reference .internal} (see [[Fig. 4.2]{.std .std-numref}](../intro/abstractions.html#img-intro-proc){.reference .internal}) the kernel maintains a table of all processes, indexed by the *process id*, or **pid**, to keep track of all the information about each process. For reasons that will soon make sense, rather than processes, we will refer here to the abstraction that the kernel runs on the processor as a **task**, although feel free to think about a task as being a process for the time being. As shown in [[Fig. 4.2]{.std .std-numref}](../intro/abstractions.html#img-intro-proc){.reference .internal}, the kernel maintains a data structures, we call here a `run queue`{.docutils .literal .notranslate} for scheduling the tasks on the CPU. On a single CPU (actually single core) system, only one task can run at a time, and the kernel is responsible for selecting the task to be run and switching between them.

For each task, the kernel maintains a pointer to the file descriptor table, the memory management data structures (i.e. the map described above) and information about execution state of the task. For example, [[Listing 8.1]{.std .std-numref}](#simple-task-struct){.reference .internal} shows a highly simplified version of the `task_struct`{.docutils .literal .notranslate} data structure used by Linux. The state field indicates if the task is currently running, is blocked for some reason, or is ready and waiting to be run. The thread structure is a place for the kernel to store all the processor registers whenever the task is not running.

::: {.margin .admonition .note}
Note

What else is there: There is much more state in the task structure including:

-   Process ID, User ID, Group ID

-   Priority/Scheduling parameters

-   Accounting information

-   Signal management functions

-   Working directory To see the actual data structure, you can use the online browser for the current linux code base, and search for `task_struct`{.docutils .literal .notranslate} at this [link](https://elixir.bootlin.com/linux/latest/source/include/linux/sched.h#L746){.reference .external}.
:::

::: {#simple-task-struct .literal-block-wrapper .docutils .container}
::: code-block-caption
[Listing 8.1 ]{.caption-number}[A highly simplified version of the Linux task struct from the kernel include file linux/sched.h]{.caption-text}[\#](#simple-task-struct "Link to this code"){.headerlink}
:::

::: {.highlight-c .notranslate}
::: highlight
     1struct task_struct {
     2  // the state of the task: running, blocked, runable
     3  unsigned int  __state;
     4
     5  // CPU-specific state of this task
     6  struct thread_struct            thread;
     7
     8  // a pointer to the memory management data structures
     9  struct mm_struct                *mm;
    10
    11  // Open file information 
    12  struct files_struct             *files;
    13}
:::
:::
:::

[[Fig. 8.2]{.std .std-numref}](#img-vp-states){.reference .internal} shows the three possible states for a task, with all the valid state transitions represented by arrows. A task in the Running state is one that is currently active on a CPU. Processes do many things other than just use the CPU, e.g., they read data from files, communicate with other processes, etc... For example, as I type this, the process is constantly blocked waiting for me to type characters. Some examples of blocking operations are: issuing a read from disk or from a network socket that does not have data ready, issuing a write to a pipe that has no more space to buffer data, trying to acquire certain kinds of resources that are already owned by another process or thread, etc.

![[Fig. 8.2 ]{.caption-number}[Task states]{.caption-text}[\#](#img-vp-states "Link to this image"){.headerlink}](../_images/ProcessLifecycle.png){style="width: 200pt;"}

In these situations, the process must wait for something external to happen before it can make progress (e.g., data arrives over the network, another process reads some data out of the pipe, the requested resource is released by another process, etc.), and is unable to make use of the CPU until that event occurs. We would be wasting the limited CPU resource if we left such a process on the CPU, and there is no point considering it among the set of runnable processes that we might want to choose next either. Tasks that are waiting for something go into the **Blocked** state, the kernel removes them from the run queue, saves all the processor registers into the thread structure, and then make a **scheduling** decision to select some other process to run from the run queue. The kernel changes the state of the selected task from **Ready** to **Running** and loads its registers from the task structures into the CPU registers.

The process of switching the CPU between two tasks is called a **Context Switch**. Context switches are expensive for two reasons. First, there is overhead to save the state (i.e., CPU registers) of the outgoing process, select the next process to run, and load the state of the incoming task. Second, even though we are saving all the state needed to resume a process, modern processors have several caches (e.g., data and instruction caches, the translation look aside buffer, etc.) that help an application run more quickly. As the application runs, these caches are filled with instructions or data that are related to the executing process. When a new task is placed on a CPU, the contents of these caches are no longer related to the running process, and either need to be cleared by the OS, or need to be replaced by the new process as it executes.

Once whatever causes the task to be blocked is resolved, the kernel changes the state of the task from **Blocked** to **Ready**, and places the task struct onto the run queue so it can be run the next time there is a scheduling decision to be made.

A task may also transition from the **Running** to the **Ready** state without going through the **Blocked** state. Some tasks may run for a really long time without doing any I/O. This can cause a problem for other tasks that are constantly blocking and doing get their fair share of the processor. To handle this, all systems have hardware timers, where the kernel can configure the timer to cause an interrupt at some future time. When the interrupt occurs, the kernel stops the current task, and makes a scheduling decision to context switch to some other task. This is called **Preemption**, where the kernel stops, or **Preempts** a task to run another one.
:::

::: prev-next-area
[](process.html "previous page"){.left-prev}

::: prev-next-info
previous

[7. ]{.section-number}The Process: A virtual Computer
:::

[](threads.html "next page"){.right-next}

::: prev-next-info
next

[9. ]{.section-number}The Thread: A Virtual CPU
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
