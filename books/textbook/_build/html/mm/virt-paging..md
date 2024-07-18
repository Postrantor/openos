---
docsearch:language: en
lang: en
title: 14.2. Paging --- Introduction to Operating Systems
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
    -   [14.2. Paging](#){.current .reference .internal}
    -   [14.3. Page Tables](page-tables.html){.reference .internal}
    -   [14.4. Memory reclaiming algorithms.](reclamation.html){.reference .internal}
    -   [14.5. Page Sizes](page-size.html){.reference .internal}
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

-   [[ ![JupyterHub logo](../_static/images/logo_jupyterhub.svg) ]{.btn__icon-container} [JupyterHub]{.btn__text-container}](https://jupyterhub-opf-jupyterhub.apps.smaug.na.operate-first.cloud/hub/user-redirect/git-pull?repo=https%3A//github.com/OpenOSOrg/openos&urlpath=lab/tree/openos/content/mm/virt-paging.ipynb&branch=main "Launch on JupyterHub"){.btn .btn-sm .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
:::

::: {.dropdown .dropdown-source-buttons}

-   [[ ]{.btn__icon-container} [Repository]{.btn__text-container}](https://github.com/OpenOSOrg/openos "Source repository"){.btn .btn-sm .btn-source-repository-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
-   [[ ]{.btn__icon-container} [Suggest edit]{.btn__text-container}](https://github.com/OpenOSOrg/openos/edit/main/content/mm/virt-paging.ipynb "Suggest edit"){.btn .btn-sm .btn-source-edit-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
-   [[ ]{.btn__icon-container} [Open issue]{.btn__text-container}](https://github.com/OpenOSOrg/openos/issues/new?title=Issue%20on%20page%20%2Fmm/virt-paging.html&body=Your%20issue%20content%20here. "Open an issue"){.btn .btn-sm .btn-source-issues-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
:::

::: {.dropdown .dropdown-download-buttons}

-   [[ ]{.btn__icon-container} [.ipynb]{.btn__text-container}](../_sources/mm/virt-paging.ipynb "Download source file"){.btn .btn-sm .btn-download-source-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
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
# Paging

::: {#print-main-content}
::: {#jb-print-toc}
<div>

## Contents

</div>

-   [14.2.1. Paged Address Translation](#paged-address-translation){.reference .internal .nav-link}
    -   [14.2.1.1. The virtual address space with Paging](#the-virtual-address-space-with-paging){.reference .internal .nav-link}
-   [14.2.2. MMU Memory Management Unit](#mmu-memory-management-unit){.reference .internal .nav-link}
    -   [14.2.2.1. Memory Over-Commitment and Paging](#memory-over-commitment-and-paging){.reference .internal .nav-link}
-   [14.2.3. Paging - Avoiding Fragmentation](#paging-avoiding-fragmentation){.reference .internal .nav-link}
    -   [14.2.3.1. Internal Fragmentation](#internal-fragmentation){.reference .internal .nav-link}
:::
:::
:::

::: {#searchbox}
:::

This chapter describes a pages virtual memory system works, what the MMU is and how it works and how we over commit physical memory using it.

::: {#paging .section .tex2jax_ignore .mathjax_ignore}
# [14.2. ]{.section-number}Paging[\#](#paging "Link to this heading"){.headerlink}

::: {#paged-address-translation .section}
## [14.2.1. ]{.section-number}Paged Address Translation[\#](#paged-address-translation "Link to this heading"){.headerlink}

Most virtual memory systems today use a paged address translation AKA paging. A paged virtual memory system divides both virtual memory and physical memory into relatively small fixed size chunks pieces. They are known as virtual pages or just pages in the virtual address space and page frames in the physical memory space. The memory management system maintains a mapping for each virtual page in use to a page frame that contains the actual memory contents.

![[Fig. 14.1 ]{.caption-number}[Paged virtual memory example]{.caption-text}[\#](#paged-memory "Link to this image"){.headerlink}](../_images/pagedmem.png){style="width: 100%;"}

Paging solves a couple major problems that segmentation has: 1.) The paged virtual address space can be much larger than physical memory. 2.) Paging eliminates the need to maintain large regions of physically contiguous memory.

In the segmentation memory model its not possible to run a program that's requires more physical memory than the system has. This means a program may run on a system with a large amount of memory and not be able to run on a system with a smaller amount of memory at all.

Another benefit of paging over segmentation is that a region of virtual memory does not need to map physically contiguous memory. Since the virtual address space is divided into small fixed size pages a virtually contiguous region of memory can map several page frames that are randomly scattered throughout the entire physical memory.

::: {#the-virtual-address-space-with-paging .section}
### [14.2.1.1. ]{.section-number}The virtual address space with Paging[\#](#the-virtual-address-space-with-paging "Link to this heading"){.headerlink}

On a paged virtual memory system every process has exactly the same size virtual address space, gigabytes, terabytes or even petabytes on modern systems is typical. By default none of the virtual pages within this huge address space is valid when a process and it's associated virtual address space is created and therefore can not be referenced. In order to make regions of the virtual address space valid either part of a file must be mapped into a virtual region or virtual memory must be dynamically allocated creating a virtual region. Since the virtual regions are relatively small the huge virtual address space is sparsely populated with small valid virtual regions. As we discussed earlier in this book a process and its associated virtual address space is created when a child process is created via fork(). At this time the valid virtual regions are duplicated from the parent process to the child process. The regions within the virtual address space can also be eliminated and new ones created when the process runs a different program via exec().

When the virtual regions are initially created or the virtual address is changed no page frames are mapped into the virtual pages within them, however a program can legally access pages within the virtual regions. When this happens the memory management system responds by mapping a physical page into each virtual page as it is accessed or on demand. This means the virtual regions are sparsely populated with physical memory pages, similar to the way the entire virtual address space is sparsely populated with valid virtual regions. As a process runs on a paged virtual memory system only a small subset of physical page frames are required to be mapped into virtual memory pages at a given time.

The paged virtual memory management system is responsible for multiplexing the page frames and insuring that at least the necessary virtual to physical mappings are in place. On systems with larger amounts of physical memory more page frames can be mapped into virtual pages than systems with smaller amounts of physical memory. This means a program running on a small memory system probably just runs slower than on systems with large amounts rather than not being able to run at all. This is a huge improvement over segmented systems where some programs can not run at all on systems without adequate memory.

Another benefit of paging over segmentation is that a region of virtual memory does not need to map physically contiguous page frames. Since the virtual address space is divided into small fixed size pages a virtually contiguous region can map page frames that are randomly scattered throughout the entire physical memory. This eliminates the need to maintain physically contiguous memory, an overhead that is both complex and very CPU intensive. In addition, it completely eliminates external fragmentation, further eliminating the need to perform compaction. The only fragmentation issue encountered in a page virtual memory system is internal fragmentation. An internal fragment is the unused portion of a page at the end of a region of virtual memory. An internal fragment which is only half of one page on the average is typically much smaller than the external fragment associated with segmentation can not be reclaimed by the memory management system.
:::
:::

::: {#mmu-memory-management-unit .section}
## [14.2.2. ]{.section-number}MMU Memory Management Unit[\#](#mmu-memory-management-unit "Link to this heading"){.headerlink}

Every time a virtual address is referenced it must be translated to a physical address before presenting it to the memory address bus hardware. This would be unacceptably slow so on paged systems the CPU includes special hardware that maintains the virtual to physical page mappings for each page. This CPU hardware is known as the Memory Management Unit or MMU.

We examine a single model of address translation in detail: the one used by the original Pentium, and by any Intel-compatible CPU running in 32-bit mode. It uses 32-bit virtual addresses, 32-bit physical addresses, and a page size of 4096 bytes. Since pages are [\\(2\^{12}\\)]{.math .notranslate .nohighlight} bytes each, addresses can be divided into 20-bit page numbers and 12-bit offsets within each page, as shown in [[Fig. 14.3]{.std .std-numref}](#fig-vm-fig5){.reference .internal}.

![[Fig. 14.2 ]{.caption-number}[Example of virtual address mapping to physical address]{.caption-text}[\#](#fig-vm-fig6 "Link to this image"){.headerlink}](../_images/virt-mem-pic10.png){style="height: 5.5cm;"}

The Memory Management Unit (MMU) maps a 20-bit virtual page number to a 20-bit physical page number; the offset can pass through unchanged, as shown in [[Fig. 14.2]{.std .std-numref}](#fig-vm-fig6){.reference .internal}, giving the physical address the CPU should access.

![[Fig. 14.3 ]{.caption-number}[Page number and offset in 32-bit paged translation with 4KB pages]{.caption-text}[\#](#fig-vm-fig5 "Link to this image"){.headerlink}](../_images/virt-mem-pic9.png){style="width: 100%;"}

Although paged address translation is far more flexible than base and bounds registers found in segmentation, it requires much more information. Base and bounds translation only requires two values, which can easily be held in registers in the MMU. In contrast, paged translation must be able to handle a separate mapping value for each of thousands or even million virtual pages(although most programs will only map a fraction of those pages). The only possible place to store the amount of information required by paged address translation is in tables located in memory itself. These memory resident tables of virtual to physical translations are known as page tables. The MMU uses the in-memory page tables or mappings to translate from every virtual address to the actual physical addresses.

::: {#memory-over-commitment-and-paging .section}
### [14.2.2.1. ]{.section-number}Memory Over-Commitment and Paging[\#](#memory-over-commitment-and-paging "Link to this heading"){.headerlink}

Page faults allow data to be dynamically fetched into memory when it is needed, in the same way that the CPU dynamically fetches data from memory into the cache. This allows the operating system to over-commit memory: the sum of all process address spaces can add up to more memory than is available, although the total amount of memory mapped at any point in time must fit into RAM. This means that when a page fault occurs and a page is allocated to a process, another page (from that or another process) may need to be evicted from memory.

There are two types of regions in a user a user's virtual address space: file-backed and anonymous.

File-backed regions are contiguous portions of a file on storage that is mapped into a user's virtual address space. For example the exec()system call mmap()'s the text and data section of an executable file into a users address space at predetermined virtual addresses. The majority of the page frames mapped into file backed regions are read-only mappings and therefore are never modified so never need to be flushed or written back to storage. When a process exits and munmap()s its file-backed regions nothing is deleted. Everything is from some file that exist on some storage device.

Anonymous memory regions do not correspond to a file. Instead, they are the data, heap and stack regions of the user's virtual address space. Unlike file-backed regions the page frames mapped into anonymous regions are almost always modified. Consider what would be the sense of allocating from a heap and only reading from it? For this reason all page frames mapped into anonymous regions must be written to some storage location if it is to be reclaimed. Also unlike file-backed regions all the page frames mapped into anonymous regions are deleted and therefor immediately freed. The data, heap and stack contents of a process that is exiting is on no value to any other process and therefor can be eliminated

Evicting a read-only page mapped from a file is simple: just forget the mapping and free the page; if a fault for that page occurs later, the page can be read back from disk. Occasionally pages are mapped read/write from a file, when a program explicitly requests it with `mmap`{.docutils .literal .notranslate}---in that case the OS can write any modified data back to the file and then evict the page; again it can be paged back from disk if needed again.

Anonymous segments such as stack and heap are typically created in memory and do not need to be swapped; however if the system runs low on memory it may evict anonymous pages owned by idle processes, in order to give more memory to the currently-running ones. To do this the OS allocates a location in "swap space" on disk: typically a dedicated swap partition in Linux, and the `PAGEFILE.sys`{.docutils .literal .notranslate} and `/var/vm/swapfile`{.docutils .literal .notranslate} files in Windows and OSX respectively. The data must first be written out to that location, then the OS can store the page-to-location mapping and release the memory page.

Hint: Linux uses/borrows the page table entry to store the location of a swapped out page.\
As long as the PTE present bit is not set the MMU hardware will not attempt to translate, instead it will cause a page fault. The entire PTE can be used by software when the present bit is not set.

![[Fig. 14.4 ]{.caption-number}[Page table entry with D (dirty) bit]{.caption-text}[\#](#fig-vm-pic106 "Link to this image"){.headerlink}](../_images/virt-mem-pic106.png){style="width: 100%;"}
:::
:::

::: {#paging-avoiding-fragmentation .section}
## [14.2.3. ]{.section-number}Paging - Avoiding Fragmentation[\#](#paging-avoiding-fragmentation "Link to this heading"){.headerlink}

The fragmentation in [[Fig. 13.13]{.std .std-numref}](phys-and-seg.html#mm-virt-mem-frag-4){.reference .internal} is termed *external fragmentation*, because the memory wasted is *external* to the regions allocated. This situation can be avoided by *compacting* memory---moving existing allocations around, thereby consolidating multiple blocks of free memory into a single large chunk. This is a slow process, requiring processes to be paused, large amounts of memory to be copied, and base+bounds registers modified to point to new locations\[\^2\].

![[Fig. 14.5 ]{.caption-number}[A mapping between virtual pages and physical pages]{.caption-text}[\#](#fig-vm-fig3 "Link to this image"){.headerlink}](../_images/virt-mem-map.png){style="width: 100%;"}

Instead, modern CPUs use *paged address translation*, which divides the physical and virtual memory spaces into fixed-sized pages, typically 4KB, and provides a flexible mapping between virtual and physical pages, as shown in [[Fig. 14.5]{.std .std-numref}](#fig-vm-fig3){.reference .internal}. The operating system can then maintain a list of free physical pages, and allocate them as needed. Because any combination of physical pages may be used for an allocation request, there is no external fragmentation, and a request will not fail as long as there are enough free physical pages to fulfill it.

::: {#internal-fragmentation .section}
### [14.2.3.1. ]{.section-number}Internal Fragmentation[\#](#internal-fragmentation "Link to this heading"){.headerlink}

Paging solves the problem of external fragmentation, there is no wasted space between pages of virtual memory. However, paging does suffer from another issue, *internal fragmentation*, space may be wasted *inside* the allocated pages. E.g. if 10 KB of memory is allocated in 4KB pages, 3 pages (a total of 12 KB) are allocated, and 2KB is wasted. To allocate hundreds of KB in pages of 4KB this is a minor overhead: about [\\(\\frac{1}{2}\\)]{.math .notranslate .nohighlight} a page, or 2 KB, wasted per allocation. But internal fragmentation makes this approach inefficient for very small allocations (e.g. the `new`{.docutils .literal .notranslate} operator in C++), as shown in [[Fig. 14.6]{.std .std-numref}](#fig-vm-fig4){.reference .internal}. (It is also one reason why even though most CPUs support multi-megabyte or even multi-gigabyte "huge" pages, which are slightly more efficient than 4 KB pages, they are rarely used.)

![[Fig. 14.6 ]{.caption-number}[Example of internal fragmentation]{.caption-text}[\#](#fig-vm-fig4 "Link to this image"){.headerlink}](../_images/virt-mem-pic7.png){style="width: 90%;"}
:::
:::
:::

::: prev-next-area
[](vmabs.html "previous page"){.left-prev}

::: prev-next-info
previous

[14.1. ]{.section-number}Abstracting a useful interface for memory management.
:::

[](page-tables.html "next page"){.right-next}

::: prev-next-info
next

[14.3. ]{.section-number}Page Tables
:::
:::
:::

::: {.bd-sidebar-secondary .bd-toc}
::: {.sidebar-secondary-items .sidebar-secondary__inner}
::: sidebar-secondary-item
::: {.page-toc .tocsection .onthispage}
Contents
:::

-   [14.2.1. Paged Address Translation](#paged-address-translation){.reference .internal .nav-link}
    -   [14.2.1.1. The virtual address space with Paging](#the-virtual-address-space-with-paging){.reference .internal .nav-link}
-   [14.2.2. MMU Memory Management Unit](#mmu-memory-management-unit){.reference .internal .nav-link}
    -   [14.2.2.1. Memory Over-Commitment and Paging](#memory-over-commitment-and-paging){.reference .internal .nav-link}
-   [14.2.3. Paging - Avoiding Fragmentation](#paging-avoiding-fragmentation){.reference .internal .nav-link}
    -   [14.2.3.1. Internal Fragmentation](#internal-fragmentation){.reference .internal .nav-link}
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
