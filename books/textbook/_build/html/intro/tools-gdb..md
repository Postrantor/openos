---
docsearch:language: en
lang: en
title: 5.7. GDB --- Introduction to Operating Systems
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
[![Introduction to Operating Systems - Home](../_static/logo.png){.logo__image .only-light}](pref.html){.navbar-brand .logo}
:::

::: sidebar-primary-item
:::

::: sidebar-primary-item
::: {.bd-toc-item .navbar-nav .active}
-   [Preface](pref.html){.reference .internal}

[Getting started]{.caption-text}

-   [1. Introduction](intro.html){.reference .internal}
-   [2. Purpose of operating systems](purpose.html){.reference .internal}
-   [3. Operating System Structure & Unix/Linux](structure.html){.reference .internal}
-   [4. Operating System Abstractions](abstractions.html){.reference .internal}
-   [5. What you should know](tools.html){.reference .internal}
    []{.toctree-toggle role="presentation"}
    -   [5.1. The C Programming Language](tools-c.html){.reference .internal}
    -   [5.2. Shell](tools-shell.html){.reference .internal}
    -   [5.3. Editors](tools-editors.html){.reference .internal}
    -   [5.4. Make](tools-make.html){.reference .internal}
    -   [5.5. Testing](tools-testing.html){.reference .internal}
    -   [5.6. Git Basics](tools-git.html){.reference .internal}
    -   [5.7. GDB](#){.current .reference .internal}

[Virtual Processor]{.caption-text}

-   [6. Introduction](../scheduling/intro.html){.reference .internal}
-   [7. The Process: A virtual Computer](../scheduling/process.html){.reference .internal}
-   [8. Virtualizing the CPU](../scheduling/virtual.html){.reference .internal}
-   [9. The Thread: A Virtual CPU](../scheduling/threads.html){.reference .internal}
-   [10. Scheduling](../scheduling/scheduling.html){.reference .internal}
    []{.toctree-toggle role="presentation"}
    -   [10.1. Scheduling Goals](../scheduling/sch-goals.html){.reference .internal}
    -   [10.2. Simple Examples of Scheduling Policies](../scheduling/sch-simple.html){.reference .internal}
    -   [10.3. Scheduling with Priorities](../scheduling/sch-prio.html){.reference .internal}
    -   [10.4. Scheduling in the real world](../scheduling/sch-real.html){.reference .internal}
-   [11. Review Questions](../scheduling/review.html){.reference .internal}

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

-   [[ ![JupyterHub logo](../_static/images/logo_jupyterhub.svg) ]{.btn__icon-container} [JupyterHub]{.btn__text-container}](https://jupyterhub-opf-jupyterhub.apps.smaug.na.operate-first.cloud/hub/user-redirect/git-pull?repo=https%3A//github.com/OpenOSOrg/openos&urlpath=lab/tree/openos/content/intro/tools-gdb.ipynb&branch=main "Launch on JupyterHub"){.btn .btn-sm .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
:::

::: {.dropdown .dropdown-source-buttons}

-   [[ ]{.btn__icon-container} [Repository]{.btn__text-container}](https://github.com/OpenOSOrg/openos "Source repository"){.btn .btn-sm .btn-source-repository-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
-   [[ ]{.btn__icon-container} [Suggest edit]{.btn__text-container}](https://github.com/OpenOSOrg/openos/edit/main/content/intro/tools-gdb.ipynb "Suggest edit"){.btn .btn-sm .btn-source-edit-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
-   [[ ]{.btn__icon-container} [Open issue]{.btn__text-container}](https://github.com/OpenOSOrg/openos/issues/new?title=Issue%20on%20page%20%2Fintro/tools-gdb.html&body=Your%20issue%20content%20here. "Open an issue"){.btn .btn-sm .btn-source-issues-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
:::

::: {.dropdown .dropdown-download-buttons}

-   [[ ]{.btn__icon-container} [.ipynb]{.btn__text-container}](../_sources/intro/tools-gdb.ipynb "Download source file"){.btn .btn-sm .btn-download-source-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
-   [ ]{.btn__icon-container} [.pdf]{.btn__text-container}
:::

[ ]{.btn__icon-container}
:::
:::
:::
:::
:::

::: {#jb-print-docs-body .onlyprint}
# GDB

::: {#print-main-content}
::: {#jb-print-toc}
:::
:::
:::

::: {#searchbox}
:::

::: {#gdb .section .tex2jax_ignore .mathjax_ignore}
[]{#cont-gs-tools-gdb}

# [5.7. ]{.section-number}GDB[\#](#gdb "Link to this heading"){.headerlink}

Until now, many of you have been able to get by debugging your programs using print statements. Don't even try to that with this course; you will not be successful. In the container image available with this course, we provide you with the very powerful GNU Debugger gdb, with documentation available [here](https://sourceware.org/gdb/current/onlinedocs/gdb.html/){.reference .external}. As discussed previously, you should always run it from [[emacs]{.std .std-ref}](tools-editors.html#cont-gs-tools-editors){.reference .internal}, but if you want to run gdb from the command line, type `gdb <program>`{.docutils .literal .notranslate} to debug the executable program, and then `run`{.docutils .literal .notranslate} to run it. Some of the key features you will find critical in this course are:

-   Setting [breakpoints](https://sourceware.org/gdb/current/onlinedocs/gdb.html/Breakpoints.html#Breakpoints){.reference .external} at specific lines in your source code where you want to see the state. For example:

    -   `break <function>`{.docutils .literal .notranslate}: sets a breakpoint at the beginning of `function`{.docutils .literal .notranslate}.

    -   `break <filename>:<linenumber>`{.docutils .literal .notranslate}: sets the breakpoint to the given line number in the source file.

    -   to delete a breakpoint, type `delete #`{.docutils .literal .notranslate} where to find out what number each breakpoint is, type `info breakpoints`{.docutils .literal .notranslate}

    -   you can then type `c`{.docutils .literal .notranslate} to continue, `n`{.docutils .literal .notranslate} to go to the next line (stepping over functions), `s`{.docutils .literal .notranslate} to step into a function, or `si`{.docutils .literal .notranslate} to step by a single machine instructions (critical with some of the programs you will write here).

-   Displaying the state of your program, e.g.:

    -   `print <variable>`{.docutils .literal .notranslate} will print the value of a variable, or \`display will print each every time you step ahead.

    -   `info registers`{.docutils .literal .notranslate} will show you the state in all the registers of the computer; and `info regis XXX`{.docutils .literal .notranslate} will show you the state of a particular register, e.g., `rsp`{.docutils .literal .notranslate} for the stack pointer

    -   `x/FMT`{.docutils .literal .notranslate} will examine the state of memory, e.g., `x/10gx <address>`{.docutils .literal .notranslate} will show you 10 values of giant (64 bit) values in hexidecimal

    -   `info threads`{.docutils .literal .notranslate} will tell you about all the threads in your program.

-   Debugging multiple processes; something you will need for implementing a shell

    -   `set follow-fork-mode <option>`{.docutils .literal .notranslate}: e.g., **set follow-fork-mode child** to debug child instead of parent

    -   `detach-on-fork <option>`{.docutils .literal .notranslate}: e.g. **set detach-on-fork off** to debug all the processes (you are debugging one at a time, and child is blocked right after fork)

    -   `info inferiors`{.docutils .literal .notranslate}: list all inferiors being managed

    -   `inferior <inferior_id>`{.docutils .literal .notranslate}: selects which inferior to switch to

-   Debugging threads of execution in your program

    -   `info threads`{.docutils .literal .notranslate}: lists all existing threads.

    -   `thread <thread_id>`{.docutils .literal .notranslate}: selects which thread to switch to.

    -   `set scheduler-locking mode`{.docutils .literal .notranslate}: if set to on will debug one thread at a time

-   Debugging signals

    -   `info signals`{.docutils .literal .notranslate} or `info signals <signal>`{.docutils .literal .notranslate}: lists all signals (or one signal) and shows how gdb responds to it.

    -   `handle <signal> <keyword>`{.docutils .literal .notranslate}: changes how gdb responds to that signal based on the keyword.

        -   `nostop`{.docutils .literal .notranslate}: gdb should not stop your program when this signal happens.

        -   `stop`{.docutils .literal .notranslate}: gdb should stop your program when this signal happens.

        -   `print`{.docutils .literal .notranslate}: gdb should print a message when this signal happens.

        -   `noprint`{.docutils .literal .notranslate}: gdb should not mention the occurrence of the signal at all.

        -   `ignore`{.docutils .literal .notranslate}: gdb should not allow your program to see this signal.

        -   `noignore`{.docutils .literal .notranslate}: gdb should allow your program to see this signal.

Note, all of the above functionality can be done from within emacs. Occassionally it is valuable to run gdb on the command line using the [text user interface](https://developer.apple.com/library/archive/documentation/DeveloperTools/gdb/gdb/gdb_23.html){.reference .external}. When you run gdb, type Xa to go into tui mode, and then X2 to switch between displays, e.g., to see assembly, all the registers...
:::

::: prev-next-area
[](tools-git.html "previous page"){.left-prev}

::: prev-next-info
previous

[5.6. ]{.section-number}Git Basics
:::

[](../scheduling/intro.html "next page"){.right-next}

::: prev-next-info
next

[6. ]{.section-number}Introduction
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
