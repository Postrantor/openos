---
docsearch:language: en
lang: en
title: 13. Memory management before paged virtual memory --- Introduction to Operating Systems
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
- [13. Memory management before paged virtual memory](#){.current .reference .internal}
- [14. Paged Virtual memory](pagvm.html){.reference .internal}
  []{.toctree-toggle role="presentation"}
  - [14.1. Abstracting a useful interface for memory management.](vmabs.html){.reference .internal}
  - [14.2. Paging](virt-paging.html){.reference .internal}
  - [14.3. Page Tables](page-tables.html){.reference .internal}
  - [14.4. Memory reclaiming algorithms.](reclamation.html){.reference .internal}
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

- [[ ![JupyterHub logo](../_static/images/logo_jupyterhub.svg) ]{.btn__icon-container} [JupyterHub]{.btn__text-container}](https://jupyterhub-opf-jupyterhub.apps.smaug.na.operate-first.cloud/hub/user-redirect/git-pull?repo=https%3A//github.com/OpenOSOrg/openos&urlpath=lab/tree/openos/content/mm/phys-and-seg.ipynb&branch=main "Launch on JupyterHub"){.btn .btn-sm .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
  :::

::: {.dropdown .dropdown-source-buttons}

- [[ ]{.btn__icon-container} [Repository]{.btn__text-container}](https://github.com/OpenOSOrg/openos "Source repository"){.btn .btn-sm .btn-source-repository-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
- [[ ]{.btn__icon-container} [Suggest edit]{.btn__text-container}](https://github.com/OpenOSOrg/openos/edit/main/content/mm/phys-and-seg.ipynb "Suggest edit"){.btn .btn-sm .btn-source-edit-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
- [[ ]{.btn__icon-container} [Open issue]{.btn__text-container}](https://github.com/OpenOSOrg/openos/issues/new?title=Issue%20on%20page%20%2Fmm/phys-and-seg.html&body=Your%20issue%20content%20here. "Open an issue"){.btn .btn-sm .btn-source-issues-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
  :::

::: {.dropdown .dropdown-download-buttons}

- [[ ]{.btn__icon-container} [.ipynb]{.btn__text-container}](../_sources/mm/phys-and-seg.ipynb "Download source file"){.btn .btn-sm .btn-download-source-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}

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

# Memory management before paged virtual memory

::: {#print-main-content}
::: {#jb-print-toc}

<div>

## Contents

</div>

- [13.1. Simple physical memory management.](#simple-physical-memory-management){.reference .internal .nav-link}
- [13.2. Segmentation - Virtual Memory](#segmentation-virtual-memory){.reference .internal .nav-link}
  - [13.2.1. Segmentation - Base and Bounds translation](#segmentation-base-and-bounds-translation){.reference .internal .nav-link}
- [13.3. Segmentation(AKA base and bounds translation).](#segmentation-aka-base-and-bounds-translation){.reference .internal .nav-link}
  - [13.3.1. Single segments per address space](#single-segments-per-address-space){.reference .internal .nav-link}
  - [13.3.2. Multiple segments per address space.](#multiple-segments-per-address-space){.reference .internal .nav-link}
  - [13.3.3. Private versus Global segments.](#private-versus-global-segments){.reference .internal .nav-link}
    - [13.3.3.1. Fragmentation and Compaction.](#fragmentation-and-compaction){.reference .internal .nav-link}
    - [13.3.3.2. Swapping.](#swapping){.reference .internal .nav-link}
    - [13.3.3.3. Limitations of segmentation.](#limitations-of-segmentation){.reference .internal .nav-link}
      :::
      :::
      :::

::: {#searchbox}
:::

This chapter describes how memory management evolved from simple physical memory management to virtual memory using segmentation and why we now have paged virtual memory on most systems.

::: {#memory-management-before-paged-virtual-memory .section .tex2jax_ignore .mathjax_ignore}

# [13. ] {.section-number}Memory management before paged virtual memory[\#](#memory-management-before-paged-virtual-memory "Link to this heading") {.headerlink}

::: {#simple-physical-memory-management .section}
[]{#cont-mm-overview-simple}

## [13.1. ] {.section-number}Simple physical memory management.[\#](#simple-physical-memory-management "Link to this heading") {.headerlink}

From a hardware perspective, the simplest memory management model is to have processes just use the physical address space; where instructions executed on the processor directly reference physical memory addresses. For example, if the application wants to load a register, from location `0x1234`{.docutils .literal .notranslate} it would get the data stored at physical memory location `0x1234`{.docutils .literal .notranslate}. For example, the original Microsoft DOS operating system, supported exactly this model.

As shown in [[Fig. 13.1]{.std .std-numref}](#mem-pys-mem-fig){.reference .internal}, the operating system needs to be loaded into one part of the memory, and each program that you would want to run needs to be loaded into different physical memory at different addresses.

![[Fig. 13.1 ]{.caption-number}[Operating system is loaded at address 0, program 1 is loaded at address `0x2000`{.docutils .literal .notranslate} and program 2 is loaded at address `0x8000`{.docutils .literal .notranslate}]{.caption-text}[\#](#mem-pys-mem-fig "Link to this image"){.headerlink}](../_images/physmem.drawio.png){style="width: 50%;"}

There are two major problems with physical memory management. First, there is no protection between the different programs. A bug in program 1 may cause program 2 to be modified, or even modify the operating system.

Second, programs need to be re-located when they are loaded. If we are going to run multiple programs, we can't know a-priori the location where the program will be loaded. However, when the program is compiled and linked into object code specific addresses, for example for branches needed to be specified in the program.

For this reason programs are usually linked as relocatable. Relocatable programs have a table of all addresses within the program image that must be changed at load time before it can be run. See [[Fig. 13.2]{.std .std-numref}](#prog-pys-mem-fig){.reference .internal}, where the jump instruction at address `0x0000`{.docutils .literal .notranslate} needs to be modified by adding the address of where the program is being loaded, i.e., `JMP 0x1000`{.docutils .literal .notranslate} is modified to `JMP 0x3000`{.docutils .literal .notranslate}.

![[Fig. 13.2 ]{.caption-number}[Changes to program 1 to load it at address `0x2000`{.docutils .literal .notranslate}]{.caption-text}[\#](#prog-pys-mem-fig "Link to this image"){.headerlink}](../_images/prog_phys.drawio.png){style="width: 80%;"}

While we don't need relocation to solve this problem with paged virtual memory, as we will discuss layer, relocation is still used today for shared libraries and for address space randomization.
:::

::: {#segmentation-virtual-memory .section}
[]{#cont-mm-virt-seg}

## [13.2. ] {.section-number}Segmentation - Virtual Memory[\#](#segmentation-virtual-memory "Link to this heading") {.headerlink}

Physical memory managment has the 2 problems; there is no isolation and you need to relocate programs to wherever they are loaded. What we really want is *virtual memory* where every process has an address space that appears to start at address `0x0000`{.docutils .literal .notranslate} and ends at some large address based on underlying hardware design. This way every process is isolated from every other process because it can only see its own virtual memory and every program can be loaded at wherever it was linked to run without relocation.

![[Fig. 13.3 ]{.caption-number}[Multiple virtual address spaces using segmentation]{.caption-text}[\#](#multiple-virtual-address-spaces "Link to this image"){.headerlink}](../_images/programs_seg.png){style="width: 100%;"}

::: {#segmentation-base-and-bounds-translation .section}

### [13.2.1. ] {.section-number}Segmentation - Base and Bounds translation[\#](#segmentation-base-and-bounds-translation "Link to this heading") {.headerlink}

We first looked at direct physical addressing, where no matter which process is executing, the same address (e.g. 0x1000) refers to the same memory location. In addition we reviewed a very simple form of address translation, shown here in [[Fig. 13.5]{.std .std-numref}](#mm-base-bound){.reference .internal}

where base and bounds registers are used to relocate a section of the *virtual address space*---the addresses seen by the program, corresponding to values in the CPU registers---to somewhere else in the physical address space. By changing these translations the operating system can create multiple virtual address spaces, one per process; however there is still only one physical address space, uniquely identifying each byte in each memory chip. In this chapter we introduce *paged address translation*, a more complex address translation mechanism used by most modern CPUs, and present the 32-bit Intel implementation as an example.

![[Fig. 13.4 ]{.caption-number}[Base and Limit registers]{.caption-text}[\#](#b-l "Link to this image"){.headerlink}](../_images/B%26Lregs.png){style="width: 80%;"}
:::
:::

::: {#segmentation-aka-base-and-bounds-translation .section}

## [13.3. ] {.section-number}Segmentation(AKA base and bounds translation).[\#](#segmentation-aka-base-and-bounds-translation "Link to this heading") {.headerlink}

In the simplest form of segmentation the hardware provides 2 registers that are loaded each time a process acquire the CPU, a base register and a limit register. For a given process the base register contains the physical address that the program was loaded at and the limit register contains the size of the program that was loaded into memory. Every process has a virtual address space starting at zero and a size determined by the actual program size that the process is running. The process specific base and limit registers which are loaded every time a process acquires the CPU establishes the bounds of the virtual address space for every process. For each and every memory reference the hardware adds the virtual address to the base register to determine a physical address and insures that the physical address is between the base register and base register plus the limit register. If it is outside those bounds the program is terminated with an illegal virtual memory reference error. Segmentation solves both the lack of protection and the mandatory relocation requirements of physical addressing. Segmentation has little or no performance overhead because the hardware performs the virtual to physical translation or the addition of the virtual address and the base register to determine every physical address.

![[Fig. 13.5 ]{.caption-number}[Base-bound registers for translation]{.caption-text}[\#](#mm-base-bound "Link to this image"){.headerlink}](../_images/virt-mem-base-bounds.png){style="width: 45%;"}

::: {#single-segments-per-address-space .section}

### [13.3.1. ] {.section-number}Single segments per address space[\#](#single-segments-per-address-space "Link to this heading") {.headerlink}

So far we discussed a segmentation implementation that provides one base register and one limit register in hardware and one of each of those process specific values that gets loaded into those registers when context switching to a given process. Since there is only one of each register, the entire process virtual address space must be physically contiguous and all text, data and stack must be within that single memory region. While this is a huge improvement over a physical memory model it limits the size of the virtual address space to being static and not expandable. There is no way to dynamically increase the size of the text, data or stack regions of a process at run-time, everything must be allocated in advance. This requires allocating physical memory that might never be used.

![[Fig. 13.6 ]{.caption-number}[Single Segment per process]{.caption-text}[\#](#segment-ex1 "Link to this image"){.headerlink}](../_images/segment_ex1.png){style="width: 80%;"}

Since every process has different base and limit register values segmentation can easily support multiple processes.

![[Fig. 13.7 ]{.caption-number}[Multiple processes using Segmentation]{.caption-text}[\#](#segment-ex2 "Link to this image"){.headerlink}](../_images/segment_ex2.png){style="width: 80%;"}
:::

::: {#multiple-segments-per-address-space .section}

### [13.3.2. ] {.section-number}Multiple segments per address space.[\#](#multiple-segments-per-address-space "Link to this heading") {.headerlink}

As mentioned earlier a single base and limit segment register implies that an entire process virtual address space is a one physically contiguous region of physical memory mapped into one virtually contiguous virtual region of virtual memory. This means that the text, data and stack regions must be packed tightly together in both physical and virtual memory unless we are willing to waste both physical and virtual memory. Also, with only one segment register its not possible to offer different types of protections for the various regions of the virtual address space. In other words all of virtual memory must be readable, writable and executable since data must be both readable and writable and text must be executable. It would be nice to prevent data regions from being executable and text regions from being readable and writable for security and debug optimizations.

This can be achieved by the hardware implementing multiple segment and limit registers with only specified permissions for text, data and stack regions and having the operating system use those registers when context switching to a process. When mapping the text into a virtual region the operating system can specify an execute only region that does not have to be adjacent to other non-executable regions. When mapping data into virtual memory the operating system can specify read/write only thereby preventing execution of data regions. Finally the stack can also be non-executable but also the operating system can move the virtual memory stack region away from any other region making it easier to debug common programming problems like stack overflows. Finally multiple segment registers eliminates the necessity for the text, data and stack regions to be physically contiguous. This allows a program to be split up into multiple smaller regions both physically and virtually making it much easier to hold more programs in physical memory at the same time.

![[Fig. 13.8 ]{.caption-number}[Multiple Segments per address space]{.caption-text}[\#](#segment-multi "Link to this image"){.headerlink}](../_images/segmentation-multi.png){style="width: 80%;"}
:::

::: {#private-versus-global-segments .section}

### [13.3.3. ] {.section-number}Private versus Global segments.[\#](#private-versus-global-segments "Link to this heading") {.headerlink}

Every process virtual address space consists of 2 types of regions, Private and Global. The private regions for a process are the program specific text, data and stack regions that the process is running. The global regions include the operating system that is and must be mapped into every process address space. As we discussed earlier in this course the operating system consists of all the software that executes on behalf of the currently running program as well as basic system overhead that runs on behalf of the system. This includes all the system calls the operating system supports. Since every process must map the operating system kernel it is shared between every running process rather than each process containing a separate copy. The global segment registers are used to map the shared kernel text, data and kernel stack area in every process and at the same virtual addresses. When a context switch occurs only the private segments registers are changed for the newly running process, there is no need to change the global segment registers since they are identical for every process.

![[Fig. 13.9 ]{.caption-number}[Global Segments]{.caption-text}[\#](#segment-global "Link to this image"){.headerlink}](../_images/segmentation-global.png){style="width: 80%;"}

::: {#fragmentation-and-compaction .section}

#### [13.3.3.1. ] {.section-number}Fragmentation and Compaction.[\#](#fragmentation-and-compaction "Link to this heading") {.headerlink}

When a new process is created and a program runs the kernel reads the program text, data and stack memory into the available or free physical memory locations. From there the private segment registers are use to map that physical memory into the private virtual address space of the process, allowing the process to run the program. When a process exits, the physical memory regions that the process consumed is made available or freed onto a physical memory free list. Over time as processes are created, run and exit the physical memory becomes more and more fragmented. After a while as processes come and go its likely that the sum of available physical memory is large enough to satisfy a request but there is no physically contiguous free memory region large enough to hold the request.

For example if memory is allocated and de-allocated in chunks of different sizes and at different times, then it can become *fragmented* so that even if large amounts of memory are free, it will be divided into smaller fragments, separated by longer-lived small allocations, as seen in (#fig:vm:fig2).

Start: 32 locations, all free

![[Fig. 13.10 ]{.caption-number}[Everything is free]{.caption-text}[\#](#mm-virt-mem-frag-1 "Link to this image"){.headerlink}](../_images/virt-mem-frag-1.png){style="width: 45%;"}

Step 1, 2: Load and run processes A and B

![[Fig. 13.11 ]{.caption-number}[Process A allocates 10 and process B allocates 1]{.caption-text}[\#](#mm-virt-mem-frag-2 "Link to this image"){.headerlink}](../_images/virt-mem-frag-2.png){style="width: 45%;"}

Step 3, 4, 5: Run and load processes C, D and E.

![[Fig. 13.12 ]{.caption-number}[Process C allocates 10, process D allocates 1 and process E allocates 10]{.caption-text}[\#](#mm-virt-mem-frag-3 "Link to this image"){.headerlink}](../_images/virt-mem-frag-3.png){style="width: 45%;"}

Steps 6, 7, 8: processes A, C and D terminate

![[Fig. 13.13 ]{.caption-number}[process A frees 10, process C frees 1 and process E frees 10]{.caption-text}[\#](#mm-virt-mem-frag-4 "Link to this image"){.headerlink}](../_images/virt-mem-frag-4.png){style="width: 45%;"}

In the last line, you can see that only 2 units of memory (out of 32) remain allocated, but the largest amount that can be allocated at one time is 10 units. If all allocation requests are small, this might not be a problem; however, in an operating system it is common to have one or two very large processes (e.g., a web browser and word processing software), and many small, long-running processes (e.g., the on-screen battery display or wifi signal strength indicator). In this case, large memory allocations may fail, even when there is enough total memory free, because long-lived small allocations fragment the available contiguous memory into smaller pieces.

When this happens the operating system must move or coalesce the used memory regions together thereby creating a large contiguous available or free region. Even though this is very time consuming and not desirable at least now one or more requests can be satisfied. This is all made possible because the base registers of the processes that map these moved regions can be updated to the new locations of the physical memory and because the operating system has the ability to relocate programs in physical memory as we discussed in the physical memory management model. Again, this is time consuming and undesirable.
:::

::: {#swapping .section}

#### [13.3.3.2. ] {.section-number}Swapping.[\#](#swapping "Link to this heading") {.headerlink}

Since the entire process must be resident in physical memory to run with segmentation, its unlikely that all processes will be able to run at the same time. In order to support more processes than can fit into memory the memory management system must swap entire processes out to disk when memory is needed and into memory from disk when they need to run again.

The memory management system has determined that process 1 had run long enough so it swaps it out and frees up memory it occupies.

![[Fig. 13.14 ]{.caption-number}[Swapping out an entire process]{.caption-text}[\#](#swapout "Link to this image"){.headerlink}](../_images/swapout.png){style="width: 80%;"}

The memory management system has determined that its time for process N to run again so it swaps it into the memory freed by the swapout.

![[Fig. 13.15 ]{.caption-number}[Swapping in an entire process]{.caption-text}[\#](#swapin "Link to this image"){.headerlink}](../_images/swapin.png){style="width: 80%;"}
:::

::: {#limitations-of-segmentation .section}

#### [13.3.3.3. ] {.section-number}Limitations of segmentation.[\#](#limitations-of-segmentation "Link to this heading") {.headerlink}

Segmentation, especially with multiple segment registers along with private and global segment registers provides a huge benefit over a physical memory management model. We can now support many processes running at the same time with protection between processes and even protection within a process. However Segmentation still has major weaknesses, 1.) the memory for a segment must be physically contiguous, 2.) the virtual address size can never exceed the physical address size with segmentation. Needing physically contiguous memory is a huge problem, it requires compaction and swapping in order to run a significant number of processes simultaneously. Limiting programs to less that the amount of physical memory on a given system is also very limiting. It would be very convenient to be able to allocate a very large sparse region of virtual memory and only actually use a small subset of it. Imagine allocating an array of fixed size records for every possible student at Boston University and indexing that array by the student's social security number. There are 10\^9 or 1 Billion social security numbers but only a few thousand students at BU. Such a large sparse array could not be implemented with segmentation unless the system actually had all the necessary physical memory for every possible social security number. Imagine being able to map millions of files in a virtual address space on a system that didn't have all that much physical memory.
:::
:::
:::
:::

::: prev-next-area
[](intro.html "previous page"){.left-prev}

::: prev-next-info
previous

[12. ]{.section-number}Introduction
:::

[](pagvm.html "next page"){.right-next}

::: prev-next-info
next

[14. ]{.section-number}Paged Virtual memory
:::
:::
:::

::: {.bd-sidebar-secondary .bd-toc}
::: {.sidebar-secondary-items .sidebar-secondary__inner}
::: sidebar-secondary-item
::: {.page-toc .tocsection .onthispage}
Contents
:::

- [13.1. Simple physical memory management.](#simple-physical-memory-management){.reference .internal .nav-link}
- [13.2. Segmentation - Virtual Memory](#segmentation-virtual-memory){.reference .internal .nav-link}
  - [13.2.1. Segmentation - Base and Bounds translation](#segmentation-base-and-bounds-translation){.reference .internal .nav-link}
- [13.3. Segmentation(AKA base and bounds translation).](#segmentation-aka-base-and-bounds-translation){.reference .internal .nav-link}
  - [13.3.1. Single segments per address space](#single-segments-per-address-space){.reference .internal .nav-link}
  - [13.3.2. Multiple segments per address space.](#multiple-segments-per-address-space){.reference .internal .nav-link}
  - [13.3.3. Private versus Global segments.](#private-versus-global-segments){.reference .internal .nav-link}
    - [13.3.3.1. Fragmentation and Compaction.](#fragmentation-and-compaction){.reference .internal .nav-link}
    - [13.3.3.2. Swapping.](#swapping){.reference .internal .nav-link}
    - [13.3.3.3. Limitations of segmentation.](#limitations-of-segmentation){.reference .internal .nav-link}
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
