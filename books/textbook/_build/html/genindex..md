---
docsearch:language: en
lang: en
title: Index --- Introduction to Operating Systems
viewport:
- width=device-width, initial-scale=1.0
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
[![Introduction to Operating Systems - Home](_static/logo.png){.logo__image .only-light}](intro/pref.html){.navbar-brand .logo}
:::

::: sidebar-primary-item
:::

::: sidebar-primary-item
::: {.bd-toc-item .navbar-nav .active}
-   [Preface](intro/pref.html){.reference .internal}

[Getting started]{.caption-text}

-   [1. Introduction](intro/intro.html){.reference .internal}
-   [2. Purpose of operating systems](intro/purpose.html){.reference .internal}
-   [3. Operating System Structure & Unix/Linux](intro/structure.html){.reference .internal}
-   [4. Operating System Abstractions](intro/abstractions.html){.reference .internal}
-   [5. What you should know](intro/tools.html){.reference .internal}
    []{.toctree-toggle role="presentation"}
    -   [5.1. The C Programming Language](intro/tools-c.html){.reference .internal}
    -   [5.2. Shell](intro/tools-shell.html){.reference .internal}
    -   [5.3. Editors](intro/tools-editors.html){.reference .internal}
    -   [5.4. Make](intro/tools-make.html){.reference .internal}
    -   [5.5. Testing](intro/tools-testing.html){.reference .internal}
    -   [5.6. Git Basics](intro/tools-git.html){.reference .internal}
    -   [5.7. GDB](intro/tools-gdb.html){.reference .internal}

[Virtual Processor]{.caption-text}

-   [6. Introduction](scheduling/intro.html){.reference .internal}
-   [7. The Process: A virtual Computer](scheduling/process.html){.reference .internal}
-   [8. Virtualizing the CPU](scheduling/virtual.html){.reference .internal}
-   [9. The Thread: A Virtual CPU](scheduling/threads.html){.reference .internal}
-   [10. Scheduling](scheduling/scheduling.html){.reference .internal}
    []{.toctree-toggle role="presentation"}
    -   [10.1. Scheduling Goals](scheduling/sch-goals.html){.reference .internal}
    -   [10.2. Simple Examples of Scheduling Policies](scheduling/sch-simple.html){.reference .internal}
    -   [10.3. Scheduling with Priorities](scheduling/sch-prio.html){.reference .internal}
    -   [10.4. Scheduling in the real world](scheduling/sch-real.html){.reference .internal}
-   [11. Review Questions](scheduling/review.html){.reference .internal}

[Virtual Memory]{.caption-text}

-   [12. Introduction](mm/intro.html){.reference .internal}
-   [13. Memory management before paged virtual memory](mm/phys-and-seg.html){.reference .internal}
-   [14. Paged Virtual memory](mm/pagvm.html){.reference .internal}
    []{.toctree-toggle role="presentation"}
    -   [14.1. Abstracting a useful interface for memory management.](mm/vmabs.html){.reference .internal}
    -   [14.2. Paging](mm/virt-paging.html){.reference .internal}
    -   [14.3. Page Tables](mm/page-tables.html){.reference .internal}
    -   [14.4. Memory reclaiming algorithms.](mm/reclamation.html){.reference .internal}
    -   [14.5. Page Sizes](mm/page-size.html){.reference .internal}
    -   [14.6. Memory Management Page Faults](mm/pagefaults.html){.reference .internal}
-   [15. Buffer Cache](mm/buffer-cache.html){.reference .internal}
-   [16. Memory management in the real world](mm/realworld.html){.reference .internal}
-   [17. Conclusion](mm/concl.html){.reference .internal}
-   [18. Review](mm/review.html){.reference .internal}

[File Systems]{.caption-text}

