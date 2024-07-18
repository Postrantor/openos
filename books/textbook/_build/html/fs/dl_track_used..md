---
docsearch:language: en
lang: en
title: "22.2. Disk Layout:Tracking Used Space --- Introduction to Operating Systems"
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

- [19. Introduction](intro.html){.reference .internal}
- [20. File System Abstraction](interface.html){.reference .internal}
- [21. A bit about Disks](diskhw.html){.reference .internal}
- [22. Implementation](impl.html){.reference .internal}
  []{.toctree-toggle role="presentation"}
  - [22.1. File System Layout](disklayout.html){.reference .internal}
  - [22.2. Disk Layout:Tracking Used Space](#){.current .reference .internal}
  - [22.3. Disk Layout:Tracking Free Space](dl_track_free.html){.reference .internal}
  - [22.4. Disk Layout:Implementing Name Space](dl_name.html){.reference .internal}
  - [22.5. Disk Layout:Dealing with Failures](dl_failures.html){.reference .internal}
  - [22.6. Disk Layout:Examples of Real World File Systems](dl_ex_exx.html){.reference .internal}
  - [22.7. Kernel implementation](kernelimp.html){.reference .internal}
- [23. Review](review.html){.reference .internal}

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

- [[ ![JupyterHub logo](../_static/images/logo_jupyterhub.svg) ]{.btn__icon-container} [JupyterHub]{.btn__text-container}](https://jupyterhub-opf-jupyterhub.apps.smaug.na.operate-first.cloud/hub/user-redirect/git-pull?repo=https%3A//github.com/OpenOSOrg/openos&urlpath=lab/tree/openos/content/fs/dl_track_used.ipynb&branch=main "Launch on JupyterHub"){.btn .btn-sm .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
  :::

::: {.dropdown .dropdown-source-buttons}

- [[ ]{.btn__icon-container} [Repository]{.btn__text-container}](https://github.com/OpenOSOrg/openos "Source repository"){.btn .btn-sm .btn-source-repository-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
- [[ ]{.btn__icon-container} [Suggest edit]{.btn__text-container}](https://github.com/OpenOSOrg/openos/edit/main/content/fs/dl_track_used.ipynb "Suggest edit"){.btn .btn-sm .btn-source-edit-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
- [[ ]{.btn__icon-container} [Open issue]{.btn__text-container}](https://github.com/OpenOSOrg/openos/issues/new?title=Issue%20on%20page%20%2Ffs/dl_track_used.html&body=Your%20issue%20content%20here. "Open an issue"){.btn .btn-sm .btn-source-issues-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
  :::

::: {.dropdown .dropdown-download-buttons}

- [[ ]{.btn__icon-container} [.ipynb]{.btn__text-container}](../_sources/fs/dl_track_used.ipynb "Download source file"){.btn .btn-sm .btn-download-source-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}

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

# Disk Layout:Tracking Used Space

::: {#print-main-content}
::: {#jb-print-toc}

<div>

## Contents

</div>

- [22.2.1. Contiguous](#contiguous){.reference .internal .nav-link}
- [22.2.2. Linked list](#linked-list){.reference .internal .nav-link}
- [22.2.3. Inode](#inode){.reference .internal .nav-link}
- [22.2.4. Extents](#extents){.reference .internal .nav-link}
  :::
  :::
  :::

::: {#searchbox}
:::

::: {#disk-layout-tracking-used-space .section .tex2jax_ignore .mathjax_ignore}
[]{#fs-dl-track-used}

# [22.2. ] {.section-number}Disk Layout:Tracking Used Space[\#](#disk-layout-tracking-used-space "Link to this heading") {.headerlink}

The main job of the file system is to use the blocks on the disk to store persistent data for users in files, and to support the organization of those files into directories. Clearly, we will need a way for the file system to keep track of which blocks are being used for each file. In this Chapter, we will explore several options for this important design decision.

Note that in many (most? all?) file systems, directory objects (which hold file system metadata about the files in that directory) are stored exactly like files. Part of the information the file system keeps about each object is a type field, which allows the file system to distinguish file objects from directory objects. While the content of file objects is only understood by the applications that use them (above the file system), the content of directory objects is understood and managed by the file system itself. Everything we say here about techniques for keeping track of the blocks used by files also applies to the task of tracking blocks used by directories.

::: {#contiguous .section}
[]{#fs-dl-track-used-contig}

## [22.2.1. ] {.section-number}Contiguous[\#](#contiguous "Link to this heading") {.headerlink}

The simplest organization of a file system is to just have each file or directory occupy a contiguous set of blocks on the disk. For example, [[Fig. 22.3]{.std .std-numref}](#fs-cd-rom){.reference .internal} shows a structure similar to early versions of the ISO-9660 file system for CD-ROM disks. Objects on disk are either files or directories, each composed of one or more 2048-byte *blocks*; all pointers in the file system are in terms of *block numbers*, with blocks numbered from block 0 at the beginning of the disk or partition. Note that the `len`{.docutils .literal .notranslate} field in [[Fig. 22.3]{.std .std-numref}](#fs-cd-rom){.reference .internal} gives the file length in *bytes*, not blocks, but space in the file system must be allocated in block-sized chunks. The number of blocks used by the file can be calculated as the ceiling of the file size divided by the block size, i.e., [\\(\\lceil len / 2048 \\rceil\\)]{.math .notranslate .nohighlight} in this example.

![[Fig. 22.3 ]{.caption-number}[Simpliﬁed ISO-9660 (CDROM) ﬁle layout for tree in [[Fig. 20.1]{.std .std-numref}](interface.html#fs-tree-logical){.reference .internal}, 2 KB blocks]{.caption-text}[\#](#fs-cd-rom "Link to this image"){.headerlink}](../_images/filesys-cdrom.png){style="width: 40%;"}

The advantages of this approach are:

- Very dense meta-data, you can represent all the blocks used by a file system with one record having a starting block number and a length.
- Very fast reads, you only need to do one seek operation to get to all the blocks of any file on the disk.

Contiguous organization works fine for a read-only file system, where all files (and their sizes) are available when the file system is created. It, however, works poorly for writable file systems because:

- File system space becomes rapidly *fragmented*, making it impossible to create large files.
- There is no way to add information to a file without reading it and writing it as a new file. Appending to a file *may* be possible, if the blocks that follow the end of the file are not being used by another file, but in general this will not be the case.
  :::

::: {#linked-list .section}
[]{#fs-dl-track-used-ll}

## [22.2.2. ] {.section-number}Linked list[\#](#linked-list "Link to this heading") {.headerlink}

Another approach to keep track of the blocks used in a file is to maintain a linked list as shown in [[Fig. 22.4]{.std .std-numref}](#fig-filesys-linked){.reference .internal}. This approach doesn't have the external fragmentation challenge of contiguous files, because any available block can be used to add more data to any file by simply adding the block to the list.

The top part of [[Fig. 22.4]{.std .std-numref}](#fig-filesys-linked){.reference .internal} uses internal pointers in a block, where each block stores slightly less than a full block of data to make room for the pointer metadata. This approach might seem attractive, however, it is not practical for several reasons. First, to read the block containing data at a particular offset in a file, one has to read blocks sequentially through the entire linked list up to the required block. Second, mixing file data with file system metadata in the same block would add complexity to operating system features like memory-mapped files. We won't be in a position to explain why this is the case until we cover memory management, however. Finally, because the amount of data stored in a block is no longer a power of 2, calculating the block that contains a given offset will require integer division operations, rather than cheaper right-shift operations.

![[Fig. 22.4 ]{.caption-number}[Linked list organization with in-object pointers (typical for in-memory structures) and external pointers, as used in MS-DOS File Allocation Table.]{.caption-text}[\#](#fig-filesys-linked "Link to this image"){.headerlink}](../_images/filesys-linked.png){style="width: 40%;"}

An alternative (shown in the bottom of [[Fig. 22.4]{.std .std-numref}](#fig-filesys-linked){.reference .internal}) would store the pointers of the linked list in a separate array from the disk blocks themselves. This is used in the MS-DOS (or FAT, File Allocation Table) file system. Block numbers are kept in a separate array, with an entry corresponding to each disk block, in what is called the File Allocation Table.

Entries in this table can indicate (a) the number of the next block in the file or directory, (b) that the block is the last one in a file or (c) the block is free. The FAT is thus used for free space management as well as file organization; when a block is needed the table may be searched for a free entry which can then be allocated.

Access to a file incurs overhead to fetch file allocation table entries, although since these are frequently used they may be cached in memory; random access to a file, however, requires walking the linked list to find the corresponding entry, which can be slow even when cached in memory. However, if a file is distributed across the disk performance can be terrible. Consider random I/O within a 1 GB virtual disk image with 4 KB blocks---the linked list will have 256 K entries, and on average each I/O will require searching halfway through the list.
:::

::: {#inode .section}

## [22.2.3. ] {.section-number}Inode[\#](#inode "Link to this heading") {.headerlink}

File systems derived from the original Unix file system use a per-file structure called an inode to not only keep track of attributes, but also block locations. The inode uses an asymmetric tree, or actually a series of trees of increasing height with the root of each tree stored in the inode.

As seen in [[Fig. 22.5]{.std .std-numref}](#filesys-inode){.reference .internal} the inode contains N *direct* block pointers (12 in ext2/ext3), so that files of N blocks or less need no indirect blocks. A single *indirect pointer* specifies an *indirect block*, holding pointers to blocks [\\(N, N+1, \... N+N_1-1\\)]{.math .notranslate .nohighlight} where [\\(N_1\\)]{.math .notranslate .nohighlight} is the number of block numbers that fit in a file system block (1024 for ext2 with a 4 KB blocksize).

If necessary, the *double-indirect pointer* specifies a block holding pointers to [\\(N_1\\)]{.math .notranslate .nohighlight} indirect blocks, which in turn hold pointers to blocks [\\(N+N_1 \... N+N_1+N_1\^2-1\\)]{.math .notranslate .nohighlight}---i.e. an [\\(N_1\\)]{.math .notranslate .nohighlight}-ary tree of height 2; a triple indirect block in turn points to a tree of height 3.

For ext2 with 4-byte block numbers, if we use 4K blocks this gives a maximum file size of [\\((4096/4)\^3\\)]{.math .notranslate .nohighlight} 4 KB blocks, or 4.004 TB. This organization allows random access within a file with overhead [\\(O(logN)\\)]{.math .notranslate .nohighlight} where [\\(N\\)]{.math .notranslate .nohighlight} is the file size, which is vastly better than the [\\(O(N)\\)]{.math .notranslate .nohighlight} overhead of the MS-DOS File Access Table system.

![[Fig. 22.5 ]{.caption-number}[Inode-type file organization as found in many Unix file systems (e.g. Linux ext2, ext3)]{.caption-text}[\#](#filesys-inode "Link to this image"){.headerlink}](../_images/filesys-inode.png){style="width: 80%;"}

Inode structures are a reasonable compromise, they have (a) low overhead for small files, in terms of both disk seeks and allocated blocks, and (b) ability to represent sufficiently large files without excessive storage space or performance overhead.

![[Fig. 22.6 ]{.caption-number}[File structure---pointers]{.caption-text}[\#](#fig-fs-ext2layout "Link to this image"){.headerlink}](../_images/files-pointers.png){style="width: 200pt;"}
:::

::: {#extents .section}

## [22.2.4. ] {.section-number}Extents[\#](#extents "Link to this heading") {.headerlink}

The ext2 and MS-DOS file systems use separate pointers to every data block in a file, located in inodes and indirect blocks in the case of ext2, and in the File Allocation Table in MS-DOS. However, a well-designed file system will attempt to allocate blocks to files sequentially to avoid disk seeks ---if the first block in a file is block 100, it's highly likely that the second will be 101, the third 102, etc.

![[Fig. 22.7 ]{.caption-number}[File structure--- extents]{.caption-text}[\#](#fig-filesys-extent "Link to this image"){.headerlink}](../_images/files-extent.png){style="width: 200pt;"}

We can take advantage of this to greatly compress the information needed to identify the blocks in a file - rather than having separate pointers to blocks 100,101,...120 we just need to identify the starting block (100) and the length (21 blocks). This is shown in [[Fig. 22.6]{.std .std-numref}](#fig-fs-ext2layout){.reference .internal}, where five data blocks are identified by direct pointers in an inode. In [[Fig. 22.7]{.std .std-numref}](#fig-filesys-extent){.reference .internal}, the same five data blocks are identified by a single extent. Why would we want to compress the information needed to organize the blocks in a file? Mostly for performance---although the code is more complicated, it will require fewer disk seeks to read from disk.

This organization is the basis of *extent-based* file systems, where blocks in a file are identified via one or more *extents*, or (start,length) pairs. The inode (or equivalent) can contain space for a small number of extents; if the file grows too big, then you add the equivalent of indirect blocks - extents pointing to blocks holding more extents. Both Microsoft NTFS and Linux ext4 use this sort of extent structure.
:::
:::

::: prev-next-area
[](disklayout.html "previous page"){.left-prev}

::: prev-next-info
previous

[22.1. ]{.section-number}File System Layout
:::

[](dl_track_free.html "next page"){.right-next}

::: prev-next-info
next

[22.3. ]{.section-number}Disk Layout:Tracking Free Space
:::
:::
:::

::: {.bd-sidebar-secondary .bd-toc}
::: {.sidebar-secondary-items .sidebar-secondary__inner}
::: sidebar-secondary-item
::: {.page-toc .tocsection .onthispage}
Contents
:::

- [22.2.1. Contiguous](#contiguous){.reference .internal .nav-link}
- [22.2.2. Linked list](#linked-list){.reference .internal .nav-link}
- [22.2.3. Inode](#inode){.reference .internal .nav-link}
- [22.2.4. Extents](#extents){.reference .internal .nav-link}
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
