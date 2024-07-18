---
docsearch:language: en
lang: en
title: 2. Purpose of operating systems --- Introduction to Operating Systems
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
- [2. Purpose of operating systems](#){.current .reference .internal}
- [3. Operating System Structure & Unix/Linux](structure.html){.reference .internal}
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

- [[ ![JupyterHub logo](../_static/images/logo_jupyterhub.svg) ]{.btn__icon-container} [JupyterHub]{.btn__text-container}](https://jupyterhub-opf-jupyterhub.apps.smaug.na.operate-first.cloud/hub/user-redirect/git-pull?repo=https%3A//github.com/OpenOSOrg/openos&urlpath=lab/tree/openos/content/intro/purpose.ipynb&branch=main "Launch on JupyterHub"){.btn .btn-sm .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
  :::

::: {.dropdown .dropdown-source-buttons}

- [[ ]{.btn__icon-container} [Repository]{.btn__text-container}](https://github.com/OpenOSOrg/openos "Source repository"){.btn .btn-sm .btn-source-repository-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
- [[ ]{.btn__icon-container} [Suggest edit]{.btn__text-container}](https://github.com/OpenOSOrg/openos/edit/main/content/intro/purpose.ipynb "Suggest edit"){.btn .btn-sm .btn-source-edit-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
- [[ ]{.btn__icon-container} [Open issue]{.btn__text-container}](https://github.com/OpenOSOrg/openos/issues/new?title=Issue%20on%20page%20%2Fintro/purpose.html&body=Your%20issue%20content%20here. "Open an issue"){.btn .btn-sm .btn-source-issues-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
  :::

::: {.dropdown .dropdown-download-buttons}

- [[ ]{.btn__icon-container} [.ipynb]{.btn__text-container}](../_sources/intro/purpose.ipynb "Download source file"){.btn .btn-sm .btn-download-source-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}

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

# Purpose of operating systems

::: {#print-main-content}
::: {#jb-print-toc}

<div>

## Contents

</div>

- [2.1. A simple model of hardware](#a-simple-model-of-hardware){.reference .internal .nav-link}
- [2.2. The fundamental platform](#the-fundamental-platform){.reference .internal .nav-link}
  - [2.2.1. Abstracting Hardware](#abstracting-hardware){.reference .internal .nav-link}
  - [2.2.2. Enabling diverse hardware](#enabling-diverse-hardware){.reference .internal .nav-link}
  - [2.2.3. Sharing the hardware](#sharing-the-hardware){.reference .internal .nav-link}
  - [2.2.4. Supporting many users](#supporting-many-users){.reference .internal .nav-link}
  - [2.2.5. Protecting from external attacks](#protecting-from-external-attacks){.reference .internal .nav-link}
  - [2.2.6. Management](#management){.reference .internal .nav-link}
  - [2.2.7. Supporting devices](#supporting-devices){.reference .internal .nav-link}
  - [2.2.8. Putting it together](#putting-it-together){.reference .internal .nav-link}
- [2.3. So why do we care](#so-why-do-we-care){.reference .internal .nav-link}
- [2.4. Is the fun over?](#is-the-fun-over){.reference .internal .nav-link}
  :::
  :::
  :::

::: {#searchbox}
:::

::: {#purpose-of-operating-systems .section .tex2jax_ignore .mathjax_ignore}
[]{#cont-gs-purpose}

# [2. ] {.section-number}Purpose of operating systems[\#](#purpose-of-operating-systems "Link to this heading") {.headerlink}

The purpose of an operating system is to provide everything needed to enable applications to run on computers. We [[first]{.std .std-ref}](#cont-gs-purpose-hw){.reference .internal} present a simple model of hardware and why the OS is needed, then discuss how operating systems are the [[fundamental platform]{.std .std-ref}](#cont-gs-purpose-platform){.reference .internal} that all computing depends on. We then discuss why developing a fundamental understanding of operating systems is [[important]{.std .std-ref}](#cont-gs-purpose-care){.reference .internal} and how now is such an [[exciting time]{.std .std-ref}](#cont-gs-purpose-care){.reference .internal} to be doing research or development in operating systems.

We understand that studying operating systems is hard. Our hope is that at the end of this chapter you will realize why this course is so important for you as a computer scientist or engineer. Also, we hope a few of you will get excited about the area and consider joining our community of OS developers and researchers. Consider that today's dominant operating systems are open source and rely on 1000s of contributors from all over the world, many of whom volunteer their time.

::: {#a-simple-model-of-hardware .section}
[]{#cont-gs-purpose-hw}

## [2.1. ] {.section-number}A simple model of hardware[\#](#a-simple-model-of-hardware "Link to this heading") {.headerlink}

The fundamental job of the operating system is to enable applications to run on a computer. To understand why this is complicated, consider the very simple model of a computer depicted in [[Fig. 2.1]{.std .std-numref}](#simplecomputer-fig){.reference .internal}. We briefly describe each of the key components of this computer, and what you need to know for now.

![[Fig. 2.1 ]{.caption-number}[A simple model of a computer. The CPU is connected to high speed memory, and through a lower speed bus to a network controller and disk controller that are in turn connected to a network (ethernet in this case) and a disk.]{.caption-text}[\#](#simplecomputer-fig "Link to this image"){.headerlink}](../_images/hardware.png){style="width: 50%;"}

- **Central Processing Unit (CPU)**: The smart part that executes instructions is called the Central Processing Unit (CPU) or **processor**. In our simple model, these instructions operate by modifying the contents of various processor registers, loading new register contents from memory, or storing register contents into memory.
- **Memory:** Also referred to as **Random Access Memory (RAM)**, holds the instructions and data that applications require as they execute. It is physically connected to the CPU via direct wiring. Random access here refers to the fact that the processor can directly load or store any memory location (addressed as an 8-bit byte) in the same amount of time. Memory today is normally volatile, meaning that its contents are lost when the computer is powered off.
- **I/O bus:** If the CPU wasn't connected to anything but RAM, you couldn't do much with it. All computers have some form of Input/Output (or I/O) bus that connects the CPU and RAM to different devices. While there are many kinds of I/O devices, for now we will ignore everything but: 1) storage, and 2) networks. The processor typically talks to an I/O device by loading and storing registers on a controller specific to the device, and that controller in turn communicates with the corresponding device(s) and transfers data between the device and memory.
- **Storage:** Since the memory is typically volatile, computers have to have some form of storage that is non-volatile or *persistent*. This may include hard disk drives (HDDs), solid state drives (SSDs), optical drives, usb sticks, etc. Most storage devices are accessed at a block granularity (e.g., 512 or 4096 bytes), meaning that entire blocks are transferred between storage and memory. Most storage devices are not **Random Access**, for example, technologies like a hard disk drive require the disk head to physically move to the storage location on the disk before reading or writing the data. When the processor wants to read or write a block of disk, it tells the storage controller the block of disk to transfer to or from memory, and the storage controller notifies the processor when the operation is complete.
- **Networking:** To talk to the outside world computers are normally connected to some network, typically ethernet today, where data is transferred between memory and the network in some form of packet as shown in [[Fig. 2.2]{.std .std-numref}](#ethernet-packet){.reference .internal}. When the processor wants to send a message over the network, it first prepares a packet in memory, and then tells the network controller to send it. When new packets arrive over the network, the controller copies them into memory, and then tells the processor (in some fashion) that a new packet is available to be processed.

![[Fig. 2.2 ]{.caption-number}[A ethernet packet is organized into a frame, which includes the destination of the frame, the address of the sender, the length of the entire frame, the data or payload, and a 32-bit hash (the CRC) of the rest of the contents that can be used to check if the packet has been corrupted in transit.]{.caption-text}[\#](#ethernet-packet "Link to this image"){.headerlink}](../_images/ethernet-frame.png){style="width: 80%;"}

::: {.admonition .note}
Note

Note this model is highly abstracted and very simple. As we will learn later in the course:

- modern processors can execute hundreds of instructions in parallel, and modern computers can be composed of many processors;
- memory today is organized in Non-Uniform Memory Access (NUMA) where some memory is closer to some processors; so it is not really random access;
- memory today is very slow compared to the processor, and normally there are multiple layers of **cache** so that the CPU doesn't have to wait for the slow memory every time it needs to fetch an instruction to execute;
- and other examples that may arise.
  :::
  :::

::: {#the-fundamental-platform .section}
[]{#cont-gs-purpose-platform}

## [2.2. ] {.section-number}The fundamental platform[\#](#the-fundamental-platform "Link to this heading") {.headerlink}

What makes operating systems so interesting is that they are the fundamental platform on which all other software is written. We briefly discuss each of their core tasks.

![[Fig. 2.3 ]{.caption-number}[Providing interfaces that applications can use on top of the complicated interfaces of today's hardware.]{.caption-text}[\#](#mappingint-fig "Link to this image"){.headerlink}](../_images/purpose-OS-source-03.drawio.png){style="width: 200pt;"}

::: {#abstracting-hardware .section}
[]{#cont-gs-purpose-platform-abs}

### [2.2.1. ] {.section-number}Abstracting Hardware[\#](#abstracting-hardware "Link to this heading") {.headerlink}

If applications needed to understand all the complicated hardware described [[above]{.std .std-ref}](#cont-gs-purpose-hw){.reference .internal}, many fewer applications would be written. Consider, for example, storage: the abstraction provided by the hardware is disk blocks, while applications that persist data want to work with higher-level abstractions like directories and files.

As shown in [[Fig. 2.3]{.std .std-numref}](#mappingint-fig){.reference .internal}, the most important job of the operating system is to enable a set of higher level abstractions, often called **"virtual abstractions"** on top of the low-level primitive "physical abstractions" provided by the hardware. That is, the operating system translates physical abstractions to virtual/clean ones that applications can be written to. Key virtual abstractions we will discuss include:

- **Process:** An abstraction of computer, where every time a **program** is started it executes as a separate process.
- **Files:** An abstraction of I/O, enabling processes to persist data in non-volatile storage and communicate with different processes.
- **Virtual memory:** An abstraction of the memory that a process can access.

::: {.cell .tag_hide-input .tag_margin .tag_hide-output .docutils .container}
[Show code cell source]{.collapsed} [Hide code cell source]{.expanded}

::: {.cell_input .above-output-prompt .docutils .container}
::: {.highlight-ipython3 .notranslate}
::: highlight
bash.run("ps -e")
:::
:::
:::

[Show code cell output]{.collapsed} [Hide code cell output]{.expanded}

::: {.cell_output .docutils .container}
:::
:::

::: {.admonition-process-versus-program .admonition}
Process versus Program

It is important to understand the difference between programs and processes. When a user wants to run an application, or **program**, the operating system creates a new process and loads the program instructions from storage into memory for the process to execute. There can be multiple processes executing the same program that are running at the same time. For example, while I am writing this book, when I type "ps -e" to tell me all the processes currently running, (see margin) I find that I have multiple "bash" shells running at the same time, a large number of "python" programs, and of course the "ps" program itself. We will describe this Unix command more later.
:::

![[Fig. 2.4 ]{.caption-number}[Different kinds of computers]{.caption-text}[\#](#hw-fig "Link to this image"){.headerlink}](../_images/purpose-OS-source-06.drawio.png){style="width: 200pt;"}
:::

::: {#enabling-diverse-hardware .section}
[]{#cont-gs-purpose-platform-hwdiv}

### [2.2.2. ] {.section-number}Enabling diverse hardware[\#](#enabling-diverse-hardware "Link to this heading") {.headerlink}

Operating systems must support diverse computer systems ([[Fig. 2.4]{.std .std-numref}](#hw-fig){.reference .internal}), ranging from tiny embedded systems in a smart fridge to massive high-performance computing systems that occupy large portions of a data center. Systems differ in the type of processors (e.g. x86, Power, ARM, RISC6), the devices, and the scale of resources like processors, memory and storage. For example, a [smart watch](https://www.pcmag.com/news/pine64s-30-linux-smartwatch-launches){.reference .external} may have just 64 kilobytes of memory whereas a set of new servers just obtained by the Mass Open Cloud have four terabytes of memory, where a terabyte is 1,073,741,824 kilobytes ([\\(2\^{40}\\)]{.math .notranslate .nohighlight}).

Abbreviations, Definitions and Notation:

Remember that numbers in computer systems are typically presented as a power of two, for example 1 kilobyte = [\\(2\^{10}\\)]{.math .notranslate .nohighlight} bytes = 1024 bytes. We will be using the common abbreviations for units as shown in the table below:

::: pst-scrollable-table-container
Value                                                        Binary Prefix   Abbreviation

---

[\\(1024 = 2\^{10}\\)]{.math .notranslate .nohighlight}      kilo            K
[\\(1024\^2 = 2\^{20}\\)]{.math .notranslate .nohighlight}   mega            M
[\\(1024\^3 = 2\^{30}\\)]{.math .notranslate .nohighlight}   giga            G
[\\(1024\^4 = 2\^{40}\\)]{.math .notranslate .nohighlight}   tera            T
[\\(1024\^5 = 2\^{50}\\)]{.math .notranslate .nohighlight}   peta            P
:::

In units, "bytes" are abbreviated with an upper-case B and "bits" with a lower-case b, so 1 kilobyte = 1 KB = 8 Kb.

Operating systems provide the same (or similar) [[virtual abstractions]{.std .std-ref}](#cont-gs-purpose-platform-abs){.reference .internal} across these very different systems, enabling many of their differences to be hidden from most applications. This makes it easy to write libraries and applications (e.g., Netflix) that can run on systems as diverse as PCs, phones, ipads, and smart cars. This, in turn, makes it possible for hardware designers to innovate, introducing new computers and even processors, while knowing that many applications will be able to use their systems.

In fact, today, the same open source Linux OS runs on cell phones, massive High Performance Computing systems, and drones delivering Amazon packages. As we will discuss, the open source nature of the system enables companies that want to innovate to make changes to the operating system to support their hardware.

While the OS enables applications to be easily ported from one hardware platform to another, the OS is also responsible for meeting the fundamental requirements of the systems it supports. In a cell phone, the OS needs to ensure that everything works in a tiny amount of memory, with limited energy use, while the OS for a server may use terabytes of memory to cache storage and allow many programs to be resident simultaneously. In a drone, one probably wants to make sure that a non-critical program can't impact the hard real-time programs controlling the propellers.
:::

::: {#sharing-the-hardware .section}
[]{#cont-gs-purpose-platform-multi}

### [2.2.3. ] {.section-number}Sharing the hardware[\#](#sharing-the-hardware "Link to this heading") {.headerlink}

![[Fig. 2.5 ]{.caption-number}[Multiple processes.]{.caption-text}[\#](#multipleapps-fig "Link to this image"){.headerlink}](../_images/purpose-OS-source-04.drawio.png){style="width: 200pt;"}

Modern operating systems enable many (thousands) of processes running different programs/applications to run at the same time ([[Fig. 2.5]{.std .std-numref}](#multipleapps-fig){.reference .internal}). The operating system needs to ensure that processes can't break each other. For example, the operating system must guarantee that a bug in an application, or even an application written by a malicious programmer, can't modify the memory of other processes.

The OS should also ensure that each process gets its fair share of the different resources of the computer consistent with their requirements. To understand what we mean by different requirements, consider two programs: an editor needs to be responsive to you as you type characters, while a compiler tries to use as much processing and disk as possible to get its work done quickly. The OS should ensure that the compiler gets to use most of the resources of the computer while reserving the limited resources that the editor requires and prioritizing the editor whenever you type a character. It has to do that without typically knowing what the requirements of the applications are.

To share the resources of the computer, the operating system multiplexes the resources in space, time or both. An example of space multiplexing is using different disk blocks to store the contents of different files. An example of time multiplexing is changing which process is running on a processor. In many cases, both are used to manage the same type of resource. For example, at a given time different processes are given access to different regions of the memory (space multiplexing), but over time a given region of memory may be used by different processes as their needs for memory change (time multiplexing).
:::

::: {#supporting-many-users .section}
[]{#cont-gs-purpose-platform-security}

### [2.2.4. ] {.section-number}Supporting many users[\#](#supporting-many-users "Link to this heading") {.headerlink}

![[Fig. 2.6 ]{.caption-number}[Multiple users]{.caption-text}[\#](#sec-fig "Link to this image"){.headerlink}](../_images/purpose-OS-source-05.drawio.png){style="width: 200pt;"}

Normally, operating systems are designed to support different users running processes at the same time. The OS must make sure that one user can't run processes that change, or even read, the files of another user. Moreover, the OS may need to make sure that each user gets their fair share of the computer; for example, ensuring that a student can't launch 1000 processes after they are done an assignment to keep classmates from successfully submitting theirs.

This protection is part of the security policies and mechanisms of the operating system. Attacks may try to violate confidentiality (one can see another user's information), integrity (one can change state of another user), or availability (one can deny other users the ability to run their programs). While OS developers have put enormous work into designing secure systems, the complexity of modern systems give operating system researchers strong job security.
:::

::: {#protecting-from-external-attacks .section}
[]{#cont-gs-purpose-platform-sec-outside}

### [2.2.5. ] {.section-number}Protecting from external attacks[\#](#protecting-from-external-attacks "Link to this heading") {.headerlink}

The best way to keep users from attacking each other is to make sure that they can't run on the same computer. In fact, in the good old days, we used to make sure that computers were disconnected from each other. For example, professors had their accounts on computers that students had no access to.

![[Fig. 2.7 ]{.caption-number}[Protecting users from outside world.]{.caption-text}[\#](#secoutside-fig "Link to this image"){.headerlink}](../_images/purpose-OS-source-07.drawio.png){style="width: 300pt;"}

Today we do all our work connected to the network, and we log into our machines remotely. In fact, right now I am typing this sentence on a laptop that is connected to a network; every key stroke I type is being sent over a network to a cloud service running containers reserved by me on a computer in a datacenter 100 miles away from my laptop. The operating system implements firewalls and security policies that make sure that only I can change this book.

While we work hard to protect computers from external attacks, new attacks are always being developed, there are always bugs in the operating system, and humans often expose passwords or make mistakes that render the computers they work on open to attacks. The OS is responsible for logging all the information needed so that we can later figure out who hacked the system, and what changes they made.

![[Fig. 2.8 ]{.caption-number}[Enabling management.]{.caption-text}[\#](#mgment-fig "Link to this image"){.headerlink}](../_images/purpose-OS-source-08.drawio.png){style="width: 300pt;"}
:::

::: {#management .section}
[]{#cont-gs-purpose-platform-mgmt}

### [2.2.6. ] {.section-number}Management[\#](#management "Link to this heading") {.headerlink}

There is a huge diversity of systems, from embedded devices to personal computers, cloud data centers, and HPC environments. If a human being was responsible for manually configuring, upgrading, and patching all these systems (which used to be the case), we wouldn't have enough people in the world.

The tools and capabilities provided in the OS give the mechanism for administrators to automate these activities at massive scale. These mechanisms also allow the operating system to be customized and even specialized to the workload it is expected to run.

![[Fig. 2.9 ]{.caption-number}[Supporting devices]{.caption-text}[\#](#devs-fig "Link to this image"){.headerlink}](../_images/purpose-OS-source-12.drawio.png){style="width: 300pt;"}
:::

::: {#supporting-devices .section}
[]{#cont-gs-purpose-platform-devs}

### [2.2.7. ] {.section-number}Supporting devices[\#](#supporting-devices "Link to this heading") {.headerlink}

Last, but certainly not least, the OS not only directly manages the hardware of a computer, but also a massive number of peripheral devices, including disks, monitors, keyboards, network connections, cameras and more. Often when a new device is developed, the developers need to provide some way to plumb it through the operating system so that applications will be able to take advantage of it. As we will discuss, **device drivers** are the vast majority of software in today's operating system.
:::

::: {#putting-it-together .section}
[]{#cont-gs-purpose-platform-together}

### [2.2.8. ] {.section-number}Putting it together[\#](#putting-it-together "Link to this heading") {.headerlink}

So, to summarize, the operating system is responsible for:

- Creating the fundamental **virtual** abstractions that applications are written to use on top of the primitive abstractions provided by hardware. This enables applications to be written without detailed understanding of the hardware, which in turn enables computer system and device developers to develop new hardware that applications can just use.
- Managing and multiplexing the hardware resources to support diverse workloads by many users across a broad set of use cases from supercomputers to cell phones. This includes providing the interfaces and tools that operators use to manage their systems.
- Protecting processes/users from both internal and external attacks and keeping activity logs.

In other words, operating systems are the fundamental platforms that all other software and hardware relies on and that people use to interact with the software and hardware.
:::
:::

::: {#so-why-do-we-care .section}
[]{#cont-gs-purpose-care}

## [2.3. ] {.section-number}So why do we care[\#](#so-why-do-we-care "Link to this heading") {.headerlink}

In all fields, if you control the platform that others need to use, you have an enormous advantage. For example, if you control the exchange that others use for trading stocks, [cryptocurrency](https://www.investopedia.com/what-went-wrong-with-ftx-6828447){.reference .external} or goods (e.g., [Amazon](https://www.amazon.com){.reference .external} and [etsy](https://www.etsy.com){.reference .external}) you are in a position to (properly or not) gain something from every use of the platform, and you have a special responsibility to all the users. As the fundamental platform in computing, we see that operating systems have played a huge role. For example:

1. Operating systems have been the focus, and responsible for the success, of some of the world's largest companies, e.g. Microsoft, VMware, Red Hat.
2. Operating system people play a key role in every major technology company.
3. Every major change in technology requires innovation or at least changes at the operating system level.
4. Operating system researchers, and their venues (e.g., SOSP, OSDI, Eurosys, Usenix) are responsible for the major distributed system innovations.
5. The world of open source, that has impacted all elements of society, started with operating systems.

Fundamentally, if you care about computing, you better care about operating systems and have some idea of how they work. If you want to develop applications, you need to understand the OS abstractions, and good performance often relies on understanding something about the policies and implementation of the OS you are using. If you want to develop new hardware, you need to understand how to expose that hardware through the OS to the applications that want to use it. If you just want to use computers, you need to understanding the fundamental capabilities and protections that the operating system can provide to secure and manage the hardware.
:::

::: {#is-the-fun-over .section}
[]{#cont-gs-purpose-fun}

## [2.4. ] {.section-number}Is the fun over?[\#](#is-the-fun-over "Link to this heading") {.headerlink}

We have been working on operating systems for as long as we have had computers. In many fields, innovation happens rapidly for a while, and then the excitement moves to another area. With operating systems, not only do they continue to be a major area of innovation, but we expect that the need for innovation in operating systems, and even development of new ones, will continue and accelerate.

Fundamentally, OS innovation is needed for any major change in application requirements, hardware capabilities, or new use cases. Consider some of the major changes that are happening now:

- The rise of cloud computing is resulting in new models of OS for services and functions that require "logical" computers to be instantiated in seconds, and demand strong guarantees on tail latency (i.e., most requests finish in some guaranteed time).
- Fundamental change in security requirements; provider/tenant
- [Denard scaling](https://en.wikipedia.org/wiki/Dennard_scaling){.reference .external} is over; but network and storage keep getting faster...
- [Edge computing](https://www.equinix.com/resources/analyst-reports/gartner-distributed-enterprise-predictions-2022?ls=Advertising%20-%20Web&lsd=22q1_enterprise_digital-infrastructure--not-applicable_/resources/analyst-reports/gartner-distributed-enterprise-predictions-2022_dm_obility_paid-search_google_us-en_AMER_digital-edge_demand-gen&utm_campaign=us-en_google_paid-search_digital-edge_dm&utm_source=google&utm_medium=paid-search&utm_content=digital-infrastructure--not-applicable_gartner-distributed-enterprise-predictions-2022&gclid=CjwKCAiAzKqdBhAnEiwAePEjkjhC-gGejQAFyu-KiGw3oeqhkMvU9hfJkoBx5hH9hdT_rArJOehavxoC8nYQAvD_BwE){.reference .external} & [Cloudlets](https://www.sciencedirect.com/topics/computer-science/cloudlet){.reference .external} driven by the emergence of high bandwidth low latency [5G](https://www.qualcomm.com/5g/what-is-5g){.reference .external} will drive a whole new model of compute.
- While persistent memory has been promised for decades a few years ago the first products became available. (and [just got cancelled](https://www.forbes.com/sites/tomcoughlin/2022/07/28/intel-winding-down-its-optane-memory-business/?sh=37b8653345b8){.reference .external})
- Rise of smart NICs where intelligence is embedded into the devices, enabling new models to offload computation to the network; e.g. high speed trading, security, accounting cloud...
- 100 GB networks spanning the world..
- Rise of AI...

Unfortunately, for some reason many engineers and computer scientists are intimidated to work at the operating system level, and many think of the OS as underlying plumbing with the fun stuff around it. We hope that this chapter has motivated you to understand why operating systems are not only historically interesting, but will continue to be a major area of innovation, and that this this course will start you on the path to mastering this exciting and important topic.
:::
:::

::: prev-next-area
[](intro.html "previous page"){.left-prev}

::: prev-next-info
previous

[1. ]{.section-number}Introduction
:::

[](structure.html "next page"){.right-next}

::: prev-next-info
next

[3. ]{.section-number}Operating System Structure & Unix/Linux
:::
:::
:::

::: {.bd-sidebar-secondary .bd-toc}
::: {.sidebar-secondary-items .sidebar-secondary__inner}
::: sidebar-secondary-item
::: {.page-toc .tocsection .onthispage}
Contents
:::

- [2.1. A simple model of hardware](#a-simple-model-of-hardware){.reference .internal .nav-link}
- [2.2. The fundamental platform](#the-fundamental-platform){.reference .internal .nav-link}
  - [2.2.1. Abstracting Hardware](#abstracting-hardware){.reference .internal .nav-link}
  - [2.2.2. Enabling diverse hardware](#enabling-diverse-hardware){.reference .internal .nav-link}
  - [2.2.3. Sharing the hardware](#sharing-the-hardware){.reference .internal .nav-link}
  - [2.2.4. Supporting many users](#supporting-many-users){.reference .internal .nav-link}
  - [2.2.5. Protecting from external attacks](#protecting-from-external-attacks){.reference .internal .nav-link}
  - [2.2.6. Management](#management){.reference .internal .nav-link}
  - [2.2.7. Supporting devices](#supporting-devices){.reference .internal .nav-link}
  - [2.2.8. Putting it together](#putting-it-together){.reference .internal .nav-link}
- [2.3. So why do we care](#so-why-do-we-care){.reference .internal .nav-link}
- [2.4. Is the fun over?](#is-the-fun-over){.reference .internal .nav-link}
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
