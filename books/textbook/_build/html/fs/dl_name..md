---
docsearch:language: en
lang: en
title: "22.4. Disk Layout:Implementing Name Space --- Introduction to Operating Systems"
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

-   [19. Introduction](intro.html){.reference .internal}
-   [20. File System Abstraction](interface.html){.reference .internal}
-   [21. A bit about Disks](diskhw.html){.reference .internal}
-   [22. Implementation](impl.html){.reference .internal}
    []{.toctree-toggle role="presentation"}
    -   [22.1. File System Layout](disklayout.html){.reference .internal}
    -   [22.2. Disk Layout:Tracking Used Space](dl_track_used.html){.reference .internal}
    -   [22.3. Disk Layout:Tracking Free Space](dl_track_free.html){.reference .internal}
    -   [22.4. Disk Layout:Implementing Name Space](#){.current .reference .internal}
    -   [22.5. Disk Layout:Dealing with Failures](dl_failures.html){.reference .internal}
    -   [22.6. Disk Layout:Examples of Real World File Systems](dl_ex_exx.html){.reference .internal}
    -   [22.7. Kernel implementation](kernelimp.html){.reference .internal}
-   [23. Review](review.html){.reference .internal}

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

-   [[ ![JupyterHub logo](../_static/images/logo_jupyterhub.svg) ]{.btn__icon-container} [JupyterHub]{.btn__text-container}](https://jupyterhub-opf-jupyterhub.apps.smaug.na.operate-first.cloud/hub/user-redirect/git-pull?repo=https%3A//github.com/OpenOSOrg/openos&urlpath=lab/tree/openos/content/fs/dl_name.ipynb&branch=main "Launch on JupyterHub"){.btn .btn-sm .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
:::

::: {.dropdown .dropdown-source-buttons}

-   [[ ]{.btn__icon-container} [Repository]{.btn__text-container}](https://github.com/OpenOSOrg/openos "Source repository"){.btn .btn-sm .btn-source-repository-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
-   [[ ]{.btn__icon-container} [Suggest edit]{.btn__text-container}](https://github.com/OpenOSOrg/openos/edit/main/content/fs/dl_name.ipynb "Suggest edit"){.btn .btn-sm .btn-source-edit-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
-   [[ ]{.btn__icon-container} [Open issue]{.btn__text-container}](https://github.com/OpenOSOrg/openos/issues/new?title=Issue%20on%20page%20%2Ffs/dl_name.html&body=Your%20issue%20content%20here. "Open an issue"){.btn .btn-sm .btn-source-issues-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
:::

::: {.dropdown .dropdown-download-buttons}

-   [[ ]{.btn__icon-container} [.ipynb]{.btn__text-container}](../_sources/fs/dl_name.ipynb "Download source file"){.btn .btn-sm .btn-download-source-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
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
# Disk Layout:Implementing Name Space

::: {#print-main-content}
::: {#jb-print-toc}
<div>

## Contents

</div>

-   [22.4.1. Smarter Directories](#smarter-directories){.reference .internal .nav-link}
:::
:::
:::

::: {#searchbox}
:::

::: {#disk-layout-implementing-name-space .section .tex2jax_ignore .mathjax_ignore}
[]{#fs-dl-name}

# [22.4. ]{.section-number}Disk Layout:Implementing Name Space[\#](#disk-layout-implementing-name-space "Link to this heading"){.headerlink}

As we discussed in the [[file system abstractions]{.std .std-ref}](interface.html#cont-fs-interface-dir){.reference .internal}, the name space is created by having directories, where a directory as shown in [[Fig. 22.10]{.std .std-numref}](#fs-tree-imp-rep){.reference .internal}, is just another file that has strings and information about the files those strings represent.

![[Fig. 22.10 ]{.caption-number}[Implementation view: hierarchical file system name space. Gray blocks are directories that contain entries with strings and corresponding inode numbers that identify the files.]{.caption-text}[\#](#fs-tree-imp-rep "Link to this image"){.headerlink}](../_images/filesys-tree2.png){style="width: 70%;"}

A simple way to implement such a directory ([[Fig. 22.11]{.std .std-numref}](#directory1){.reference .internal}a), is to have a fixed array of data structures, where each entry has room for a fixed-size string, and the attributes of the file such as permissions, owner, and location of file on disk. This approach is used in the MS-DOS, and CDROM file systems described earlier. With these file systems, there is only one name for each file, and attributes identify if an entry is valid or not.

For Unix file systems, the directory typically does not contain the attributes, but instead contains an inode number ([[Fig. 22.11]{.std .std-numref}](#directory1){.reference .internal}b) that identifies the inode that contains those attributes; this approach enables multiple directory entries to reference the same file. The separation of name (i.e., directory entry) and attributes (the inode and the blocks it points to) allows files to have multiple names, which for historical reasons are called hard links.

![[Fig. 22.11 ]{.caption-number}[Structure of a simplified directory with fixed-size file names where attributes are stored in the directory or in an external inode]{.caption-text}[\#](#directory1 "Link to this image"){.headerlink}](../_images/directory1.png){style="width: 70%;"}

The directory structure above could be implemented with the following data structure in [[Listing 22.1]{.std .std-numref}](#fs-simple-dirent){.reference .internal}:

::: {#fs-simple-dirent .literal-block-wrapper .docutils .container}
::: code-block-caption
[Listing 22.1 ]{.caption-number}[Simple data structure for a directory entry.]{.caption-text}[\#](#fs-simple-dirent "Link to this code"){.headerlink}
:::

::: {.highlight-c .notranslate}
::: highlight
    struct dentry {
        // inode number
        unsigned int inode;
        // file name, max 252 chars
        char name[252];
    };
:::
:::
:::

This simple directory entry structure supports files with string names that can be up to 252 characters, and an inode number. Assuming 4-byte integers, one directory entry takes up 256 bytes. When searching for a file, the directory block(s) are read into memory and a linear search through the entries is used to locate the file. The alignment to 256 bytes (i.e., the somewhat strange length of the string name) ensures that when the entry is loaded into memory, the 4 byte inode is aligned to 4 bytes; so the processor can load it with a single memory load. The 256-byte entry size also ensures that directory entries are never split across file system blocks. For example, with a 4 K block size, one directory block will hold exactly 16 of these 256-byte directory entries. A simple fixed-size data structure like this is easy to manage: a new file is added by searching for an entry with an invalid attribute, and deleting a file just sets the attribute to invalid.

With the above data structure, all file names are limited to at most 252 characters, and more importantly, you are wasting a great deal of space for most files that have short names. More sophisticated file systems use structures like the ext2 file system shown below in [[Listing 22.2]{.std .std-numref}](#fs-ext2-dirent){.reference .internal}:

::: {#fs-ext2-dirent .literal-block-wrapper .docutils .container}
::: code-block-caption
[Listing 22.2 ]{.caption-number}[Data structure used by ext2 file system directory entries.]{.caption-text}[\#](#fs-ext2-dirent "Link to this code"){.headerlink}
:::

::: {.highlight-c .notranslate}
::: highlight
    struct ext2_dir_entry {
        // inode number
        unsigned int   inode;
        // directory entry length
        unsigned short rec_len;
        // name length
        unsigned char  name_len;  
        // file type
        unsigned char  file_type;
        // file name, max 255 chars
        char           name[];
    };
:::
:::
:::

In this case, the name of the file is variable length, with the length of the string specified by `name_len`{.docutils .literal .notranslate}. The `rec_len`{.docutils .literal .notranslate} describes how big the record is. The `rec_len`{.docutils .literal .notranslate} may include padding to ensure that entries are aligned to 4-byte boundaries. The last entry's `rec_len`{.docutils .literal .notranslate} can be set to the remainder of the size of the directory block, and if a file is unlinked from a directory, the previous entry's `rec_len`{.docutils .literal .notranslate} can be padded by the size of the record being removed. This enables the file system to add a new file to the directory by comparing the `rec_len`{.docutils .literal .notranslate} and the `name_len`{.docutils .literal .notranslate} to identify if there is enough unused space between the used part of a directory entry and the next to insert the file.

::: {#smarter-directories .section}
## [22.4.1. ]{.section-number}Smarter Directories[\#](#smarter-directories "Link to this heading"){.headerlink}

From your data structures class, you should realize that linear search isn't an optimal algorithm for searching, but it's simple, robust, and fast enough for small directories, where the primary cost is retrieving a block of data from the disk. As an example, a local machine of the author has has 94,944 directories that use a single 4 KB block, another 957 directories that use 2 to 5 blocks, and only 125 directories that are larger than 5 blocks. In other words, for the 99% of the directories that fit within a single 4 KB block, a more complex algorithm would not reduce the amount of data read from disk, and the difference between [\\(O(N)\\)]{.math .notranslate .nohighlight} and [\\(O(logN)\\)]{.math .notranslate .nohighlight} algorithms when searching a single block is negligible.

However, the largest directories are actually quite big: the largest on this machine, for example, has 13,748 entries; another system contains about 64,000 files with long file names, or roughly 4000 blocks (16 MB) of directory data. Since directories tend to grow slowly, these blocks were probably allocated a few at a time, resulting in hundreds or thousands of disk seeks to read the entire directory into memory. At 15 ms per seek, this could require 10-30 seconds or more, and once the data was cached in memory, linear search in a 16 MB array will probably take a millisecond or two.

To allow directories with tens of thousands of files or more, modern file systems tend to use more advanced data structures for their directories. NTFS and Btrfs use B-trees, a form of a balanced tree. Other file systems, like Sun ZFS, use hash tables for their directories, while ext4 uses a hybrid hash/tree structure.
:::
:::

::: prev-next-area
[](dl_track_free.html "previous page"){.left-prev}

::: prev-next-info
previous

[22.3. ]{.section-number}Disk Layout:Tracking Free Space
:::

[](dl_failures.html "next page"){.right-next}

::: prev-next-info
next

[22.5. ]{.section-number}Disk Layout:Dealing with Failures
:::
:::
:::

::: {.bd-sidebar-secondary .bd-toc}
::: {.sidebar-secondary-items .sidebar-secondary__inner}
::: sidebar-secondary-item
::: {.page-toc .tocsection .onthispage}
Contents
:::

-   [22.4.1. Smarter Directories](#smarter-directories){.reference .internal .nav-link}
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
