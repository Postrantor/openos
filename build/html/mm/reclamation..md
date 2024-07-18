---
docsearch:language: en
lang: en
title: 14.4. Memory reclaiming algorithms. --- Introduction to Operating Systems
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
  - [14.4. Memory reclaiming algorithms.](#){.current .reference .internal}
  - [14.5. Page Sizes](page-size.html){.reference .internal}
  - [14.6. Memory Management Page Faults](pagefaults.html){.reference .internal}
- [15. Buffer Cache](buffer-cache.html){.reference .internal}
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

- [[ ![JupyterHub logo](../_static/images/logo_jupyterhub.svg) ]{.btn__icon-container} [JupyterHub]{.btn__text-container}](https://jupyterhub-opf-jupyterhub.apps.smaug.na.operate-first.cloud/hub/user-redirect/git-pull?repo=https%3A//github.com/OpenOSOrg/openos&urlpath=lab/tree/openos/content/mm/reclamation.ipynb&branch=main "Launch on JupyterHub"){.btn .btn-sm .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
  :::

::: {.dropdown .dropdown-source-buttons}

- [[ ]{.btn__icon-container} [Repository]{.btn__text-container}](https://github.com/OpenOSOrg/openos "Source repository"){.btn .btn-sm .btn-source-repository-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
- [[ ]{.btn__icon-container} [Suggest edit]{.btn__text-container}](https://github.com/OpenOSOrg/openos/edit/main/content/mm/reclamation.ipynb "Suggest edit"){.btn .btn-sm .btn-source-edit-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
- [[ ]{.btn__icon-container} [Open issue]{.btn__text-container}](https://github.com/OpenOSOrg/openos/issues/new?title=Issue%20on%20page%20%2Fmm/reclamation.html&body=Your%20issue%20content%20here. "Open an issue"){.btn .btn-sm .btn-source-issues-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
  :::

::: {.dropdown .dropdown-download-buttons}

- [[ ]{.btn__icon-container} [.ipynb]{.btn__text-container}](../_sources/mm/reclamation.ipynb "Download source file"){.btn .btn-sm .btn-download-source-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}

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

# Memory reclaiming algorithms.

::: {#print-main-content}
::: {#jb-print-toc}

<div>

## Contents

</div>

- [14.4.1. The Memory Hierarchy](#the-memory-hierarchy){.reference .internal .nav-link}
- [14.4.2. Dirty and Clean Pages](#dirty-and-clean-pages){.reference .internal .nav-link}
- [14.4.3. Page Replacement](#page-replacement){.reference .internal .nav-link}
- [14.4.4. Page Replacement Strategies](#page-replacement-strategies){.reference .internal .nav-link}
  - [14.4.4.1. FIFO](#fifo){.reference .internal .nav-link}
  - [14.4.4.2. LRU](#lru){.reference .internal .nav-link}
  - [14.4.4.3. OPT](#opt){.reference .internal .nav-link}
  - [14.4.4.4. FIFO with Second Chance (CLOCK)](#fifo-with-second-chance-clock){.reference .internal .nav-link}
  - [14.4.4.5. CLOCK](#clock){.reference .internal .nav-link}
    :::
    :::
    :::

::: {#searchbox}
:::

This chapter describes various page replacement algorithms and how the referenced and dirty bits in the PTE are used.

::: {#memory-reclaiming-algorithms .section .tex2jax_ignore .mathjax_ignore}

# [14.4. ] {.section-number}Memory reclaiming algorithms.[\#](#memory-reclaiming-algorithms "Link to this heading") {.headerlink}

- Global page reclaiming

  - FIFO, LRU, NRU...
- Local page reclaiming

  - Reclaiming within a specific address space
- Working set page reclaiming

::: {#the-memory-hierarchy .section}

## [14.4.1. ] {.section-number}The Memory Hierarchy[\#](#the-memory-hierarchy "Link to this heading") {.headerlink}

Demand paging from files and from swap provides the mechanisms to create the traditional memory hierarchy, as shown in [[Fig. 14.15]{.std .std-numref}](#fig-vm-pic108){.reference .internal}.

---

![[Fig. 14.15 ]{.caption-number}[4-level Memory Hierarchy]{.caption-text}[\#](#fig-vm-pic108 "Link to this image"){.headerlink}](../_images/virt-mem-pic108.png){style="width: 45%;"}

To access address A:

1.) If it's not in the cache, then the old cache line is evicted, and A is loaded into the resulting empty cache line, this is done in hardware.

2.) If it's not in memory, then the old page is evicted, and the page containing A is loaded into the resulting empty page, this is done in software.

3.) This page is mapped into the faulting virtual page via the page table entry, this is done in software.

In general, this works because of *locality*: when a cache line is brought in from memory, a page is loaded into in memory from disk, etc., it tends to get accessed multiple times before eviction.

Decades ago this was used to run programs much bigger than physical memory---CPUs were slow and disks were almost as fast as they are today, so the relative overhead of paging infrequently-used data to disk was low. Today's CPUs are thousands of times faster, while disks are only a few times faster, and virtual memory doesn't seem like such a great idea anymore. However it still gets used, even on desktop and laptop systems, to "steal" memory from idle programs: if you leave a large program like Chrome or Microsoft Word idle for half an hour while you use another memory-hungry program, memory will be released from the idle process and given to the active one; if you switch back, the original program will run slowly for a while as it swaps these pages back in.
:::

::: {#dirty-and-clean-pages .section}

## [14.4.2. ] {.section-number}Dirty and Clean Pages[\#](#dirty-and-clean-pages "Link to this heading") {.headerlink}

How does the operating system determine whether a page has been modified and needs to be written to disk? It uses the D bit in the page table entry for this, as seen in [[Fig. 14.4]{.std .std-numref}](virt-paging.html#fig-vm-pic106){.reference .internal}. When a page is mapped in the page table, the D bit in the PTE is set to zero; when the CPU writes to a page with D = 0, the MMU re-writes the page table entry with D = 1. When the OS decides to evict a page, the D bit tells it whether the page is "clean," i.e., it hasn't been modified, or whether it is "dirty" and has to be written back to disk.

When the OS is paging in from a file (e.g. executable code), it is straightforward to find the data to read in, as there is a direct mapping between a range of pages in a specific file and corresponding pages in the virtual memory space. This correspondence can easily be stored in the definition of that virtual address segment. When pages are saved to swap space this doesn't work, however, as the locations they are saved to are allocated dynamically and fairly arbitrarily.

This problem is solved by using the page table itself. After evicting a page, its page table entry is invalidated by setting P = 0; however, the other 31 bits of the entry are ignored by the MMU. These bits are used to store the location of the page in swap space, so it can be found later later at page fault time. Thus, the page table entry does dual duty: when the page is present it points to the physical page itself, and is interpreted by the MMU; otherwise, it points to a location in swap space, and is ignored by the MMU and used by the software page fault handler.
:::

::: {#page-replacement .section}

## [14.4.3. ] {.section-number}Page Replacement[\#](#page-replacement "Link to this heading") {.headerlink}

If there's a limited amount of memory available, then every time a page is swapped in from disk, it will be necessary to remove, or evict, another page from memory. The choice of which page to evict is important: the best page to choose would be one that won't be needed anymore, while the worst page to evict would be one of the next to be used. (in that case, paging it back in would force another page to be evicted, and the work of paging it out and back in again would be wasted.) In fact, replacement of items in a cache is a general problem in computer systems; examples include:

- Cache line replacement in the hardware CPU cache
- Entry replacement in the TLB
- Buffer replacement in a file system buffer pool
- Page replacement in virtual memory

The page replacement problem can be stated in abstract form:

Given the following:

- A disk holding [\\(d\\)]{.math .notranslate .nohighlight} (virtual) pages, with virtual addresses [\\(0,\\ldots d-1\\)]{.math .notranslate .nohighlight};
- A memory [\\({M}\\)]{.math .notranslate .nohighlight} consisting of [\\(m\\)]{.math .notranslate .nohighlight} (physical) pages, where each page is either empty or holds one of the [\\(d\\)]{.math .notranslate .nohighlight} virtual pages, and
- An access pattern [\\(a_1, a_2, a_3, \\cdots\\)]{.math .notranslate .nohighlight} where each [\\(a_i\\)]{.math .notranslate .nohighlight} is a virtual address in the range [\\((0,d-1)\\)]{.math .notranslate .nohighlight}:

a demand-paging strategy is an algorithm which for each access [\\(a_i\\)]{.math .notranslate .nohighlight} does the following:

- If [\\(a_i\\)]{.math .notranslate .nohighlight} is already in one of the [\\(m\\)]{.math .notranslate .nohighlight} physical pages in [\\({M}\\)]{.math .notranslate .nohighlight} (i.e. a *hit*): do nothing
- Otherwise (a miss) it must:
- Select a physical page [\\(j\\)]{.math .notranslate .nohighlight} in [\\({M}\\)]{.math .notranslate .nohighlight} (holding some virtual address [\\(M_j\\)]{.math .notranslate .nohighlight}) and evict it, then
- Fetch virtual page [\\(a_i\\)]{.math .notranslate .nohighlight} from disk into physical page [\\(j\\)]{.math .notranslate .nohighlight}

In other words it only fetches page [\\(j\\)]{.math .notranslate .nohighlight} *on demand*---i.e. in response to a request for it.
:::

::: {#page-replacement-strategies .section}

## [14.4.4. ] {.section-number}Page Replacement Strategies[\#](#page-replacement-strategies "Link to this heading") {.headerlink}

In this class we consider the following page replacement strategies:

- FIFO: *first-in first-out*. The page evicted from memory is the first page to have been fetched into memory.
- LRU: *least-recently used*. Here, accesses to each page are tracked after it has been loaded into memory, and the least-recently-used page is evicted (unsurprisingly, given the name of the strategy).
- OPT: this is the optimal demand-paged strategy, which is simple but impossible to implement, since it requires knowledge of the future. It's examined because it provides a way of telling how well a real replacement strategy is performing---is it close to OPT, or is it far worse?

::: {#fifo .section}

### [14.4.4.1. ] {.section-number}FIFO[\#](#fifo "Link to this heading") {.headerlink}

![[Fig. 14.16 ]{.caption-number}[Example of first-in-first-out (FIFO) page replacement]{.caption-text}[\#](#fig-vm-pic107 "Link to this image"){.headerlink}](../_images/virt-mem-pic107.png){style="width: 100%;"}

This strategy is very simple to implement, as it only requires keeping track of the order in which pages were fetched into memory. Given 4 pages in physical memory, and the following access pattern:

1 2 3 4 2 1 3 4 5 4 1 2 5 6 3 2 5 2 3 6

The contents of memory after each access is shown in [[Fig. 14.16]{.std .std-numref}](#fig-vm-pic107){.reference .internal}, with hits shown in light grey and pages evicted (when misses occur) shown in dark grey.
:::

::: {#lru .section}

### [14.4.4.2. ] {.section-number}LRU[\#](#lru "Link to this heading") {.headerlink}

![[Fig. 14.17 ]{.caption-number}[Example of least-recently-used (LRU) page replacement]{.caption-text}[\#](#fig-vm-pic109 "Link to this image"){.headerlink}](../_images/virt-mem-pic109.png){style="width: 100%;"}

The idea behind LRU is that pages which have been accessed in the recent past are likely to be accessed in the near future, and pages which haven't, aren't. LRU replacement is shown in [[Fig. 14.17]{.std .std-numref}](#fig-vm-pic109){.reference .internal}.

To make the operation of the LRU algorithm more clear, on each hit, the accessed page is moved to the top of the column. (This is how LRU is typically implemented in software: elements are kept in a list, and on access, an element is removed and reinserted at the front of the list. The least-recently-used element may then be found by taking the tail of the list) Although this is a small example, a performance improvement is noted, with four misses compared to six for FIFO.
:::

::: {#opt .section}

### [14.4.4.3. ] {.section-number}OPT[\#](#opt "Link to this heading") {.headerlink}

![[Fig. 14.18 ]{.caption-number}[Example of the optimal algorithm for page replacement]{.caption-text}[\#](#fig-vm-pic110 "Link to this image"){.headerlink}](../_images/virt-mem-pic110.png){style="width: 100%;"}

The optimal algorithm picks a page to evict by looking forward in time and finding the page which goes for the longest time without being accessed again. Except for seeing the future, OPT plays by the same rules as other demand-paging algorithms: in particular, it can't fetch a page until it is accessed. (That's why the OPT strategy still has misses.) OPT is shown in [[Fig. 14.18]{.std .std-numref}](#fig-vm-pic110){.reference .internal}, using the same access pattern as before. The first eviction decision is shown graphically: pages 4, 2, and 1 are accessed 1, 3, and 2 steps in the future, respectively, while page 3 isn't accessed for 6 steps and is thus chosen to be evicted.
:::

::: {#fifo-with-second-chance-clock .section}

### [14.4.4.4. ] {.section-number}FIFO with Second Chance (CLOCK)[\#](#fifo-with-second-chance-clock "Link to this heading") {.headerlink}

![[Fig. 14.19 ]{.caption-number}[Example of FIFO with second chance]{.caption-text}[\#](#fig-vm-pic111 "Link to this image"){.headerlink}](../_images/virt-mem-pic111.png){style="width: 100%;"}

LRU is simple and quite effective in many caching applications, and it's ideal that the operating system uses it to determine which pages to evict from memory. But there is one small problem in using it in a virtual memory system: in this case, a "miss" corresponds to a page fault and fetching a page from disk, while a "hit" is when the page is already mapped in memory and the access succeeds in hardware. This means that once a page is faulted into memory, any further use of that page is "invisible" to the operating system. If the OS doesn't know when a page was last used, it can't implement the Least-Recently-Used replacement strategy.

Despite this issue, it's still possible to do better than FIFO by using the A ("accessed") bit in the page table entry, which indicates whether the page has been accessed since the last time the bit was cleared\[\^18\]. In [[Fig. 14.19]{.std .std-numref}](#fig-vm-pic111){.reference .internal} we see an algorithm called "FIFO with second chance," where the A bit is used to determine whether a page has been accessed while it was in the FIFO queue. If the A bit is 1, the replacement algorithm clears it and re-writes the page table entry, and the page is given "another chance," i.e., it is cycled back to the head of the list. If the A bit is 0, then there have been no accesses to the page during its entire trip through the list, and so it is selected for replacement.
:::

::: {#clock .section}

### [14.4.4.5. ] {.section-number}CLOCK[\#](#clock "Link to this heading") {.headerlink}

![[Fig. 14.20 ]{.caption-number}[Example of the CLOCK algorithm for page replacement]{.caption-text}[\#](#fig-vm-pic112 "Link to this image"){.headerlink}](../_images/virt-mem-pic112.png){style="width: 100%;"}

An alternate way of visualizing the FIFO with second chance algorithm is shown in [[Fig. 14.20]{.std .std-numref}](#fig-vm-pic112){.reference .internal}. Pages are arranged in a circle, with a "hand" advancing around the circle testing pages and determining whether to keep or evict them. This description is the origin of the widely-used name for this algorithm, CLOCK.
:::
:::
:::

::: prev-next-area
[](page-tables.html "previous page"){.left-prev}

::: prev-next-info
previous

[14.3. ]{.section-number}Page Tables
:::

[](page-size.html "next page"){.right-next}

::: prev-next-info
next

[14.5. ]{.section-number}Page Sizes
:::
:::
:::

::: {.bd-sidebar-secondary .bd-toc}
::: {.sidebar-secondary-items .sidebar-secondary__inner}
::: sidebar-secondary-item
::: {.page-toc .tocsection .onthispage}
Contents
:::

- [14.4.1. The Memory Hierarchy](#the-memory-hierarchy){.reference .internal .nav-link}
- [14.4.2. Dirty and Clean Pages](#dirty-and-clean-pages){.reference .internal .nav-link}
- [14.4.3. Page Replacement](#page-replacement){.reference .internal .nav-link}
- [14.4.4. Page Replacement Strategies](#page-replacement-strategies){.reference .internal .nav-link}
  - [14.4.4.1. FIFO](#fifo){.reference .internal .nav-link}
  - [14.4.4.2. LRU](#lru){.reference .internal .nav-link}
  - [14.4.4.3. OPT](#opt){.reference .internal .nav-link}
  - [14.4.4.4. FIFO with Second Chance (CLOCK)](#fifo-with-second-chance-clock){.reference .internal .nav-link}
  - [14.4.4.5. CLOCK](#clock){.reference .internal .nav-link}
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
