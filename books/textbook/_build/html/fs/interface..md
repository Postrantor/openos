---
docsearch:language: en
lang: en
title: 20. File System Abstraction --- Introduction to Operating Systems
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
-   [20. File System Abstraction](#){.current .reference .internal}
-   [21. A bit about Disks](diskhw.html){.reference .internal}
-   [22. Implementation](impl.html){.reference .internal}
    []{.toctree-toggle role="presentation"}
    -   [22.1. File System Layout](disklayout.html){.reference .internal}
    -   [22.2. Disk Layout:Tracking Used Space](dl_track_used.html){.reference .internal}
    -   [22.3. Disk Layout:Tracking Free Space](dl_track_free.html){.reference .internal}
    -   [22.4. Disk Layout:Implementing Name Space](dl_name.html){.reference .internal}
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

-   [[ ![JupyterHub logo](../_static/images/logo_jupyterhub.svg) ]{.btn__icon-container} [JupyterHub]{.btn__text-container}](https://jupyterhub-opf-jupyterhub.apps.smaug.na.operate-first.cloud/hub/user-redirect/git-pull?repo=https%3A//github.com/OpenOSOrg/openos&urlpath=lab/tree/openos/content/fs/interface.ipynb&branch=main "Launch on JupyterHub"){.btn .btn-sm .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
:::

::: {.dropdown .dropdown-source-buttons}

-   [[ ]{.btn__icon-container} [Repository]{.btn__text-container}](https://github.com/OpenOSOrg/openos "Source repository"){.btn .btn-sm .btn-source-repository-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
-   [[ ]{.btn__icon-container} [Suggest edit]{.btn__text-container}](https://github.com/OpenOSOrg/openos/edit/main/content/fs/interface.ipynb "Suggest edit"){.btn .btn-sm .btn-source-edit-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
-   [[ ]{.btn__icon-container} [Open issue]{.btn__text-container}](https://github.com/OpenOSOrg/openos/issues/new?title=Issue%20on%20page%20%2Ffs/interface.html&body=Your%20issue%20content%20here. "Open an issue"){.btn .btn-sm .btn-source-issues-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
:::

::: {.dropdown .dropdown-download-buttons}

-   [[ ]{.btn__icon-container} [.ipynb]{.btn__text-container}](../_sources/fs/interface.ipynb "Download source file"){.btn .btn-sm .btn-download-source-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
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
# File System Abstraction

::: {#print-main-content}
::: {#jb-print-toc}
<div>

## Contents

</div>

-   [20.1. Naming](#naming){.reference .internal .nav-link}
-   [20.2. Objects](#objects){.reference .internal .nav-link}
    -   [20.2.1. Files](#files){.reference .internal .nav-link}
    -   [20.2.2. Directory](#directory){.reference .internal .nav-link}
    -   [20.2.3. Symbolic links](#symbolic-links){.reference .internal .nav-link}
-   [20.3. File System Operations:](#file-system-operations){.reference .internal .nav-link}
    -   [20.3.1. Open/close](#open-close){.reference .internal .nav-link}
        -   [20.3.1.1. Read/Write operations](#read-write-operations){.reference .internal .nav-link}
    -   [20.3.2. Naming and Directories](#naming-and-directories){.reference .internal .nav-link}
-   [20.4. Some examples](#some-examples){.reference .internal .nav-link}
:::
:::
:::

::: {#searchbox}
:::

::: {.cell .tag_remove-input .tag_hide-output .docutils .container}
:::

::: {#file-system-abstraction .section .tex2jax_ignore .mathjax_ignore}
[]{#cont-fs-interface}

# [20. ]{.section-number}File System Abstraction[\#](#file-system-abstraction "Link to this heading"){.headerlink}

From a user perspective, file systems support:

-   a *name space*, the set of names that identify objects;

-   *objects* such as the files themselves as well as directories and other supporting objects;

-   *operations* on these objects.

We first describe how naming works in a Unix file system, then some of the core objects and how they are identified, and then the operations a process can perform on those objects.

::: {#naming .section}
## [20.1. ]{.section-number}Naming[\#](#naming "Link to this heading"){.headerlink}

Most file systems today support a tree-structured namespace[[\[]{.fn-bracket}1[\]]{.fn-bracket}](#hier){#id1 .footnote-reference .brackets role="doc-noteref"}, as shown in [[Fig. 20.1]{.std .std-numref}](#fs-tree-logical){.reference .internal}. This tree is constructed via the use of *directories*, or objects in the namespace which map strings to further file system objects. A full filename thus specifies a *path* from the root, through the tree, to the object (a file or directory) itself. (Hence the use of the term "path" to mean "filename" in Unix documentation.)

![[Fig. 20.1 ]{.caption-number}[Logical view: hierarchical file system name space]{.caption-text}[\#](#fs-tree-logical "Link to this image"){.headerlink}](../_images/filesys-tree.png){style="width: 70%;"}

Each process has an associated *current directory*, which may be changed via the `chdir`{.docutils .literal .notranslate} system call. File names beginning with '`/`{.docutils .literal .notranslate}' are termed *absolute* names, and are interpreted relative to the root of the naming tree, while *relative* names are interpreted beginning at the current directory. Thus in the file system in [[Fig. 20.1]{.std .std-numref}](#fs-tree-logical){.reference .internal}, if the current directory were `/home`{.docutils .literal .notranslate}, the the paths `pjd/.profile`{.docutils .literal .notranslate} and `/home/pjd/.profile`{.docutils .literal .notranslate} refer to the same file, and `../bin/cat`{.docutils .literal .notranslate} and `/bin/cat`{.docutils .literal .notranslate} refer to the same file.

Each directory also contains two special files `.`{.docutils .literal .notranslate} and `..`{.docutils .literal .notranslate}, where `d/..`{.docutils .literal .notranslate} identifies the parent directory of `d`{.docutils .literal .notranslate}, and `d/.`{.docutils .literal .notranslate} identifies `d`{.docutils .literal .notranslate} itself.

A typical system may provide access to several file systems at once, e.g., a local disk and an external USB drive or network volume. In order to unambiguously specify a file we thus need to both identify the file within possibly nested directories in a single file system, as well as identifying the file system itself. Unix enables a file system to be *mounted* onto a directory in another file system, giving a single uniform namespace. For example, on the systems you are using, there is an *ext4* file system mounted in the root file system at `/opt/app-root/src`{.docutils .literal .notranslate}, which you can see if you use the mount command to list all the file systems mounted on this computer.

::: {.cell .tag_remove-input .docutils .container}
::: {.cell_output .docutils .container}
:::
:::

The actual implementation of mounting in Linux and other Unix-like systems is implemented via a *mount table*, a small table in the kernel mapping directories to directories on other file systems. As the kernel translates a pathname it checks each directory in this table; if found, it substitutes the mapped file system and directory before searching for an entry. Thus before searching "/opt/app-root/src" on for the entry "foo", the kernel will substitute the top-level directory on the mounted ext4 files system then search for "foo".

For a more thorough explanation of path translation in Linux and other Unix systems see the `path_resolution(7)`{.docutils .literal .notranslate} man page, i.e. type `man path_resolution`{.docutils .literal .notranslate}.
:::

::: {#objects .section}
## [20.2. ]{.section-number}Objects[\#](#objects "Link to this heading"){.headerlink}

So, why is it called an inode? Dennis Ritchie, who was one of the authors of UNIX, gave this enlightened answer to the Linux kernel mailing list in 2002:

> <div>
>
> In truth, I don't know either. It was just a term that we started to use. "Index" is my best guess, because of the slightly unusual file system structure that stored the access information of files as a flat array on the disk, with all the hierarchical directory information living aside from this. Thus the i-number is an index in this array, the i-node is the selected element of the array.
>
> </div>

\-\--Dennis Ritchie, [\[LKML 2002\]](https://lkml.indiana.edu/hypermail/linux/kernel/0207.2/1182.html)

Once you use a pathname to find an object in the file system, you need to find out what kind of an object you have found. Each file is identified in the file system by a unique **inode number** that references an **inode** data structure that maintains all kinds of information, or *meta-data* about the file (try `man inode`{.docutils .literal .notranslate} for more information). While the inode itself is internal to the file system, and contains additional information, generic information can be obtained for any file as described [[below]{.std .std-ref}](#cont-fs-calls-naming){.reference .internal}. One of the fields in an inode identifies the type of object that the inode refers to. The types of objects that can be referenced by inode are shown in [[Table 20.1]{.std .std-numref}](#file-types){.reference .internal}.

::: pst-scrollable-table-container
+-------------------+----------------+--------------------------------------------------------------------------+
| Name              | Value          | Purpose                                                                  |
+===================+================+==========================================================================+
| regular file      | S_IFREG        | A regular file normally used to store data                               |
+-------------------+----------------+--------------------------------------------------------------------------+
| directory         | S_IFDIR        | A special file used to contain files or other directories                |
+-------------------+----------------+--------------------------------------------------------------------------+
| symbolic link     | S_IFLNK        | A kind of "file" that is essentially a pointer to another file name      |
+-------------------+----------------+--------------------------------------------------------------------------+
| block device      | S_IFBLK        | A device that like a disk that is accessed by reading and writing blocks |
+-------------------+----------------+--------------------------------------------------------------------------+
| character device  | S_IFCHR        | A charter device like a `tty`{.docutils .literal .notranslate}           |
+-------------------+----------------+--------------------------------------------------------------------------+
| FIFO              | S_IFIFO        | A pipe                                                                   |
+-------------------+----------------+--------------------------------------------------------------------------+
| socket            | S_IFSOCK       | A socket used for networking                                             |
+-------------------+----------------+--------------------------------------------------------------------------+

: [Table 20.1 ]{.caption-number}[Types of objects in a file system.]{.caption-text}[\#](#file-types "Link to this table"){.headerlink}
:::

The last four are special files that you can connect into a file system. The first three are core objects for all file systems.

::: {#files .section}
### [20.2.1. ]{.section-number}Files[\#](#files "Link to this heading"){.headerlink}

In keeping with the idea that everything is a file, Unix made all files just a sequence of 8-bit bytes[[\[]{.fn-bracket}2[\]]{.fn-bracket}](#eff){#id2 .footnote-reference .brackets role="doc-noteref"}[[\[]{.fn-bracket}3[\]]{.fn-bracket}](#simple){#id3 .footnote-reference .brackets role="doc-noteref"}. Any structure to the file (such as a JPEG image, an executable program, or a database) is the responsibility of applications which read and write the file. The file format is commonly indicated by a file extension like .jpg or .xml, but this is just a convention followed by applications and users. You can do things like rename file.pdf to file.jpg, which will confuse some applications and users, but it will have no effect on the file contents.

Data in a byte-sequence file is identified by the combination of the file and its offset (in bytes) within the file. Unlike in-memory objects in an application, where a reference (pointer) to a component of an object may be passed around independently, a portion of a file cannot be named without identifying the file it is contained in. Data in a file can be created by a `write`{.docutils .literal .notranslate} which appends more data to the end of a shorter file, and modified by over-writing in the middle of a file. However, it can't be "moved" from one offset to another: if you use a text editor to add or delete text in the middle of a file, the editor must re-write the entire file (or at least from the modified part to the end).

![[Fig. 20.2 ]{.caption-number}[Implementation view: hierarchical file system name space. Gray blocks are directories that contain entries with strings and corresponding inode numbers that identify the files.]{.caption-text}[\#](#fs-tree-imp "Link to this image"){.headerlink}](../_images/filesys-tree2.png){style="width: 70%;"}
:::

::: {#directory .section}
[]{#cont-fs-interface-dir}

### [20.2.2. ]{.section-number}Directory[\#](#directory "Link to this heading"){.headerlink}

As shown in [[Fig. 20.2]{.std .std-numref}](#fs-tree-imp){.reference .internal}, a directory contains entries with strings that identify objects contained in the directory, and for each the inode numbers that can then be used to find out more information about the corresponding object. The same inode can be referenced by multiple directories, with potentially different names. Each directory entry that maps a name to an inode number is called a *hard link* to the inode, and another field in the inode structure records the number of hard links to that inode. For example, the entry named `..`{.docutils .literal .notranslate} in any directory is a hard link to the parent directory. To illustrate this point, let's create a directory named `foo`{.docutils .literal .notranslate} in the `/tmp`{.docutils .literal .notranslate} directory and see how the link count for `foo`{.docutils .literal .notranslate} changes when we create a subdirectory `bar`{.docutils .literal .notranslate} inside foo.

::: {.cell .tag_remove-input .docutils .container}
::: {.cell_output .docutils .container}
:::
:::

As we can see, after creating a directory `/tmp/foo`{.docutils .literal .notranslate} the reference count (second entry in the output above) for the `.`{.docutils .literal .notranslate} in `foo`{.docutils .literal .notranslate} is 2 before we create a subdirectory `bar`{.docutils .literal .notranslate} in it, and 3 after. The initial two links come from the parent directory's entry named `foo`{.docutils .literal .notranslate}, and the `.`{.docutils .literal .notranslate} entry in `foo`{.docutils .literal .notranslate} itself. After the creation of `bar`{.docutils .literal .notranslate}, there is a third link to the inode for `foo`{.docutils .literal .notranslate} due to the `..`{.docutils .literal .notranslate} entry in `bar`{.docutils .literal .notranslate}, which refers to its parent directory.

The link count in an inode ensures that the object the inode refers to (file or directory) will not be deleted as long as there is at least one hard link to the inode. When you issue a delete command for a filename (e.g., 'rm somefile'), the file system removes the entry for the filename from a directory and decrements the link count on the inode that entry referred to. Only when the last hard link is removed will the file object really be freed.
:::

::: {#symbolic-links .section}
### [20.2.3. ]{.section-number}Symbolic links[\#](#symbolic-links "Link to this heading"){.headerlink}

The third file system object is a *symbolic link*. This holds a text string which is interpreted as a "pointer" to another location in the file system. When the kernel is searching for a file and encounters a symbolic link, it substitutes this text into the current portion of the path, and continues the translation process.

This can be very useful

    directory: /usr/program-1.0.1
      file:      /usr/program-1.0.1/file.txt
      sym link:  /usr/program-current -> "program-1.0.1"

and if the OS is looking up the file `/usr/program-current/file.txt`{.docutils .literal .notranslate}, it will:

1.  look up `usr`{.docutils .literal .notranslate} in the root directory, finding a pointer to the `/usr`{.docutils .literal .notranslate} directory

2.  look up `program-current`{.docutils .literal .notranslate} in `/usr`{.docutils .literal .notranslate}, finding the link with contents `program-1.0.1`{.docutils .literal .notranslate}

3.  look up `program-1.0.1`{.docutils .literal .notranslate} and use this result instead of the result from looking up `program-current`{.docutils .literal .notranslate}, getting a pointer to the `/usr/program-1.0.1`{.docutils .literal .notranslate} directory.

4.  look up `file.txt`{.docutils .literal .notranslate} in this directory, and find it.

Note that unlike hard links, a symbolic link does not increase the link count in the inode that it refers to. As a result, a symbolic link may be "broken"---i.e., if the file it points to does not exist. This can happen if the link was created in error, or the file or directory it points to is deleted later. In that case path translation will fail with an error:

::: {.cell .tag_remove-input .docutils .container}
::: {.cell_output .docutils .container}
:::
:::

Finally, to prevent loops there is a limit on how many levels of symbolic link may be traversed in a single path translation:

::: {.cell .tag_remove-input .docutils .container}
::: {.cell_output .docutils .container}
:::
:::
:::
:::

::: {#file-system-operations .section}
## [20.3. ]{.section-number}File System Operations:[\#](#file-system-operations "Link to this heading"){.headerlink}

There are several common types of file operations supported by Linux (and with slight differences, Windows). They can be classified into three main categories: open/close, read/write, and naming and directories.

::: {#open-close .section}
### [20.3.1. ]{.section-number}Open/close[\#](#open-close "Link to this heading"){.headerlink}

In order to access a file in Linux (or most operating systems) you first need to open the file, passing the file name and other parameters and receiving a *handle* (called a *file descriptor* in Unix) which may be used for further operations. The corresponding system calls are:

-   `int desc = open(name, O_READ)`{.docutils .literal .notranslate}: Verify that file `name`{.docutils .literal .notranslate} exists and may be read, and then return a *descriptor* which may be used to refer to that file when reading it.

-   `int desc = open(name, O_WRITE | flags, mode)`{.docutils .literal .notranslate}: Verify permissions and open `name`{.docutils .literal .notranslate} for writing, creating it (or erasing existing contents) if necessary as specified in `flags`{.docutils .literal .notranslate}. Returns a descriptor which may be used for writing to that file.

-   `close(desc)`{.docutils .literal .notranslate}: stop using this descriptor, and free any resources allocated for it.

Note that application programs rarely use the system calls themselves to access files, but instead use higher-level frameworks, ranging from Unix Standard I/O to high-level application frameworks.

::: {#read-write-operations .section}
[]{#cont-fs-interface-operations}

#### [20.3.1.1. ]{.section-number}Read/Write operations[\#](#read-write-operations "Link to this heading"){.headerlink}

To get a file with data in it, you need to write it; to use that data you need to read it. To enable files to be accessed as a *stream* just like from a terminal or pipe, UNIX uses the concept of a *current position* associated with a file descriptor. When you read 100 bytes (i.e. bytes 0 to 99) from a file, this pointer advances by 100 bytes, so that the next read will start at byte 100, and similarly for write. When a file is opened for reading the pointer starts at 0; when open for writing the application writer can choose to start at the beginning (default) and overwrite old data, or start at the end (`O_APPEND`{.docutils .literal .notranslate} flag) to append new data to the file.

The read and write routines are the same ones we described before, but, for ease of reference, they are:

-   `n = read(desc, buffer, max)`{.docutils .literal .notranslate}: Read `max`{.docutils .literal .notranslate} bytes (or fewer if the end of the file is reached) into `buffer`{.docutils .literal .notranslate}, starting at the current position, and returning the actual number of bytes `n`{.docutils .literal .notranslate} read; the current position is then incremented by `n`{.docutils .literal .notranslate}.

-   `n = write(desc, buffer, len)`{.docutils .literal .notranslate}: Write `len`{.docutils .literal .notranslate} bytes from `buffer`{.docutils .literal .notranslate} into the file, starting at the current position, and incrementing the current position by `len`{.docutils .literal .notranslate}.

-   `lseek(desc, offset, flag)`{.docutils .literal .notranslate}: Set an open file's current position to that specified by `offset`{.docutils .literal .notranslate} and `flag`{.docutils .literal .notranslate}, which specifies whether `offset`{.docutils .literal .notranslate} is relative to the beginning, end, or current position in the file.

Note that in the basic Unix interface (unlike e.g. Windows) there is no way to specify a particular location in a file to read or write from[[\[]{.fn-bracket}4[\]]{.fn-bracket}](#pread){#id4 .footnote-reference .brackets role="doc-noteref"}. Programs like databases (e.g. SQLite, MySQL) which need to write to and read from arbitrary file locations must instead move the current position by using `lseek`{.docutils .literal .notranslate} before a read or write. However, most programs either read or write a file from the beginning to the end (especially when written for an OS that makes it easier to do things that way), and thus don't really need to perform seeks. Because most Unix programs use simple "stream" input and output, these may be re-directed so that the same program can---without any special programming---read from or write to a terminal, a network connection, a file, or a pipe from or to another program.
:::
:::

::: {#naming-and-directories .section}
[]{#cont-fs-calls-naming}

### [20.3.2. ]{.section-number}Naming and Directories[\#](#naming-and-directories "Link to this heading"){.headerlink}

In Unix there is a difference between a name (a directory entry) and the object (file or directory) that the name points to. The naming and directories operations are:

-   `rename(path1, path2)`{.docutils .literal .notranslate} - Rename an object (i.e., a file or directory) by either changing the name in its directory entry (if the destination is in the same directory) or creating a new entry and deleting the old one (if moving into a new directory).

-   `link(path1, path2)`{.docutils .literal .notranslate}: Add a *hard link* to a file[[\[]{.fn-bracket}5[\]]{.fn-bracket}](#hardlink){#id5 .footnote-reference .brackets role="doc-noteref"}.

-   `unlink(path)`{.docutils .literal .notranslate}: Decrement the reference count to a file, if it goes to zero, delete the file[[\[]{.fn-bracket}6[\]]{.fn-bracket}](#unlink){#id6 .footnote-reference .brackets role="doc-noteref"}.

-   `desc = opendir(path)`{.docutils .literal .notranslate}, `readdir(desc, dirent*), dirent=(name,type,length)`{.docutils .literal .notranslate}: This interface allows a program to enumerate names in a directory, and determine their type (i.e., file, directory, symbolic link, or special-purpose file).

-   `stat(file, statbuf)`{.docutils .literal .notranslate}, `fstat(desc, statbuf)`{.docutils .literal .notranslate}: returns information about the file such as size, owner, permissions, modification time, etc. These are attributes of the file itself, residing in the inode and returned in the following structure.

::: {.highlight-c .notranslate}
::: highlight
    struct stat {
      dev_t     st_dev;         /* ID of device containing file */
      ino_t     st_ino;         /* Inode number */
      mode_t    st_mode;        /* File type and mode */
      nlink_t   st_nlink;       /* Number of hard links */
      uid_t     st_uid;         /* User ID of owner */
      gid_t     st_gid;         /* Group ID of owner */
      dev_t     st_rdev;        /* Device ID (if special file) */
      off_t     st_size;        /* Total size, in bytes */
      blksize_t st_blksize;     /* Block size for filesystem I/O */
      blkcnt_t  st_blocks;      /* Number of 512B blocks allocated */
      struct timespec st_atim;  /* Time of last access */
      struct timespec st_mtim;  /* Time of last modification */
      struct timespec st_ctim;  /* Time of last status change */
    };
:::
:::

-   `mkdir(path)`{.docutils .literal .notranslate}, `rmdir(path)`{.docutils .literal .notranslate}: directory operations: create a new, empty directory, or delete an empty directory.
:::
:::

::: {#some-examples .section}
## [20.4. ]{.section-number}Some examples[\#](#some-examples "Link to this heading"){.headerlink}

Consider the following program in [[Listing 20.1]{.std .std-numref}](#filecopy-listing){.reference .internal}, which copies one file to another. After opening the input file (line 26) we stat the input file to get the permissions (i.e., the mode), create a file with that mode (line 37), and then go into a loop reading data from the input file into a buffer, and then writing the buffer to the output file.

::: {#filecopy-listing .literal-block-wrapper .docutils .container}
::: code-block-caption
[Listing 20.1 ]{.caption-number}[fcopy2.c - An example program that copies one file to another using the file system interface.]{.caption-text}[\#](#filecopy-listing "Link to this code"){.headerlink}
:::

::: {.highlight-default .notranslate}
::: highlight
     1// simple program to copy a file
     2
     3#include <sys/types.h>
     4#include <fcntl.h>
     5#include <stdlib.h>
     6#include <unistd.h>
     7#include <stdio.h>
     8#include <assert.h>
     9#include <sys/stat.h>
    10
    11#define BUF_SIZE 4096
    12// user has read and write permission
    13
    14int main(int argc, char *argv[])
    15{
    16 int in_fd, out_fd, rd_count, wt_count, rc;
    17 mode_t md; 
    18 struct stat statbuf;    
    19 char buffer[BUF_SIZE];
    20
    21 if (argc != 3) {
    22     perror("Can't open input file\n");
    23     exit(1);
    24 }
    25
    26   in_fd = open(argv[1], O_RDONLY);
    27  if (in_fd < 0) {
    28     perror("Can't creat output file\n");
    29     exit(1);
    30 }
    31 if ((rc = fstat(in_fd, &statbuf)) <0) {
    32     perror("fstat failed\n");
    33     exit(1);
    34 }
    35 md = statbuf.st_mode & (S_IRWXU|S_IRWXG|S_IRWXO);
    36
    37   out_fd = creat(argv[2], md);
    38  if (out_fd < 0) {
    39     perror("Can't creat output file\n");
    40     exit(1);
    41 }
    42
    43   while(1) {
    44        rd_count = read(in_fd, buffer, BUF_SIZE);
    45      if (rd_count==0) { // done
    46         exit(0);
    47     }
    48     assert(rd_count > 0);
    49
    50         
    51       wt_count = write(out_fd, buffer, rd_count);
    52      assert(wt_count == rd_count);
    53 }
    54 close(in_fd);
    55 close(out_fd);
    56}
:::
:::
:::

::: {.cell .tag_remove-input .docutils .container}
::: {.cell_output .docutils .container}
:::
:::

To prove these are the same, let's first use the `diff`{.docutils .literal .notranslate} program to compare them:

::: {.cell .tag_remove-input .docutils .container}
::: {.cell_output .docutils .container}
:::
:::

We can see that there is no difference between the files, since `diff`{.docutils .literal .notranslate} produces no output. But just to be sure, let's append a string to the end of the copy (i.e., echo "Hello class" \>\> rm2) and use the `diff`{.docutils .literal .notranslate} program to compare them again.

::: {.cell .tag_remove-input .docutils .container}
::: {.cell_output .docutils .container}
:::
:::

And here we see that the only difference is the line we just appended to the copy of the original `README.md`{.docutils .literal .notranslate} file.

------------------------------------------------------------------------

[[\[]{.fn-bracket}[1](#id1){role="doc-backlink"}[\]]{.fn-bracket}]{.label}

Very early file systems sometimes had a single flat directory per user, or like MS-DOS 1.0, a single directory per floppy disk

[[\[]{.fn-bracket}[2](#id2){role="doc-backlink"}[\]]{.fn-bracket}]{.label}

it is probably not a coincidence that Unix arrived at the same time as computers which dealt only with multiples of 8-bit bytes (e.g. 16 and 32-bit words), replacing older systems which frequently used odd word sizes such as 36 bits. (Note that a machine with 36-bit instructions already needs two incompatible types of files, one for text and one for executable code.)

[[\[]{.fn-bracket}[3](#id3){role="doc-backlink"}[\]]{.fn-bracket}]{.label}

This is the case for almost all operating systems today, but... of course there are exceptions. Apple OSX uses resource forks to store information associated with a file (HFS and HFS+ file systems only), Windows NTFS provides for multiple data streams in single file, although they were never put to use, and several file systems support file attributes, which are small tags associated with a file.

[[\[]{.fn-bracket}[4](#id4){role="doc-backlink"}[\]]{.fn-bracket}]{.label}

On Linux the `pread`{.docutils .literal .notranslate} and `pwrite`{.docutils .literal .notranslate} system calls allow specifying an offset for the read or write; other UNIX-derived operating systems have their own extensions for this purpose.

[[\[]{.fn-bracket}[5](#id5){role="doc-backlink"}[\]]{.fn-bracket}]{.label}

A hard link is an additional directory entry pointing to the same file, giving the file two (or more) names. Hard links are peculiar to Unix, and in modern systems have mostly been replaced with symbolic links (covered above); however Apple's Time Machine makes very good use of them: multiple backups can point to the same single copy of an un-modified file using hard links.

[[\[]{.fn-bracket}[6](#id6){role="doc-backlink"}[\]]{.fn-bracket}]{.label}

Even when the reference count goes to zero, the file might not be removed yet - on Unix, if you delete an open file it won't actually be removed until all open file handles are closed.. In general, deleting open files is a problem: while Unix solves the problem by deferring the actual delete, Windows solves it by protecting open files so that they cannot be deleted.
:::
:::

::: prev-next-area
[](intro.html "previous page"){.left-prev}

::: prev-next-info
previous

[19. ]{.section-number}Introduction
:::

[](diskhw.html "next page"){.right-next}

::: prev-next-info
next

[21. ]{.section-number}A bit about Disks
:::
:::
:::

::: {.bd-sidebar-secondary .bd-toc}
::: {.sidebar-secondary-items .sidebar-secondary__inner}
::: sidebar-secondary-item
::: {.page-toc .tocsection .onthispage}
Contents
:::

-   [20.1. Naming](#naming){.reference .internal .nav-link}
-   [20.2. Objects](#objects){.reference .internal .nav-link}
    -   [20.2.1. Files](#files){.reference .internal .nav-link}
    -   [20.2.2. Directory](#directory){.reference .internal .nav-link}
    -   [20.2.3. Symbolic links](#symbolic-links){.reference .internal .nav-link}
-   [20.3. File System Operations:](#file-system-operations){.reference .internal .nav-link}
    -   [20.3.1. Open/close](#open-close){.reference .internal .nav-link}
        -   [20.3.1.1. Read/Write operations](#read-write-operations){.reference .internal .nav-link}
    -   [20.3.2. Naming and Directories](#naming-and-directories){.reference .internal .nav-link}
-   [20.4. Some examples](#some-examples){.reference .internal .nav-link}
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
