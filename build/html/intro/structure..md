---
docsearch:language: en
lang: en
title: 3. Operating System Structure & Unix/Linux --- Introduction to Operating Systems
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
[![Introduction to Operating Systems - Home](../_static/logo.png){.logo__image .only-light}](pref.html){.navbar-brand .logo}
:::

::: sidebar-primary-item
:::

::: sidebar-primary-item
::: {.bd-toc-item .navbar-nav .active}

- [Preface](pref.html){.reference .internal}

[Getting started]{.caption-text}

- [1. Introduction](intro.html){.reference .internal}
- [2. Purpose of operating systems](purpose.html){.reference .internal}
- [3. Operating System Structure & Unix/Linux](#){.current .reference .internal}
- [4. Operating System Abstractions](abstractions.html){.reference .internal}
- [5. What you should know](tools.html){.reference .internal}
  []{.toctree-toggle role="presentation"}
  - [5.1. The C Programming Language](tools-c.html){.reference .internal}
  - [5.2. Shell](tools-shell.html){.reference .internal}
  - [5.3. Editors](tools-editors.html){.reference .internal}
  - [5.4. Make](tools-make.html){.reference .internal}
  - [5.5. Testing](tools-testing.html){.reference .internal}
  - [5.6. Git Basics](tools-git.html){.reference .internal}
  - [5.7. GDB](tools-gdb.html){.reference .internal}

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

- [[ ![JupyterHub logo](../_static/images/logo_jupyterhub.svg) ]{.btn__icon-container} [JupyterHub]{.btn__text-container}](https://jupyterhub-opf-jupyterhub.apps.smaug.na.operate-first.cloud/hub/user-redirect/git-pull?repo=https%3A//github.com/OpenOSOrg/openos&urlpath=lab/tree/openos/content/intro/structure.ipynb&branch=main "Launch on JupyterHub"){.btn .btn-sm .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
  :::

::: {.dropdown .dropdown-source-buttons}

- [[ ]{.btn__icon-container} [Repository]{.btn__text-container}](https://github.com/OpenOSOrg/openos "Source repository"){.btn .btn-sm .btn-source-repository-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
- [[ ]{.btn__icon-container} [Suggest edit]{.btn__text-container}](https://github.com/OpenOSOrg/openos/edit/main/content/intro/structure.ipynb "Suggest edit"){.btn .btn-sm .btn-source-edit-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
- [[ ]{.btn__icon-container} [Open issue]{.btn__text-container}](https://github.com/OpenOSOrg/openos/issues/new?title=Issue%20on%20page%20%2Fintro/structure.html&body=Your%20issue%20content%20here. "Open an issue"){.btn .btn-sm .btn-source-issues-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
  :::

::: {.dropdown .dropdown-download-buttons}

- [[ ]{.btn__icon-container} [.ipynb]{.btn__text-container}](../_sources/intro/structure.ipynb "Download source file"){.btn .btn-sm .btn-download-source-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}

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

# Operating System Structure & Unix/Linux

::: {#print-main-content}
::: {#jb-print-toc}

<div>

## Contents

</div>

- [3.1. Unix and Linux](#unix-and-linux){.reference .internal .nav-link}
- [3.2. OS Structure and services](#os-structure-and-services){.reference .internal .nav-link}
  :::
  :::
  :::

::: {#searchbox}
:::

::: {#operating-system-structure-unix-linux .section .tex2jax_ignore .mathjax_ignore}
[]{#cont-gs-structure}

# [3. ] {.section-number}Operating System Structure & Unix/Linux[\#](#operating-system-structure-unix-linux "Link to this heading") {.headerlink}

We [[first]{.std .std-ref}](#cont-gs-structure-linux){.reference .internal} discuss why we focus on Linux in this book, and [[then]{.std .std-ref}](#cont-gs-structure-struc){.reference .internal} discuss how systems like Linux are structured and how the core services are provided. The [[next]{.std .std-ref}](abstractions.html#cont-gs-abstractions){.reference .internal} chapter describes some of the key abstractions those services provide to applications.

::: {#unix-and-linux .section}
[]{#cont-gs-structure-linux}

## [3.1. ] {.section-number}Unix and Linux[\#](#unix-and-linux "Link to this heading") {.headerlink}

There are hundreds of operating systems that have been developed over the years, many of which are designed to hide most aspects of the computer from "normal" users. Those users mainly just want to use programs written by others. The interface of these operating systems tends to focus on graphics and visually oriented ways of interacting with programs. [![](../_images/Unix.gif){.align-right style="width: 25%;"}](../_images/Unix.gif){.reference .internal} Unix, on the other hand, assumes that its users are primarily programmers. Its design and collection of tools are not meant to be particularly user-friendly. Rather Unix is designed to allow programmers to be very productive and to support a broad range of programming tools.

UNIX, Unix or Unix-like?

We use all-caps UNIX to refer to the official UNIX operating system, and Unix to refer generically to all Unix-like operating systems that broadly follow the design of the original UNIX. Refer to [The Linux Information Project](http://www.linfo.org/unix_upper.html){.reference .external} for more discussion of these distinctions.

While most elements of this book apply to most operating systems, for a number of reasons we typically focus on Unix, and, in particular, the *Linux* open source variant of Unix:

1. Even many operating systems like MacOS and Android, have a form of Unix or Linux at their core. If you want to really understand these systems, you need to understand Unix.
2. The [UNIX](https://www.opengroup.org/membership/forums/platform/unix){.reference .external} operating system was built by master programmers who valued programmability and productivity. In some sense learning to work on a Unix system is a right of passage that not only teaches you how to be productive on a computer running a Unix operating system, but also teaches you to think and act like a programmer.
3. Unix is designed with a core principle of small programs that can be composed through file system interfaces. You are encouraged to write little re-usable programs that you incrementally evolve as needed and combine with others to get big tasks done.
4. Unix's programming-oriented nature leads to an environment in which almost anything about the OS and user experience can be customized and programmed. Unix makes automation the name of the game -- largely everything you can do manually can be turned into a program that automates the task.
5. Linux, the dominant Unix today, is open source, enabling programmers and researchers to go deep into the code. Anyone can modify the operating system to support their system, or to enable their new workload.

Unix/Linux's programming-friendly nature has led to the development of a very large and rich body of existing software, with contributions from researchers, industry, students and hobbyists alike. This body of software has come to be a large scale shared repository of code, ideas, and programs that modern applications rely on heavily. As a result, the computer servers that form the core of the Internet and the Cloud largely run Linux. Many of the computers embedded in the devices that surround us from wifi routers, medical devices, automobiles, and everything else also often run a version of Linux. In fact, Android is, at its core, Linux.

> <div>
>
> [![](../_images/history.png){.align-left style="width: 60px;"}](../_images/history.png){.reference .internal}
>
> Unix recently celebrated its 50th year Anniversary.
> [50 Years of Unix](https://www.bell-labs.com/about/history/innovation-stories/50-years-unix/#gref){.reference .external}
> The people and its history are a fascinating journey into how we have gotten to where we are today.
> [The Strange birth and long life of Unix](https://spectrum.ieee.org/the-strange-birth-and-long-life-of-unix#toggle-gdpr){.reference .external}
> UNIX and its children literally make our digital world go around and will likely continue to do so for quite some time.
>
> </div>

:::

::: {#os-structure-and-services .section}
[]{#cont-gs-structure-struc}

## [3.2. ] {.section-number}OS Structure and services[\#](#os-structure-and-services "Link to this heading") {.headerlink}

![[Fig. 3.1 ]{.caption-number}[What's in a kernel]{.caption-text}[\#](#def-kernel "Link to this image"){.headerlink}](../_images/kerneldef.png){style="width: 300pt;"}

As stated [[earlier]{.std .std-ref}](purpose.html#cont-gs-purpose-platform-abs){.reference .internal}, operating systems provide a set of virtual abstractions on top of the primitive capabilities provided by hardware. Most operating systems today, and Linux in particular, provide these abstractions in the OS *kernel* (see [[Fig. 3.1]{.std .std-numref}](#def-kernel){.reference .internal}). The kernel runs at the highest permission level in the hardware, and can access any memory or device. All untrusted application code runs in *processes*, where any access to the real computer is controlled by the kernel.

The kernel controls the computer and provides the abstraction of *processes* for application code. You can think of a process as a virtual computer that uses unprivileged computer instructions and a set of [[abstractions]{.std .std-ref}](abstractions.html#cont-gs-abstractions){.reference .internal} provided by the kernel. The kernel provides each process: 1) an abstraction of an isolated CPU (while multiplexing it between different processes), 2) a *virtual memory* abstraction of massive contiguous memory that starts at address `0x0`{.docutils .literal .notranslate}, and 3) a set of file abstractions that allow the process to persist data and communicate with other processes.

![[Fig. 3.2 ]{.caption-number}[The kernel controls the computer and provides the abstraction of *processes* for application code.]{.caption-text}[\#](#os-struc "Link to this image"){.headerlink}](../_images/osstructure.syscall.drawio.png){style="width: 600pt;"}

Only the kernel can execute the privileged instructions that, for example, control the memory that a process can see, switch which process is currently running on a CPU, or control the I/O devices attached to the computer. While processes can only execute unpriviledged instructions, the kernel adds *logical* instructions to the process, called system calls, that can be used to create new processes, communicate with other processes/virtual computers, allocate memory, etc... These system calls are really special procedure calls that happen to switch to the kernel, and the process will stop executing until the kernel returns from the system call.

An *interrupt* is a signal that can be raised by I/O and other devices like timers that causes the CPU to start executing kernel code at some well-defined location. They are used to allow the kernel to respond in a timely fashion to I/O operations; even if an application is running for a long time the interrupt will stop the process and start executing the kernel, enabling it to notice that something has happened and to deal with it. Also, the kernel can schedule timer interrupts to enable it to gain back control every so often from processes to, for example, let other processes run.

Just as an interrupt informs the kernel that something has happened, the kernel provides a virtual abstraction called *signals* to let a process know that something has happened, where a signal causes the CPU to start executing at a handler specified by the application. This can be used, for example, to enable asynchronous I/O, to let a process know that other processes have died, etc...

![[Fig. 3.3 ]{.caption-number}[Core services]{.caption-text}[\#](#os-struc-services "Link to this image"){.headerlink}](../_images/osstructure.services.drawio.png){style="width: 600pt;"}

The different core services provided by the kernel (see [[Fig. 3.3]{.std .std-numref}](#os-struc-services){.reference .internal}) multiplex the resources of the computer in time and space. They maintain information about the running processes, schedule the processor, manage memory, implement file systems, and enable communication with other processes both on the same computer and, over the network, to other computers. A large part of the operating system is *device drivers*, which implement code specific to a particular type of hardware, and are often provided by the hardware developer.

As shown in [[Fig. 3.3]{.std .std-numref}](#os-struc-services){.reference .internal}, large portions of the kernel are dynamically loaded. This allows new devices to be attached to an already running kernel, e.g., if you plug a portable drive into your PC. When the kernel starts up, it discovers all the devices that exist, and figures out what kind of device drivers and file systems it needs and then gets them. Similarly, large portions of the applications are dynamically loaded libraries. Unless your application is really complicated, probably 90% of the code is actually libraries, and those libraries are loaded into the process by the operating system at run time to ensure that the most recent version of the library is used, and to allow all that memory used by library code to be shared across all the processes running on the computer.
:::
:::

::: prev-next-area
[](purpose.html "previous page"){.left-prev}

::: prev-next-info
previous

[2. ]{.section-number}Purpose of operating systems
:::

[](abstractions.html "next page"){.right-next}

::: prev-next-info
next

[4. ]{.section-number}Operating System Abstractions
:::
:::
:::

::: {.bd-sidebar-secondary .bd-toc}
::: {.sidebar-secondary-items .sidebar-secondary__inner}
::: sidebar-secondary-item
::: {.page-toc .tocsection .onthispage}
Contents
:::

- [3.1. Unix and Linux](#unix-and-linux){.reference .internal .nav-link}
- [3.2. OS Structure and services](#os-structure-and-services){.reference .internal .nav-link}
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
