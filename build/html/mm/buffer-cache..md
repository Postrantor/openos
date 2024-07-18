---
docsearch:language: en
lang: en
title: 15. Buffer Cache --- Introduction to Operating Systems
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

- [6. Introduction](../scheduling/intro.html){.reference .internal}
- [7. The Process: A virtual Computer](../scheduling/process.html){.reference .internal}
- [8. Virtualizing the CPU](../scheduling/virtual.html){.reference .internal}
- [9. The Thread: A Virtual CPU](../scheduling/threads.html){.reference .internal}
- [10. Scheduling](../scheduling/scheduling.html){.reference .internal}
  []{.toctree-toggle role="presentation"}
  - [10.1. Scheduling Goals](../scheduling/sch-goals.html){.reference .internal}
  - [10.2. Simple Examples of Scheduling Policies](../scheduling/sch-simple.html){.reference .internal}
  - [10.3. Scheduling with Priorities](../scheduling/sch-prio.html){.reference .internal}
  - [10.4. Scheduling in the real world](../scheduling/sch-real.html){.reference .internal}
- [11. Review Questions](../scheduling/review.html){.reference .internal}

[Virtual Memory]{.caption-text}

- [12. Introduction](intro.html){.reference .internal}
- [13. Memory management before paged virtual memory](phys-and-seg.html){.reference .internal}
- [14. Paged Virtual memory](pagvm.html){.reference .internal}
  []{.toctree-toggle role="presentation"}
  - [14.1. Abstracting a useful interface for memory management.](vmabs.html){.reference .internal}
  - [14.2. Paging](virt-paging.html){.reference .internal}
  - [14.3. Page Tables](page-tables.html){.reference .internal}
  - [14.4. Memory reclaiming algorithms.](reclamation.html){.reference .internal}
  - [14.5. Page Sizes](page-size.html){.reference .internal}
  - [14.6. Memory Management Page Faults](pagefaults.html){.reference .internal}