-   [19. Introduction](fs/intro.html){.reference .internal}
-   [20. File System Abstraction](fs/interface.html){.reference .internal}
-   [21. A bit about Disks](fs/diskhw.html){.reference .internal}
-   [22. Implementation](fs/impl.html){.reference .internal}
    []{.toctree-toggle role="presentation"}
    -   [22.1. File System Layout](fs/disklayout.html){.reference .internal}
    -   [22.2. Disk Layout:Tracking Used Space](fs/dl_track_used.html){.reference .internal}
    -   [22.3. Disk Layout:Tracking Free Space](fs/dl_track_free.html){.reference .internal}
    -   [22.4. Disk Layout:Implementing Name Space](fs/dl_name.html){.reference .internal}
    -   [22.5. Disk Layout:Dealing with Failures](fs/dl_failures.html){.reference .internal}
    -   [22.6. Disk Layout:Examples of Real World File Systems](fs/dl_ex_exx.html){.reference .internal}
    -   [22.7. Kernel implementation](fs/kernelimp.html){.reference .internal}
-   [23. Review](fs/review.html){.reference .internal}

[Concurrency]{.caption-text}

-   [24. Introduction](sync/sync.html){.reference .internal}
-   [25. Basic Synchronization](sync/basic.html){.reference .internal}
    []{.toctree-toggle role="presentation"}
    -   [25.1. Cooperating Processes and Inter-process Communication](sync/sharing.html){.reference .internal}
    -   [25.2. The Critical Section Problem](sync/criticalsection.html){.reference .internal}
    -   [25.3. Implementing Locks](sync/locks.html){.reference .internal}
    -   [25.4. Ordering Thread Events](sync/ordering.html){.reference .internal}
-   [26. Common Concurrency Bugs](sync/concurrency_bugs.html){.reference .internal}
-   [27. Advanced Synchronization](sync/advanced.html){.reference .internal}
    []{.toctree-toggle role="presentation"}
    -   [27.1. Read-Dominated Workloads](sync/readmostly.html){.reference .internal}
    -   [27.2. Challenges of Modern Hardware](sync/hardware_challenges.html){.reference .internal}
    -   [27.3. Locking in the Linux Kernel](sync/linux_locking.html){.reference .internal}
-   [28. Review](sync/review.html){.reference .internal}

[Other Topics]{.caption-text}

-   [29. Input and Output](devices/devices.html){.reference .internal}
-   [30. More on Disks](devices/disk2.html){.reference .internal}
-   [31. Virtualization](virt/virt.html){.reference .internal}
-   [32. Security](sec/sec.html){.reference .internal}

[Appendices]{.caption-text}

-   [33. How to read this book](misc/howto.html){.reference .internal}
-   [34. Contributing](contributing/intro.html){.reference .internal}
    []{.toctree-toggle role="presentation"}
    -   [34.1. Examples](contributing/examples.html){.reference .internal}
    -   [34.2. Contributors](contributing/credit.html){.reference .internal}
    -   [34.3. Contributing](contributing/Contributing.html){.reference .internal}
    -   [34.6. Resources to look at](contributing/resources.html){.reference .internal}
    -   [34.7. Out of date](contributing/fix.html){.reference .internal}
-   [35. Bibliography](misc/bib.html){.reference .internal}
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
::: {.dropdown .dropdown-source-buttons}

-   [[ ]{.btn__icon-container} [Repository]{.btn__text-container}](https://github.com/OpenOSOrg/openos "Source repository"){.btn .btn-sm .btn-source-repository-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
-   [[ ]{.btn__icon-container} [Open issue]{.btn__text-container}](https://github.com/OpenOSOrg/openos/issues/new?title=Issue%20on%20page%20%2Fgenindex.html&body=Your%20issue%20content%20here. "Open an issue"){.btn .btn-sm .btn-source-issues-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
:::

[ ]{.btn__icon-container}
:::
:::
:::
:::
:::

::: {#jb-print-docs-body .onlyprint}
# 

::: {#print-main-content}
::: {#jb-print-toc}
:::
:::
:::

::: {#searchbox}
:::

# Index

::: genindex-jumpbox
:::

::: prev-next-area
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
