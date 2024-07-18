---
docsearch:language: en
lang: en
title: 14.5. Page Sizes --- Introduction to Operating Systems
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

-   [12. Introduction](intro.html){.reference .internal}
-   [13. Memory management before paged virtual memory](phys-and-seg.html){.reference .internal}
-   [14. Paged Virtual memory](pagvm.html){.reference .internal}
    []{.toctree-toggle role="presentation"}
    -   [14.1. Abstracting a useful interface for memory management.](vmabs.html){.reference .internal}
    -   [14.2. Paging](virt-paging.html){.reference .internal}
    -   [14.3. Page Tables](page-tables.html){.reference .internal}
    -   [14.4. Memory reclaiming algorithms.](reclamation.html){.reference .internal}
    -   [14.5. Page Sizes](#){.current .reference .internal}
    -   [14.6. Memory Management Page Faults](pagefaults.html){.reference .internal}
-   [15. Buffer Cache](buffer-cache.html){.reference .internal}
-   [16. Memory management in the real world](realworld.html){.reference .internal}
-   [17. Conclusion](concl.html){.reference .internal}
-   [18. Review](review.html){.reference .internal}

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

-   [[ ![JupyterHub logo](../_static/images/logo_jupyterhub.svg) ]{.btn__icon-container} [JupyterHub]{.btn__text-container}](https://jupyterhub-opf-jupyterhub.apps.smaug.na.operate-first.cloud/hub/user-redirect/git-pull?repo=https%3A//github.com/OpenOSOrg/openos&urlpath=lab/tree/openos/content/mm/page-size.ipynb&branch=main "Launch on JupyterHub"){.btn .btn-sm .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
:::

::: {.dropdown .dropdown-source-buttons}

-   [[ ]{.btn__icon-container} [Repository]{.btn__text-container}](https://github.com/OpenOSOrg/openos "Source repository"){.btn .btn-sm .btn-source-repository-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
-   [[ ]{.btn__icon-container} [Suggest edit]{.btn__text-container}](https://github.com/OpenOSOrg/openos/edit/main/content/mm/page-size.ipynb "Suggest edit"){.btn .btn-sm .btn-source-edit-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
-   [[ ]{.btn__icon-container} [Open issue]{.btn__text-container}](https://github.com/OpenOSOrg/openos/issues/new?title=Issue%20on%20page%20%2Fmm/page-size.html&body=Your%20issue%20content%20here. "Open an issue"){.btn .btn-sm .btn-source-issues-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
:::

::: {.dropdown .dropdown-download-buttons}

-   [[ ]{.btn__icon-container} [.ipynb]{.btn__text-container}](../_sources/mm/page-size.ipynb "Download source file"){.btn .btn-sm .btn-download-source-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
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
# Page Sizes

::: {#print-main-content}
::: {#jb-print-toc}
<div>

## Contents

</div>

-   [14.5.1. Small page sizes](#small-page-sizes){.reference .internal .nav-link}
    -   [14.5.1.1. Pros:](#pros){.reference .internal .nav-link}
    -   [14.5.1.2. Cons:](#cons){.reference .internal .nav-link}
-   [14.5.2. Large page sizes](#large-page-sizes){.reference .internal .nav-link}
    -   [14.5.2.1. Pros:](#id1){.reference .internal .nav-link}
    -   [14.5.2.2. Cons:](#id2){.reference .internal .nav-link}
:::
:::
:::

::: {#searchbox}
:::

This chapter describes what page sizes, the pros and cons if small vs large page sizes and how some systems can use multiple page sizes at the same time.

::: {#page-sizes .section .tex2jax_ignore .mathjax_ignore}
# [14.5. ]{.section-number}Page Sizes[\#](#page-sizes "Link to this heading"){.headerlink}

Most modern processors that support a paged virtual memory model also support multiple page sizes. There are several benefits and downsides of any page size.

A smaller page size reduces the internal fragmentation, on the average 1/2 of the last page of a memory region will be unused or wasted. Half of a 4KB page is only 2KB but half of a 1GB page is 512MB! Smaller page sizes also make for a more compact virtual address space since pages must be aligned on their size boundaries. When the virtual address space is more compact both text and data regions can be smaller and closer together allowing for more efficient relative addressing instructions to be used. This typically results in fewer memory references because the distance between instructions and data is smaller and fit within an instruction. This is especially true for smaller programs.

A larger page size allows for fewer page structures for a given amount of memory that the memory management system has to manage. This means that fewer page structures will be on various linked lists, etc. which typically results in needing to hold spin locks for shorter periods of time when walking these linked lists. A larger page size also results in significantly more text and data being mapped in translation caches. A cache that has 128 entries can only map 512KB with a 4KB page size where it can map 128GB with a 1GB page size. This alone will practically eliminate translation cache misses once a process is running.

Selecting a page size is a trade-off and there is really no one-size fits all optimally. The Intel x86_64 processor supports 3 page sizes; 4KB, 2MB and 1GB. Most operating systems that will run on this architecture can be built and booted to run any of these page sizes. In addition, the x86_64 can use all 3 pages sizes at the same time within a single address space. Regions of memory that are fairly small(measured in KB) like a stack or heap might use a 4KB page size. Regions of memory that are larger(measured in MB) like a large program text or shared library text might use a 2MB page size. Finally regions of memory that are huge like a data base cache or huge shared mapped files might use a 1GB page size.

![[Fig. 14.21 ]{.caption-number}[X86_64 page sizes]{.caption-text}[\#](#fig-pagesize "Link to this image"){.headerlink}](../_images/pagesize.png){style="width: 100%;"}

::: {#small-page-sizes .section}
## [14.5.1. ]{.section-number}Small page sizes[\#](#small-page-sizes "Link to this heading"){.headerlink}

::: {#pros .section}
### [14.5.1.1. ]{.section-number}Pros:[\#](#pros "Link to this heading"){.headerlink}

1.  Less internal fragmentation

2.  Better fit for various data structures, code sections

3.  Less unused program memory
:::

::: {#cons .section}
### [14.5.1.2. ]{.section-number}Cons:[\#](#cons "Link to this heading"){.headerlink}

1.  Programs need many pages, larger page tables

2.  More TLB misses

3.  Higher memory management overhead
:::
:::

::: {#large-page-sizes .section}
## [14.5.2. ]{.section-number}Large page sizes[\#](#large-page-sizes "Link to this heading"){.headerlink}

::: {#id1 .section}
### [14.5.2.1. ]{.section-number}Pros:[\#](#id1 "Link to this heading"){.headerlink}

1.  Smaller page tables

2.  fewer TLB misses

3.  Lower memory management overhead
:::

::: {#id2 .section}
### [14.5.2.2. ]{.section-number}Cons:[\#](#id2 "Link to this heading"){.headerlink}

1.  More internal fragmentation

2.  More unused program memory

3.  Worse fit for various data structures, code sections
:::
:::
:::

::: prev-next-area
[](reclamation.html "previous page"){.left-prev}

::: prev-next-info
previous

[14.4. ]{.section-number}Memory reclaiming algorithms.
:::

[](pagefaults.html "next page"){.right-next}

::: prev-next-info
next

[14.6. ]{.section-number}Memory Management Page Faults
:::
:::
:::

::: {.bd-sidebar-secondary .bd-toc}
::: {.sidebar-secondary-items .sidebar-secondary__inner}
::: sidebar-secondary-item
::: {.page-toc .tocsection .onthispage}
Contents
:::

-   [14.5.1. Small page sizes](#small-page-sizes){.reference .internal .nav-link}
    -   [14.5.1.1. Pros:](#pros){.reference .internal .nav-link}
    -   [14.5.1.2. Cons:](#cons){.reference .internal .nav-link}
-   [14.5.2. Large page sizes](#large-page-sizes){.reference .internal .nav-link}
    -   [14.5.2.1. Pros:](#id1){.reference .internal .nav-link}
    -   [14.5.2.2. Cons:](#id2){.reference .internal .nav-link}
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
