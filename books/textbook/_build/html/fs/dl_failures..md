---
docsearch:language: en
lang: en
title: "22.5. Disk Layout:Dealing with Failures --- Introduction to Operating Systems"
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
  - [22.2. Disk Layout:Tracking Used Space](dl_track_used.html){.reference .internal}
  - [22.3. Disk Layout:Tracking Free Space](dl_track_free.html){.reference .internal}
  - [22.4. Disk Layout:Implementing Name Space](dl_name.html){.reference .internal}
  - [22.5. Disk Layout:Dealing with Failures](#){.current .reference .internal}
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

- [[ ![JupyterHub logo](../_static/images/logo_jupyterhub.svg) ]{.btn__icon-container} [JupyterHub]{.btn__text-container}](https://jupyterhub-opf-jupyterhub.apps.smaug.na.operate-first.cloud/hub/user-redirect/git-pull?repo=https%3A//github.com/OpenOSOrg/openos&urlpath=lab/tree/openos/content/fs/dl_failures.ipynb&branch=main "Launch on JupyterHub"){.btn .btn-sm .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
  :::

::: {.dropdown .dropdown-source-buttons}

- [[ ]{.btn__icon-container} [Repository]{.btn__text-container}](https://github.com/OpenOSOrg/openos "Source repository"){.btn .btn-sm .btn-source-repository-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
- [[ ]{.btn__icon-container} [Suggest edit]{.btn__text-container}](https://github.com/OpenOSOrg/openos/edit/main/content/fs/dl_failures.ipynb "Suggest edit"){.btn .btn-sm .btn-source-edit-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
- [[ ]{.btn__icon-container} [Open issue]{.btn__text-container}](https://github.com/OpenOSOrg/openos/issues/new?title=Issue%20on%20page%20%2Ffs/dl_failures.html&body=Your%20issue%20content%20here. "Open an issue"){.btn .btn-sm .btn-source-issues-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
  :::

::: {.dropdown .dropdown-download-buttons}

- [[ ]{.btn__icon-container} [.ipynb]{.btn__text-container}](../_sources/fs/dl_failures.ipynb "Download source file"){.btn .btn-sm .btn-download-source-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}

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

# Disk Layout:Dealing with Failures

::: {#print-main-content}
::: {#jb-print-toc}

<div>

## Contents

</div>

- [22.5.1. Consistency and Journaling](#consistency-and-journaling){.reference .internal .nav-link}
- [22.5.2. Journaling](#journaling){.reference .internal .nav-link}
- [22.5.3. Log-Structured File Systems](#log-structured-file-systems){.reference .internal .nav-link}
  :::
  :::
  :::

::: {#searchbox}
:::

::: {#disk-layout-dealing-with-failures .section .tex2jax_ignore .mathjax_ignore}
[]{#fs-dl-failures}

# [22.5. ] {.section-number}Disk Layout:Dealing with Failures[\#](#disk-layout-dealing-with-failures "Link to this heading") {.headerlink}

::: {#consistency-and-journaling .section}

## [22.5.1. ] {.section-number}Consistency and Journaling[\#](#consistency-and-journaling "Link to this heading") {.headerlink}

Unlike in-memory structures, data structures on disk must survive system crashes, whether due to hardware reasons (e.g., power failure) or software failures. The problem is compounded by the fact that operating systems typically cache reads and writes to increase performance, so that writes to the disk may occur in a much different order than that in which they were issued by the file system code.

In its simplest form, the problem is that file system operations often involve writing to multiple disk blocks---for example, moving a file from one directory to another requires writing to blocks in the source and destination directories, while creating a file writes to the block and inode allocation bitmaps, the new inode, the directory block, and the file data block or blocks[[\[]{.fn-bracket}1[\]]{.fn-bracket}](#steps){#id1 .footnote-reference .brackets role="doc-noteref"}. If some, but not all, of these writes occur before a crash, the file system may become *inconsistent*---i.e. in a state not achievable through any legal sequence of file system operations, where some operations may return improper data or cause data loss.

![[Fig. 22.12 ]{.caption-number}[File, directory, bitmap]{.caption-text}[\#](#fig-delete-vicious "Link to this image"){.headerlink}](../_images/files-corruption.png){style="width: 200pt;"}

For a particularly vicious example, consider deleting the file `/a/b`{.docutils .literal .notranslate} as shown in [[Fig. 22.12]{.std .std-numref}](#fig-delete-vicious){.reference .internal}, which requires the following actions:

1. Clear the directory entry for /a/b. This is done by marking the entry as unused and writing its block back to the directory.
2. Free the file data block, by clearing the corresponding entry in the block allocation bitmap

![[Fig. 22.13 ]{.caption-number}[Directory block written before crash]{.caption-text}[\#](#id3 "Link to this image"){.headerlink}](../_images/files-failure-case1.png){style="width: 200pt;"}

This results in two disk blocks being modified and written back to disk; if the blocks are cached and written back at a later point in time they may be written to disk in any order. (This doesn't matter for running programs, as when they access the file system the OS will check cached data before going to disk.)

If the system crashes (e.g., due to a power failure) after one of these blocks has been written to disk, but not the other, two cases are possible:

1. The directory block is written, but not the bitmap. The file is no longer accessible, but the block is still marked as in use. This is a disk space leak (like a memory leak), resulting in a small loss of disk space but no serious problems.
2. The bitmap block is written, but not the directory. Applications are still able to find the file, open it, and write to it, but the block is also available to be allocated to a new file or directory. This is much more serious.

If the same block is re-allocated for a new file (`/a/c`{.docutils .literal .notranslate} in this case), we now have two files sharing the same data block, which is obviously a problem. If an application writes to `/a/b`{.docutils .literal .notranslate} it will also overwrite any data in `/a/c`{.docutils .literal .notranslate}, and vice versa. If `/a/c`{.docutils .literal .notranslate} is a directory rather than a file things are even worse---a write to `/a/b`{.docutils .literal .notranslate} will wipe out directory entries, causing files pointed to by those entries to be lost. (The files themselves won't be erased, but without directory entries pointing to them there won't be any way for a program to access them.)

![[Fig. 22.14 ]{.caption-number}[Bitmap block written before crash]{.caption-text}[\#](#fig-delete-vicious2 "Link to this image"){.headerlink}](../_images/files-failure-case2.png){style="width: 200pt;"}

This can be prevented by writing blocks in a specific order---for instance, in this case the directory entry could always be cleared before the block is marked as free, as shown in [[Fig. 22.15]{.std .std-numref}](#fig-syncwrites){.reference .internal}, so that in the worst case a crash might cause a few data blocks to become unusable. Unfortunately, this is very slow, as these writes must be done synchronously, waiting for each write to complete before issuing the next one.

![[Fig. 22.15 ]{.caption-number}[Synchronous disk writes for ext2 consistency.]{.caption-text}[\#](#fig-syncwrites "Link to this image"){.headerlink}](../_images/files-syncwrite.png){style="width: 70%;"}

**Fsck / chkdsk**: An alternative to the overhead of synchronous file system writes is to allow the OS to write blocks back to disk in any order, but detect and recover from any inconsistencies that occur due to an untimely crash. One way to do this is to run a disk checking routine every time the system boots after a crash. Earlier in [[Section 22.1]{.std .std-numref}](disklayout.html#cont-fs-layout){.reference .internal} we mentioned the file system superblock contained information to help with recovery. In particular, the superblock contains a *dirty* flag, which is set to **true** when the file system is mounted, and set to **false** when the file system is cleanly unmounted. In both cases, these changes to the superblock dirty flag are written to disk. When a machine boots, or a file system is mounted later, if the file system is marked dirty, `fsck`{.docutils .literal .notranslate} (or `chkdsk`{.docutils .literal .notranslate} in Windows) is run to repair any problems.

In particular, the Unix file system checker performs the following checks and corrections:

1. Blocks and sizes. Each allocated inode is checked to see that (a) the number of blocks reachable through direct and indirect pointers is consistent with the file size in the inode, (b) all block pointers are within the valid range for the volume, and (c) no blocks are referenced by more than one inode.
2. Pathnames. The directory tree is traversed from the root, and each entry is checked to make sure that it points to a valid inode of the same type (directory / file / device) as indicated in the entry.
3. Connectivity. Verifies that all directory inodes are reachable from the root.
4. Reference counts. Each inode holds a count of how many directory entries (hard links) are pointing to it. This step validates that count against the count determined by traversing the directory tree, and fixes it if necessary.
5. "Cylinder Groups". The block and inode bitmaps are checked for consistency. In particular, are all blocks and inodes reachable from the root marked in use, and all unreachable ones marked free?
6. "Salvage Cylinder Groups". Free inode and block bitmaps are updated to fix any discrepancies.

This is a lot of work, and involves a huge number of disk seeks. On a large volume it can take hours to run. Note that full recovery may involve a lot of manual work; for instance, if fsck finds any files without matching directory entries, it puts them into a `lost+found`{.docutils .literal .notranslate} directory with numeric names, leaving a human (i.e., you) to figure out what they are and where they belong.

Checking disks at startup worked fine when disks were small, but as they got larger (and seek times didn't get faster) it started taking longer and longer to check a file system after a crash. Uninterruptible power supplies help, but not completely, since many crashes are due to software faults in the operating system. The corruption problem you saw was due to inconsistency in the on-disk file system state. In this example, the free space bitmap did not agree with the directory entry and inode. If the file system can ensure that the on-disk data is always in a consistent state, then it should be possible to prevent losing any data except that being written at the exact moment of the crash.

Performing disk operations synchronously (and carefully ordering them in the code) will prevent inconsistency, but as described above, imposes excessive performance costs. Instead a newer generation of file systems, termed *journaling* file systems, has incorporated mechanisms which add additional information which can be used for recovery, allowing caching and efficient use of the disk, while maintaining a consistent on-disk state.
:::

::: {#journaling .section}

## [22.5.2. ] {.section-number}Journaling[\#](#journaling "Link to this heading") {.headerlink}

Most modern file systems (NTFS, ext3, ext4, and various others) use *journaling*, a variant of the database technique of *write-ahead logging*. The idea is to keep a log which records the changes that are going to be made to the file system, *before those changes are made*. After an entry is written to the log, the changes can be written back in any order; after they are all written, the section of log recording those changes can be freed.

When recovering from a crash, the OS goes through the log and checks that all the changes recorded there have been performed on the file system itself[[\[]{.fn-bracket}2[\]]{.fn-bracket}](#log){#id2 .footnote-reference .brackets role="doc-noteref"}. Some thought should convince you that if a log entry is written, then the modification is guaranteed to happen, either before or after a crash; if the log entry isn't written completely then the modification never happened. (There are several ways to detect a half-written log entry, including using an explicit end marker or a checksum; we'll just assume that it's possible.)

![[Fig. 22.16 ]{.caption-number}[Step 1: record action in log]{.caption-text}[\#](#id4 "Link to this image"){.headerlink}](../_images/files-logging.png){style="width: 200pt;"}

![[Fig. 22.17 ]{.caption-number}[Step 2: write blocks in any order]{.caption-text}[\#](#id5 "Link to this image"){.headerlink}](../_images/files-corruption2.png){style="width: 200pt;"}

**Ext3 Journaling**: The ext3 file system uses physical block logging: each log entry contains a header identifying the disk blocks which are modified (in the example you saw earlier, the bitmap and the directory entry) and a copy of the disk blocks themselves. After a crash the log is replayed by writing each block from the log to the location where it belongs. If a block is written multiple times in the log, it will get overwritten multiple times during replay, and after the last over-write it will have the correct value.

To avoid synchronous journal writes for every file operation, ext3 uses *batch commit*: journal writes are deferred, and multiple writes are combined into a single transaction. The log entries for the entire batch are written to the log in a single sequential write, called a *checkpoint*. In the event of a crash, any modifications since the last checkpoint will be lost, but since checkpoints are performed at least every few seconds, this typically isn't a problem. (If your program needs a guarantee that data is written to a file *right now*, you need to use the `fsync`{.docutils .literal .notranslate} system call to flush data to disk.)

Ext3 supports three different journaling modes:

- *Journaled*: In this mode, all changes (to file data, directories, inodes and bitmaps) are written to the log before any modifications are made to the main file system.
- *Ordered*: Here, data blocks are flushed to the main file system before a journal entry for any metadata changes (directories, free space bitmaps, inodes) is written to the log, after which the metadata changes may be made in the file system. This provides the same consistency guarantees as journaled mode, but is usually faster.
- *Writeback*: In this mode, metadata changes are always written to the log before being applied to the main file system, but data may be written at any time. It is faster than the other two modes, and will prevent the file system itself from becoming corrupted, but data within a file may be lost.
  :::

::: {#log-structured-file-systems .section}

## [22.5.3. ] {.section-number}Log-Structured File Systems[\#](#log-structured-file-systems "Link to this heading") {.headerlink}

Log-structured file systems (like LFS in NetBSD, or NetApp WAFL) are an extreme version of a journaled file system: the journal is the entire file system. Data is never over-written; instead a form of copy-on-write is used: modified data is written sequentially to new locations in the log. This gives very high write speeds because all writes (even random ones) are written sequentially to the disk.

[[Fig. 22.18]{.std .std-numref}](#fig-fs-lfs){.reference .internal} compares LFS to ext2, showing a simple file system with two directories (dir1, dir2) and two files (/dir1/file1, /dir2/file2). In ext2 the root directory inode is found in a fixed location, and its data blocks do not move after being allocated; in LFS both inode and data blocks move around---as they are modified, the new blocks get written to the head of the log rather than overwriting the old ones. The result can be seen graphically in the figure---in the LFS image, pointers only point to the left, pointing to data that is older than the block holding a pointer.

![[Fig. 22.18 ]{.caption-number}[Ext2 vs. Log-structured file system layout]{.caption-text}[\#](#fig-fs-lfs "Link to this image"){.headerlink}](../_images/files-lfs.png){style="width: 100%;"}

Unlike ext2 there is no fixed location to find the root directory; this is solved by periodically storing its location in a small checkpoint record in a fixed location in the superblock. (This checkpoint is not shown in the figure, and would be the only arrow pointing to the right.)

When a data block is re-written, a new block with a new address is used. This means that the inode (or indirect block) pointing to the data block must be modified, which means that its address changes.

LFS uses a table mapping inodes to locations on disk, which is updated with the new inode address to complete the process; this table is itself stored as a file. (The astute reader may wonder why this update doesn't in fact trigger another update to the inode file, leading to an infinite loop. This is solved by buffering blocks in memory before they are written, so that multiple changes can be made.)

![[Fig. 22.19 ]{.caption-number}[WAFL tree before update]{.caption-text}[\#](#fig-fs-waflbef "Link to this image"){.headerlink}](../_images/files-wafl1.png){style="width: 200pt;"}

![[Fig. 22.20 ]{.caption-number}[WAFL tree after update]{.caption-text}[\#](#fig-fs-waflaft "Link to this image"){.headerlink}](../_images/files-wafl2.png){style="width: 200pt;"}

In WAFL these changes percolate all the way up through directory entries, directory inodes, etc., to the root of the file system, potentially causing a large number of writes for a small modification. (although they'll still be fairly fast since it's a single sequential write) To avoid this overhead, WAFL buffers a large number of changes before writing to disk; thus although any single write will modify the root directory, only a single modified copy of the root directory has to be written in each batch.

In [[Fig. 22.19]{.std .std-numref}](#fig-fs-waflbef){.reference .internal} and [[Fig. 22.20]{.std .std-numref}](#fig-fs-waflaft){.reference .internal} a WAFL directory tree is shown before and after modifying /dir1/file2, with the out-of-date blocks shown in grey. If we keep a pointer to the old root node, then you can access a copy of the file system as it was at that point in time. When the disk fills up, these out-of-date blocks are collected by a garbage collection process, and made available for new writes.

One of the advantages of a log-structured file system is the ability to easily keep snapshots of file system state---a pointer to an old version of the inode table or root directory will give you access to a copy of the file system at the point in time corresponding to that version.

---

[[\[]{.fn-bracket}[1](#id1){role="doc-backlink"}[\]]{.fn-bracket}]{.label}

These steps ignore inode writes to update file or directory modification times.

[[\[]{.fn-bracket}[2](#id2){role="doc-backlink"}[\]]{.fn-bracket}]{.label}

Actually it doesn't check, but rather "replays" all the changes recorded in the log.
:::
:::

::: prev-next-area
[](dl_name.html "previous page"){.left-prev}

::: prev-next-info
previous

[22.4. ]{.section-number}Disk Layout:Implementing Name Space
:::

[](dl_ex_exx.html "next page"){.right-next}

::: prev-next-info
next

[22.6. ]{.section-number}Disk Layout:Examples of Real World File Systems
:::
:::
:::

::: {.bd-sidebar-secondary .bd-toc}
::: {.sidebar-secondary-items .sidebar-secondary__inner}
::: sidebar-secondary-item
::: {.page-toc .tocsection .onthispage}
Contents
:::

- [22.5.1. Consistency and Journaling](#consistency-and-journaling){.reference .internal .nav-link}
- [22.5.2. Journaling](#journaling){.reference .internal .nav-link}
- [22.5.3. Log-Structured File Systems](#log-structured-file-systems){.reference .internal .nav-link}
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
