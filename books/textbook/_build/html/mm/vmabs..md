---
docsearch:language: en
lang: en
title: 14.1. Abstracting a useful interface for memory management. --- Introduction to Operating Systems
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
    -   [14.1. Abstracting a useful interface for memory management.](#){.current .reference .internal}
    -   [14.2. Paging](virt-paging.html){.reference .internal}
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

-   [[ ![JupyterHub logo](../_static/images/logo_jupyterhub.svg) ]{.btn__icon-container} [JupyterHub]{.btn__text-container}](https://jupyterhub-opf-jupyterhub.apps.smaug.na.operate-first.cloud/hub/user-redirect/git-pull?repo=https%3A//github.com/OpenOSOrg/openos&urlpath=lab/tree/openos/content/mm/vmabs.ipynb&branch=main "Launch on JupyterHub"){.btn .btn-sm .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
:::

::: {.dropdown .dropdown-source-buttons}

-   [[ ]{.btn__icon-container} [Repository]{.btn__text-container}](https://github.com/OpenOSOrg/openos "Source repository"){.btn .btn-sm .btn-source-repository-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
-   [[ ]{.btn__icon-container} [Suggest edit]{.btn__text-container}](https://github.com/OpenOSOrg/openos/edit/main/content/mm/vmabs.ipynb "Suggest edit"){.btn .btn-sm .btn-source-edit-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
-   [[ ]{.btn__icon-container} [Open issue]{.btn__text-container}](https://github.com/OpenOSOrg/openos/issues/new?title=Issue%20on%20page%20%2Fmm/vmabs.html&body=Your%20issue%20content%20here. "Open an issue"){.btn .btn-sm .btn-source-issues-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
:::

::: {.dropdown .dropdown-download-buttons}

-   [[ ]{.btn__icon-container} [.ipynb]{.btn__text-container}](../_sources/mm/vmabs.ipynb "Download source file"){.btn .btn-sm .btn-download-source-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
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
# Abstracting a useful interface for memory management.

::: {#print-main-content}
::: {#jb-print-toc}
<div>

## Contents

</div>

-   [14.1.1. The Virtual Interface](#the-virtual-interface){.reference .internal .nav-link}
-   [14.1.2. Basic Memory Management functions](#basic-memory-management-functions){.reference .internal .nav-link}
    -   [14.1.2.1. Library calls](#library-calls){.reference .internal .nav-link}
    -   [14.1.2.2. system calls](#system-calls){.reference .internal .nav-link}
-   [14.1.3. Physical Memory/No Virtual Memory](#physical-memory-no-virtual-memory){.reference .internal .nav-link}
-   [14.1.4. Virtual Memory](#virtual-memory){.reference .internal .nav-link}
    -   [14.1.4.1. Segmented Virtual Memory](#segmented-virtual-memory){.reference .internal .nav-link}
    -   [14.1.4.2. Paged Virtual Memory](#paged-virtual-memory){.reference .internal .nav-link}
        -   [14.1.4.2.1. The virtual address space](#the-virtual-address-space){.reference .internal .nav-link}
        -   [14.1.4.2.2. Pros](#pros){.reference .internal .nav-link}
        -   [14.1.4.2.3. Cons](#cons){.reference .internal .nav-link}
:::
:::
:::

::: {#searchbox}
:::

::: {#abstracting-a-useful-interface-for-memory-management .section .tex2jax_ignore .mathjax_ignore}
[]{#cont-mm-pvm-abs}

# [14.1. ]{.section-number}Abstracting a useful interface for memory management.[\#](#abstracting-a-useful-interface-for-memory-management "Link to this heading"){.headerlink}

One of the fundamental jobs of the memory management system is to provide a useful abstraction to the system's physical memory. This abstraction must be conducive to writing and running applications without needing to know the details of the physical memory. The MM abstraction must provide a consistent virtual interface to physical memory and provide a set of operating systems services that create, delete, expand, contract and manipulate regions of virtual memory that the running programs use.

::: {#the-virtual-interface .section}
## [14.1.1. ]{.section-number}The Virtual Interface[\#](#the-virtual-interface "Link to this heading"){.headerlink}

The virtual interface must transparently hide the details of the actual physical memory on the system and provide the same interface to every running process. This interface or "Virtual Address Space' should appear as an array bytes and start at the same location for every process. In the ideal world virtual address space provided by the operating system would be identical for every process and provide a set of functions that allow programs to manipulate it.
:::

::: {#basic-memory-management-functions .section}
## [14.1.2. ]{.section-number}Basic Memory Management functions[\#](#basic-memory-management-functions "Link to this heading"){.headerlink}

As mentioned earlier the memory management systems must provide a set of operating systems services that create, delete, expand, contract and manipulate regions of virtual memory that the running programs use. These memory management functions provided to user programs can be divided into 2 categories: library calls and system calls.

::: {#library-calls .section}
### [14.1.2.1. ]{.section-number}Library calls[\#](#library-calls "Link to this heading"){.headerlink}

The most basic memory management library functions to allocate and free virtual memory are malloc() and free() respectively.

1.) malloc(): The malloc library function use is "address=malloc(size)" where you pass the number of bytes you want to allocate in size and malloc returns the virtual address of the memory allocated into address.

2.) free(): The free library function use is "status=free(address)" where address is the virtual address malloc() returned to the user and status is simply an indication of success or failure.
:::

::: {#system-calls .section}
### [14.1.2.2. ]{.section-number}system calls[\#](#system-calls "Link to this heading"){.headerlink}

The memory management system calls are sbrk(), brk(), mmap(), munmap() and mprotect().

1.) sbrk(): The sbrk() system call is used to expand and contract the end of the program's data section. The use is prev=sbrk(size)" where size is the positive or negative number of bytes to expand or extract the end of the data section and prev is the end of the data section before the call.

2.) brk(): The brk() system call is used to explicitly set the end of the program's data section. The use is "status=brk(address)" where address is where to set the end of the data section and status is the success/failure of the call.

3.) mmap(): The mmap() system call is used to allocate anonymous memory in page sized increments into a contiguous set of virtual pages or map the contents of a file segment into a set virtual pages. The use is "address=mmap(arguments, ...)" where the arguments instruct whether to allocate anonymous memory or map a file section and address is the page aligned virtual address of the newly allocated memory.

4.) munmap(): The munmap() system call is used free anonymous memory allocated via mmap() or unmap the contents of a file segment that was mapped via mmap(). The use is "status=munmap(address, size)" where address is the page aligned virtual address to be unmapped, size is the size of memory to be unmapped and status is the success of the call.

5.) mprotect(): The mprotect() system call is used to set the protection for a range of valid virtual pages. The use is "status=mprotect(address, size, protection)" where address is the base address and size is the location and size of the virtual region that gets the new protection.
:::
:::

::: {#physical-memory-no-virtual-memory .section}
## [14.1.3. ]{.section-number}Physical Memory/No Virtual Memory[\#](#physical-memory-no-virtual-memory "Link to this heading"){.headerlink}

On a system without virtual memory there is one physical address space and programs are loaded into physical memory, allocate physical memory as needed and directly access those physical memory locations or addresses. If more than one program is running at the same time they are simply loaded into a different physical address and allocate different physical addresses. This means every program must either know the physical address that it is running or it must be relocated when it is loaded.
:::

::: {#virtual-memory .section}
## [14.1.4. ]{.section-number}Virtual Memory[\#](#virtual-memory "Link to this heading"){.headerlink}

What is most desirable and usable is a virtual memory model where every program would run in a process that has a unique but identical virtual address space. A virtual address space would ideally start at address zero and extend up to some very large address. Since every process appears to have the same virtual address space programs can be loaded at the same virtual address and therefore do not need to to be relocated. There are 2 basic virtual memory models: Segmented Virtual Memory and Paged Virtual Memory.

::: {#segmented-virtual-memory .section}
### [14.1.4.1. ]{.section-number}Segmented Virtual Memory[\#](#segmented-virtual-memory "Link to this heading"){.headerlink}

A simple segmented virtual address space starts at location zero and extend up to some upper limit. Its implemented in hardware using base and offset registers. Every memory reference is virtual and is translated to a physical address in hardware by adding the base register to the virtual address and qualified by insuring the result is less than the offset register.
:::

::: {#paged-virtual-memory .section}
### [14.1.4.2. ]{.section-number}Paged Virtual Memory[\#](#paged-virtual-memory "Link to this heading"){.headerlink}

A paged virtual memory model splits both the virtual address space and physical memory into fixed size pieces knows as virtual pages and physical page frames respectively. The mapping of virtual pages to physical page frames is accomplished via an array of page frame numbers known as a page table. There is one page table entry for each virtual page and only then pages that are being used contain valid page table entries and therefore map physical page frames.

::: {#the-virtual-address-space .section}
#### [14.1.4.2.1. ]{.section-number}The virtual address space[\#](#the-virtual-address-space "Link to this heading"){.headerlink}

The virtual address space of every process is typically very large and fixed in size, for example the virtual address space for every process running on an x86_64 system is 2\^48 or 258TB. By default the entire virtual address space is not accessible to programs running in it. The only portions or regions that are accessible are those that the program requested via system calls(mmap and sbrk) and the kernel granted access to. So the virtual address space is sparsely populated with valid regions and those are either anonymous regions or file-backed regions. Anonymous regions are any region that is not backed by a file, for example; stacks, heaps, BSS, malloc()'d and sbrk()'d regions. File-backed regions are sections of a file that are mapped into the virtual address space. Once the valid regions have been created physical memory pages are mapped into the virtual pages on demand therefore those regions are sparsely populated with physical memory.

Paged virtual memory aka paging introduces the possibility of several additional highly desirable features or pros to the memory management system but also introduces several additional challenges or cons.
:::

::: {#pros .section}
#### [14.1.4.2.2. ]{.section-number}Pros[\#](#pros "Link to this heading"){.headerlink}

-   Several huge virtual address spaces can be much larger than physical memory via over-committing physical memory.

-   Total isolation of each virtual address space from all others.

-   Sharing of selective regions of memory between different virtual address spaces is easy.

-   Use of memory pages to cache file system data and meta-data is possible.

-   Very large and sparse virtual address space requires page fault logic that maps physical memory on-demand.
:::

::: {#cons .section}
#### [14.1.4.2.3. ]{.section-number}Cons[\#](#cons "Link to this heading"){.headerlink}

-   Over-committing physical memory requires sophisticated page reclaim logic.

-   Supporting multiple page sizes on different architectures complicates an already complex memory management system.

-   Very large virtual address space requires large and complex multi-level page table design.

The next chapter describes...

-   [[virt-seg]{.std .std-ref}](phys-and-seg.html#cont-mm-virt-seg){.reference .internal}

-   [[virt-paging]{.std .std-ref}](virt-paging.html#cont-mm-virt-paging){.reference .internal}

-   [[page-tables]{.xref .myst}](#cont:mm:page-tables){.reference .internal}

-   [[reclamation]{.std .std-ref}](reclamation.html#cont-mm-reclamation){.reference .internal}

-   [[page-size]{.std .std-ref}](page-size.html#cont-mm-page-size){.reference .internal}

-   [[misc]{.xref .myst}](#cont:mm:misc){.reference .internal}

-   [[buffer-cache]{.std .std-ref}](buffer-cache.html#cont-mm-buffer-cache){.reference .internal}

-   [[mem-dynamics]{.std .std-ref}](pagefaults.html#cont-mm-mmdyn){.reference .internal}

-   [[realworld]{.std .std-ref}](realworld.html#cont-mm-realworld){.reference .internal}

-   [[concl]{.std .std-ref}](concl.html#cont-mm-concl){.reference .internal}
:::
:::
:::
:::

::: prev-next-area
[](pagvm.html "previous page"){.left-prev}

::: prev-next-info
previous

[14. ]{.section-number}Paged Virtual memory
:::

[](virt-paging.html "next page"){.right-next}

::: prev-next-info
next

[14.2. ]{.section-number}Paging
:::
:::
:::

::: {.bd-sidebar-secondary .bd-toc}
::: {.sidebar-secondary-items .sidebar-secondary__inner}
::: sidebar-secondary-item
::: {.page-toc .tocsection .onthispage}
Contents
:::

-   [14.1.1. The Virtual Interface](#the-virtual-interface){.reference .internal .nav-link}
-   [14.1.2. Basic Memory Management functions](#basic-memory-management-functions){.reference .internal .nav-link}
    -   [14.1.2.1. Library calls](#library-calls){.reference .internal .nav-link}
    -   [14.1.2.2. system calls](#system-calls){.reference .internal .nav-link}
-   [14.1.3. Physical Memory/No Virtual Memory](#physical-memory-no-virtual-memory){.reference .internal .nav-link}
-   [14.1.4. Virtual Memory](#virtual-memory){.reference .internal .nav-link}
    -   [14.1.4.1. Segmented Virtual Memory](#segmented-virtual-memory){.reference .internal .nav-link}
    -   [14.1.4.2. Paged Virtual Memory](#paged-virtual-memory){.reference .internal .nav-link}
        -   [14.1.4.2.1. The virtual address space](#the-virtual-address-space){.reference .internal .nav-link}
        -   [14.1.4.2.2. Pros](#pros){.reference .internal .nav-link}
        -   [14.1.4.2.3. Cons](#cons){.reference .internal .nav-link}
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