- [15. Buffer Cache](#){.current .reference .internal}
- [16. Memory management in the real world](realworld.html){.reference .internal}
- [17. Conclusion](concl.html){.reference .internal}
- [18. Review](review.html){.reference .internal}

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

- [[ ![JupyterHub logo](../_static/images/logo_jupyterhub.svg) ]{.btn__icon-container} [JupyterHub]{.btn__text-container}](https://jupyterhub-opf-jupyterhub.apps.smaug.na.operate-first.cloud/hub/user-redirect/git-pull?repo=https%3A//github.com/OpenOSOrg/openos&urlpath=lab/tree/openos/content/mm/buffer-cache.ipynb&branch=main "Launch on JupyterHub"){.btn .btn-sm .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
  :::

::: {.dropdown .dropdown-source-buttons}

- [[ ]{.btn__icon-container} [Repository]{.btn__text-container}](https://github.com/OpenOSOrg/openos "Source repository"){.btn .btn-sm .btn-source-repository-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
- [[ ]{.btn__icon-container} [Suggest edit]{.btn__text-container}](https://github.com/OpenOSOrg/openos/edit/main/content/mm/buffer-cache.ipynb "Suggest edit"){.btn .btn-sm .btn-source-edit-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
- [[ ]{.btn__icon-container} [Open issue]{.btn__text-container}](https://github.com/OpenOSOrg/openos/issues/new?title=Issue%20on%20page%20%2Fmm/buffer-cache.html&body=Your%20issue%20content%20here. "Open an issue"){.btn .btn-sm .btn-source-issues-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
  :::

::: {.dropdown .dropdown-download-buttons}

- [[ ]{.btn__icon-container} [.ipynb]{.btn__text-container}](../_sources/mm/buffer-cache.ipynb "Download source file"){.btn .btn-sm .btn-download-source-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}

-  [ ]{.btn__icon-container} [.pdf]{.btn__text-container}
  :::

[ ]{.btn__icon-container}
:::
:::
:::
:::
:::

::: {#jb-print-docs-body .onlyprint}

# Buffer Cache

::: {#print-main-content}
::: {#jb-print-toc}
:::
:::
:::

::: {#searchbox}
:::

This chapter describes the buffer cache and how it is integrated with the memory management system as well as the file systems.

::: {#buffer-cache .section .tex2jax_ignore .mathjax_ignore}

# [15. ] {.section-number}Buffer Cache[\#](#buffer-cache "Link to this heading") {.headerlink}

On a typical paged virtual memory system a very small number of page frames are actually in use at any one time. All memory allocated to a program running in a process virtual address space is virtual memory. When a program starts running none of the virtual pages map to physical page frames until the program references a virtual page without a mapping and a page fault occurs. This happens repeatedly until the program maps an active subset of its virtual address space known as its process working set. Over time all of the running programs create their own process working sets and collectively all processes create a system wide working set which is typically much smaller the all of the page frames on the entire system leaving a set of unused or free page frames. Rather than allowing these free page frames to be unused the memory management system implements a Buffer Cache. The Buffer Cache uses the free page frames as an in-memory cache of file system data and even meta-data.

Each time a file system read occurs the Buffer Cache is searched to see if it can locate an in-memory copy of that data in one of the unused page frames. If that data is found(AKA buffer cache hit) it is simply copied from the page frame to the user buffer. If that data is not found(AKA buffer cache miss) the Buffer Cache allows the underlying file system to read the actual file data into a free page frame before copying it to the user buffer, afterwards any subsequent read for that data will be found in a free page frame(hit). A file system write is similar to a read with the exception that the user buffer data is copied from the user buffer to one of the free page frames and marking that buffer cache managed page "dirty". The underlying file system is called at some later time to write the contents of the associated dirty free page frame to the file itself and marking it "clean" after. This concept of delaying the writing of modified data from the Buffer Cache to the actual file system is known as a "write-back cache". This is in contrast with a "write-through cache" which would immediately write the modifications to the file system, blocking the write system call until its complete.

While it does add complexity to the memory management system the technique that the Buffer Cache uses of borrowing free page frames to cache file system data, copying between free page frames and user buffers and delaying the writes results in the file system read and write system calls being thousands or even millions times faster than doing actual file system IO operations. The complexity involves keeping track of which buffer cache pages are dirty and making sure they get written back to the underlying file at some point. How frequently dirty buffer cache pages get written to the actual file is a trade-off. If they are not written back frequently enough the in-memory copy is more up to date than the copy in the actual file. If a system crashes with a lot of dirty buffer cache pages a lot of data in the underlying files will be incorrect and file system data will be lost. On the other hand if the dirty buffer cache pages are written back to disk too frequently(frequency) or too many pages are written at the same time(magnitude), the file data will be written multiple times and the overall system performance will suffer. This is especially true if those files are temporary and will be deleted any time soon as is typically the case when compiling and linking large programs.

In the Unix/Linux operating system the buffer cache is implemented with an array of hash buckets or pointers to the linked list of pages with the same hash. Pages that cache a file's data blocks are placed in the hash list based on the inode/offset tuple. Once they are on a given hash list they can be easily found by using the inode/offset tuple to generate the hash index which locates the page list to search.

![[Fig. 15.1 ]{.caption-number}[Buffer Cache Structure]{.caption-text}[\#](#fig-bcstructure "Link to this image"){.headerlink}](../_images/BCstructure.png){style="width: 100%;"}

When a file system read() occurs the underlying file system searches the buffer cache for an in-memory cached copy of the file system data based on the inode/tuple for that data. If that data is not found the buffer cache code allocates one or more pages, performs file system read operations for that data along with other surrounding pages and inserts them into the appropriate buffer cache hash list.

![[Fig. 15.2 ]{.caption-number}[Buffer Cache read() with read-ahead]{.caption-text}[\#](#fig-bcread "Link to this image"){.headerlink}](../_images/BCread.png){style="width: 100%;"}

Since more than just the target page is read into the buffer cache subsequent pages are likely found and the read is a simple copy from the buffer cache page to the user's buffer.

![[Fig. 15.3 ]{.caption-number}[Buffer Cache read() of another page]{.caption-text}[\#](#fig-bcread2 "Link to this image"){.headerlink}](../_images/BCread2.png){style="width: 100%;"}

File system write() operations also search the buffer cache for an in-memory cached copy of the file data. If its not found(miss) it must be read into a new buffer cache page inserted into the appropriate hash list so subsequent look up operations will find it(hit). Once the page is found the user buffer is simply copied into the buffer cache page and a modified flag is set for that page. At later time a buffer cache kernel thread or daemon writes that page to the underlying file system and clears the modified flag.

![[Fig. 15.4 ]{.caption-number}[Buffer Cache write()]{.caption-text}[\#](#fig-bcwrite "Link to this image"){.headerlink}](../_images/BCwrite.png){style="width: 100%;"}

Since both the frequency and magnitude of writing/flushing dirty buffer cache pages is critical to both file system correctness and system performance there are often multiple tuning parameters that control this. The frequency which is the time between periodic flush operations is controlled by one parameter and the magnitude which is the actual amount of buffer cache data that is written back to the underlying file system is controlled by another parameter.

The mmap()ing of files also uses the buffer cache pages. The appropriate page table entries that map the underlying file into the processes virtual address space are created with the page frame number(PFN) of the page cache page when the file-backed page fault occurs.

![[Fig. 15.5 ]{.caption-number}[Buffer Cache mmap()'d file]{.caption-text}[\#](#fig-bcmmap "Link to this image"){.headerlink}](../_images/BCmmap.png){style="width: 100%;"}

Reclaiming buffer cache pages is typically very simple. Most of the buffer cache pages are 1.) clean/exactly the same as the underlying file system copy in storage, 2.) from a previously closed file and 3.) not mapped into any virtual address. If they are dirty/modified they must be written to the underlying file system and if they are mapped into a virtual address the associated page table entry(PTE) must be cleared out.

![[Fig. 15.6 ]{.caption-number}[Reclaiming Buffer Cache pages]{.caption-text}[\#](#fig-bcreclaim "Link to this image"){.headerlink}](../_images/BCreclaim.png){style="width: 100%;"}
:::

::: prev-next-area
[](pagefaults.html "previous page"){.left-prev}

::: prev-next-info
previous

[14.6. ]{.section-number}Memory Management Page Faults
:::

[](realworld.html "next page"){.right-next}

::: prev-next-info
next

[16. ]{.section-number}Memory management in the real world
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
