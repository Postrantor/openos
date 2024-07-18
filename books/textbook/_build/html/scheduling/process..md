---
docsearch:language: en
lang: en
title: "7. The Process: A virtual Computer --- Introduction to Operating Systems"
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

-   [6. Introduction](intro.html){.reference .internal}
-   [7. The Process: A virtual Computer](#){.current .reference .internal}
-   [8. Virtualizing the CPU](virtual.html){.reference .internal}
-   [9. The Thread: A Virtual CPU](threads.html){.reference .internal}
-   [10. Scheduling](scheduling.html){.reference .internal}
    []{.toctree-toggle role="presentation"}
    -   [10.1. Scheduling Goals](sch-goals.html){.reference .internal}
    -   [10.2. Simple Examples of Scheduling Policies](sch-simple.html){.reference .internal}
    -   [10.3. Scheduling with Priorities](sch-prio.html){.reference .internal}
    -   [10.4. Scheduling in the real world](sch-real.html){.reference .internal}
-   [11. Review Questions](review.html){.reference .internal}

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

-   [[ ![JupyterHub logo](../_static/images/logo_jupyterhub.svg) ]{.btn__icon-container} [JupyterHub]{.btn__text-container}](https://jupyterhub-opf-jupyterhub.apps.smaug.na.operate-first.cloud/hub/user-redirect/git-pull?repo=https%3A//github.com/OpenOSOrg/openos&urlpath=lab/tree/openos/content/scheduling/process.ipynb&branch=main "Launch on JupyterHub"){.btn .btn-sm .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
:::

::: {.dropdown .dropdown-source-buttons}

-   [[ ]{.btn__icon-container} [Repository]{.btn__text-container}](https://github.com/OpenOSOrg/openos "Source repository"){.btn .btn-sm .btn-source-repository-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
-   [[ ]{.btn__icon-container} [Suggest edit]{.btn__text-container}](https://github.com/OpenOSOrg/openos/edit/main/content/scheduling/process.ipynb "Suggest edit"){.btn .btn-sm .btn-source-edit-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
-   [[ ]{.btn__icon-container} [Open issue]{.btn__text-container}](https://github.com/OpenOSOrg/openos/issues/new?title=Issue%20on%20page%20%2Fscheduling/process.html&body=Your%20issue%20content%20here. "Open an issue"){.btn .btn-sm .btn-source-issues-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
:::

::: {.dropdown .dropdown-download-buttons}

-   [[ ]{.btn__icon-container} [.ipynb]{.btn__text-container}](../_sources/scheduling/process.ipynb "Download source file"){.btn .btn-sm .btn-download-source-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
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
# The Process: A virtual Computer

::: {#print-main-content}
::: {#jb-print-toc}
<div>

## Contents

</div>

-   [7.1. The interface](#the-interface){.reference .internal .nav-link}
-   [7.2. Process versus Program](#process-versus-program){.reference .internal .nav-link}
:::
:::
:::

::: {#searchbox}
:::

::: {.cell .tag_remove-input .docutils .container}
:::

::: {#the-process-a-virtual-computer .section .tex2jax_ignore .mathjax_ignore}
[]{#cont-vp-process}

# [7. ]{.section-number}The Process: A virtual Computer[\#](#the-process-a-virtual-computer "Link to this heading"){.headerlink}

A process is a virtual computer than encapsulates CPU state for execution context, a virtual memory abstraction of massive contiguous memory that starts at address `0x0`{.docutils .literal .notranslate}, and state needed to interact with other processes and read/write state from file system.

::: {#the-interface .section}
## [7.1. ]{.section-number}The interface[\#](#the-interface "Link to this heading"){.headerlink}

The key system calls in traditional Unix related to processes are:

-   `pid = fork(void)`{.docutils .literal .notranslate}: Create a child process that is a duplicate of the parent; return 0 in child, and `PID`{.docutils .literal .notranslate} of child in parent.

-   `exit(status)`{.docutils .literal .notranslate}: Terminate the calling process and record the status passed in for others.

-   `pid = waitpid(cpid, *status...)`{.docutils .literal .notranslate}: Wait for specified child process `cpid`{.docutils .literal .notranslate} to complete (or change state), fill `*status`{.docutils .literal .notranslate} with the status passed on child's exit, and garbage collect any kernel resources; return the `PID`{.docutils .literal .notranslate} of the child process that exited (or changed state).

-   `err = execve(program, arguments, environment)`{.docutils .literal .notranslate}: executing the file `program`{.docutils .literal .notranslate} with specified arguments and environment information

The `fork`{.docutils .literal .notranslate} system call duplicates the calling process (referred to as the *parent*) into a new *child* process, where the only difference that enables the parent and child to distinguish themself is the return value. You can think of this logically as creating a copy of all the process memory, copying the CPU state, and copying the file descriptor table (while incrementing reference counts on all the files pointed to by the file descriptor table).

A process has a large amount of state associated with it. Linux implements `fork`{.docutils .literal .notranslate} in a library on top of the lower level `clone`{.docutils .literal .notranslate} call that lets the calling program control what part of the state is copied to the child. As we will see, this enables the same system call to be used to both create processes, and create threads within those processes.

Fork is usually quickly followed by a call to `exec`{.docutils .literal .notranslate} to execute a new program. One of the often claimed *elegant* design decisions of unix is that after a fork, the child has fine grained control to change file descriptor state before calling `exec`{.docutils .literal .notranslate}; that is, the same functionality that is used for normal access to files is used by the shell between fork and exec to set up he child.

Some of the authors have argued that fork was a clever hack for machines and programs of the 1970s that has long outlived its usefulness and is now a liability [\[[BAKR19](../misc/bib.html#id3 "Andrew Baumann, Jonathan Appavoo, Orran Krieger, and Timothy Roscoe. A fork() in the road. In Proceedings of the Workshop on Hot Topics in Operating Systems, HotOS '19, 14–22. New York, NY, USA, 2019. Association for Computing Machinery. URL: https://doi.org/10.1145/3317550.3321435, doi:10.1145/3317550.3321435."){.reference .internal}\]]{#id1}. Many operating systems provide powerful primitives to control the launching of new programs without an intervening `fork`{.docutils .literal .notranslate}, and fork imposes design constraints and overheads that these alternatives don't have. Even on Linux for many use cases, `posix_spawn`{.docutils .literal .notranslate} combines the functionality of `fork`{.docutils .literal .notranslate} and `exec`{.docutils .literal .notranslate}. However, `posix_spawn`{.docutils .literal .notranslate} is on Linux implemented on top of clone, so it doesn't actually alleviate the author's concerns.

Heresy "fork is a clever hack that has outlived its usefulness":

The paper "A fork in the road"[\[[BAKR19](../misc/bib.html#id3 "Andrew Baumann, Jonathan Appavoo, Orran Krieger, and Timothy Roscoe. A fork() in the road. In Proceedings of the Workshop on Hot Topics in Operating Systems, HotOS '19, 14–22. New York, NY, USA, 2019. Association for Computing Machinery. URL: https://doi.org/10.1145/3317550.3321435, doi:10.1145/3317550.3321435."){.reference .internal}\]]{#id2}, resulted in thousands and thousands of heated posts on a range of public forums. You can see some of the debate between Orran Krieger and a well known Linux architect Uli Drepper [here](https://www.bu.edu/rhcollab/2019/04/11/a-fork-in-the-road/){.reference .external}, along with links to the public forums. While those of us that wrote the paper still assert `fork`{.docutils .literal .notranslate} is a poor idea, we will use this opportunity to assert that we much prefer Linux to windows and we are in fact not "Microsoft stooges".

There are actually many more interfaces supported by systems like Linux related to process management. You can, for example, send a signal (e.g., to stop or kill) a process using:

-   `kill(pid_t pid, int sig)`{.docutils .literal .notranslate}: Send a signal to a process or group of processes

Some of these interfaces are actual system calls and are in section 2 of the man pages, others are implemented in a library; you can, for example type `man -k exec`{.docutils .literal .notranslate} to find out which man pages relate to exec. If you type `man 3 exec`{.docutils .literal .notranslate} you will find a whole series of higher level functions built on top of `execve`{.docutils .literal .notranslate}.
:::

::: {#process-versus-program .section}
## [7.2. ]{.section-number}Process versus Program[\#](#process-versus-program "Link to this heading"){.headerlink}

It is important to understand the difference between a program and a process. A program is a executable file, generated by a compiler and linker, that can be executed using `exec`{.docutils .literal .notranslate}. The `exec`{.docutils .literal .notranslate} system call then populates the memory region of the process with information pulled out of that program and there can be many processes, by many users, running the same program.

To understand how the portions of the executable file are used by the process, consider the following trivial program that runs an infinite loop so we can examine it while it is running.

::: {#while-one-listing .literal-block-wrapper .docutils .container}
::: code-block-caption
[Listing 7.1 ]{.caption-number}[wo.c - A simple program that loops forever]{.caption-text}[\#](#while-one-listing "Link to this code"){.headerlink}
:::

::: {.highlight-c .notranslate}
::: highlight
    1int main() {
    2  while(1);
    3}
:::
:::
:::

If we compile this program, run it, I can use the synthetic file system "/proc/PID/maps" to ask Linux about what is mapped in different parts of the application address space. Node, in bash the variable `$!`{.docutils .literal .notranslate} is the pid of the last started process.

::: {.admonition .note}
Note

Fields when looking at /proc/PID/maps:

-   address: This is the starting and ending address of the region in the process's address space

-   permissions - This describes how pages in the region can be accessed. There are four different permissions: read, write, execute, and shared. If a region is not shared, it is private, so a p will appear instead of an s.

-   offset - If the region was mapped from a file (using mmap), this is the offset in the file where the mapping begins. If the memory was not mapped from a file, it's just 0.

-   device - If the region was mapped from a file, this is the major and minor device number (in hex) where the file lives.

-   inode - If the region was mapped from a file, this is the file number.

-   pathname - If the region was mapped from a file, this is the name of the file. Otherwise, for special regions like the heap, stack... this field identifies the use.
:::

::: {.cell .tag_remove-input .tag_hide-output .docutils .container}
:::

::: {.cell .tag_remove-input .docutils .container}
::: {.cell_output .docutils .container}
:::
:::

We can see that the first five regions of the process come directly from the file. We can use the `objdump`{.docutils .literal .notranslate} utility to print the different sections of the executable file, as shown below, where the second column `Name`{.docutils .literal .notranslate} describes that part of the file, and the fourth column `VMA`{.docutils .literal .notranslate} is the virtual memory address that should be loaded from the program. If you scroll through that information, you can see that the executable parts of the program (`.init`{.docutils .literal .notranslate}, `.plt `{.docutils .literal .notranslate}and `.text`{.docutils .literal .notranslate}) is loaded into the memory with executable permission. The `.rodata`{.docutils .literal .notranslate} is mapped into memory right after that, etc... All these regions have the **p**, or private, flag set in the permissions on the map, meaning that the operating system is creating a copy of the information from the file, so many processes can run the same program, and any writes they make to the corresponding memory will not be visible to other processes executing the same program.

::: {.cell .tag_remove-input .tag_output_scroll .docutils .container}
::: {.cell_output .docutils .container}
:::
:::
:::
:::

::: prev-next-area
[](intro.html "previous page"){.left-prev}

::: prev-next-info
previous

[6. ]{.section-number}Introduction
:::

[](virtual.html "next page"){.right-next}

::: prev-next-info
next

[8. ]{.section-number}Virtualizing the CPU
:::
:::
:::

::: {.bd-sidebar-secondary .bd-toc}
::: {.sidebar-secondary-items .sidebar-secondary__inner}
::: sidebar-secondary-item
::: {.page-toc .tocsection .onthispage}
Contents
:::

-   [7.1. The interface](#the-interface){.reference .internal .nav-link}
-   [7.2. Process versus Program](#process-versus-program){.reference .internal .nav-link}
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
