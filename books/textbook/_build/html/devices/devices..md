---
docsearch:language: en
lang: en
title: 29. Input and Output --- Introduction to Operating Systems
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

- [29. Input and Output](#){.current .reference .internal}
- [30. More on Disks](disk2.html){.reference .internal}
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

- [[ ![JupyterHub logo](../_static/images/logo_jupyterhub.svg) ]{.btn__icon-container} [JupyterHub]{.btn__text-container}](https://jupyterhub-opf-jupyterhub.apps.smaug.na.operate-first.cloud/hub/user-redirect/git-pull?repo=https%3A//github.com/OpenOSOrg/openos&urlpath=lab/tree/openos/content/devices/devices.ipynb&branch=main "Launch on JupyterHub"){.btn .btn-sm .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
  :::

::: {.dropdown .dropdown-source-buttons}

- [[ ]{.btn__icon-container} [Repository]{.btn__text-container}](https://github.com/OpenOSOrg/openos "Source repository"){.btn .btn-sm .btn-source-repository-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
- [[ ]{.btn__icon-container} [Suggest edit]{.btn__text-container}](https://github.com/OpenOSOrg/openos/edit/main/content/devices/devices.ipynb "Suggest edit"){.btn .btn-sm .btn-source-edit-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
- [[ ]{.btn__icon-container} [Open issue]{.btn__text-container}](https://github.com/OpenOSOrg/openos/issues/new?title=Issue%20on%20page%20%2Fdevices/devices.html&body=Your%20issue%20content%20here. "Open an issue"){.btn .btn-sm .btn-source-issues-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
  :::

::: {.dropdown .dropdown-download-buttons}

- [[ ]{.btn__icon-container} [.ipynb]{.btn__text-container}](../_sources/devices/devices.ipynb "Download source file"){.btn .btn-sm .btn-download-source-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}

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

# Input and Output

::: {#print-main-content}
::: {#jb-print-toc}

<div>

## Contents

</div>

- [29.1. IO Hardware](#io-hardware){.reference .internal .nav-link}
  - [29.1.1. Structure of a computer](#structure-of-a-computer){.reference .internal .nav-link}
  - [29.1.2. Controllers](#controllers){.reference .internal .nav-link}
  - [29.1.3. Accessing the controller](#accessing-the-controller){.reference .internal .nav-link}
  - [29.1.4. Polled vs. Interrupt-driven I/O](#polled-vs-interrupt-driven-i-o){.reference .internal .nav-link}
  - [29.1.5. Interrupts](#interrupts){.reference .internal .nav-link}
  - [29.1.6. Direct Memory Access (DMA)](#direct-memory-access-dma){.reference .internal .nav-link}
- [29.2. I/O Software and Device Drivers](#i-o-software-and-device-drivers){.reference .internal .nav-link}
  - [29.2.1. Fundamental Goals](#fundamental-goals){.reference .internal .nav-link}
- [29.3. Putting it all together](#putting-it-all-together){.reference .internal .nav-link}
  :::
  :::
  :::

::: {#searchbox}
:::

::: {#input-and-output .section .tex2jax_ignore .mathjax_ignore}
[]{#cont-other-devices}

# [29. ] {.section-number}Input and Output[\#](#input-and-output "Link to this heading") {.headerlink}

Input/Output (I/O) devices are crucial to the operation of a computer. The data that a program processes --- as well as the program binary itself --- must be loaded into memory from some I/O device such as a disks, networks, or keyboard. Similarly, without a way to output the results of a computation to the monitors or to storage, those results would be lost.

One of the primary functions of the operating system is to manage these I/O devices. It should control access to them, as well as providing a consistent programming interface across a wide range of hardware devices with similar functionality but differing details.

![[Fig. 29.1 ]{.caption-number}[Supporting devices]{.caption-text}[\#](#devs-fig-rep "Link to this image"){.headerlink}](../_images/purpose-OS-source-12.drawio.png){style="width: 300pt;"}

We first describe the characteristics of device hardware, and then how the OS interacts with that hardware.

::: {#io-hardware .section}

## [29.1. ] {.section-number}IO Hardware[\#](#io-hardware "Link to this heading") {.headerlink}

We outline structure of a standard computer, device controllers, how the OS interacts with the controller using port and memory mapped I/O, how interrupts work, and conclude with a discussion of Direct Memory Access (DMA).

![[Fig. 29.2 ]{.caption-number}[An abstract model of a computer.]{.caption-text}[\#](#simplecomputer-fig2 "Link to this image"){.headerlink}](../_images/hardware.png){style="width: 50%;"}

::: {#structure-of-a-computer .section}

### [29.1.1. ] {.section-number}Structure of a computer[\#](#structure-of-a-computer "Link to this heading") {.headerlink}

At the start of the course, we [[presented]{.std .std-ref}](../intro/purpose.html#cont-gs-purpose-hw){.reference .internal} a simple model of hardware ([[Fig. 29.2]{.std .std-numref}](#simplecomputer-fig2){.reference .internal}) was discussed. The CPU is connected to high speed memory, and through a lower speed bus to a network controller and disk controller that are in turn connected to a network (ethernet in this case) and a disk.

[[Fig. 29.3]{.std .std-numref}](#fig-iobus-1){.reference .internal} shows the more complicated architecture of a relatively modern Intel-architecture. Different parts of the system are connected by buses, or communication channels, operating at various speeds. The Front-Side Bus carries all memory transactions which miss in L1 and L2 cache, and the North Bridge directs these transactions to memory (DDR2 bus) or I/O devices (PCIe bus) based on their address. The PCI Express (PCIe) is somewhat slower than the front-side bus, but can be extended farther; it connects all the I/O devices on the system. In some cases (like USB and SATA), a controller connected to the PCIe bus (although typically located on the motherboard itself) may interface to a yet slower external interface. Finally, the ISA bus, used to connect slow devices like keyboards, is a vestige of the original IBM PC; for some reason, they've never moved some crucial system functions off of it, so it's still needed.[[\[]{.fn-bracket}1[\]]{.fn-bracket}](#id2){#id1 .footnote-reference .brackets role="doc-noteref"}

![[Fig. 29.3 ]{.caption-number}[A standard Intel PC Architecture]{.caption-text}[\#](#fig-iobus-1 "Link to this image"){.headerlink}](../_images/iobus-fig1.png){style="width: 80%;"}

The term "bus" was taken from electrical engineering; in high-power electric systems a *bus bar* is a copper bar used to distribute power to multiple pieces of equipment. A simple bus like this one distributes address and data signals in much the same way.
:::

::: {#controllers .section}

### [29.1.2. ] {.section-number}Controllers[\#](#controllers "Link to this heading") {.headerlink}

I/O devices typically connected as PCI/ISA cards installed on the mother board have, in additional to their mechanical components, controllers that manage the device. The task of this controller is to convert from the operations on the bus to device specific operations. The processor interacts with these controllers by reading and writing controller registers.

![[Fig. 29.4 ]{.caption-number}[Registers of an Intel network interface card. It contains around 5600 32-bit registers broken down as shown. Note that complex OSes, like Linux, only initialize around 1000 of these registers.]{.caption-text}[\#](#fig-intelnic "Link to this image"){.headerlink}](../_images/modernnic-regs.png){style="width: 70%;"}

To understand how complex modern devices can be, consider [[Fig. 29.4]{.std .std-numref}](#fig-intelnic){.reference .internal} that shows the breakdown of registers of a modern Intel NIC. There are over 5600 32 bit registers, providing enormous complexity in how the OS can configure and interact with the device. As a result, these controllers often have a general purpose CPU, a fair amount of RAM to buffer data going to/from the device, and often some permanent flash storage. The software that used on these processors, typically referred to as firmware is complex enough that it must be regularly upgraded to deal with bugs. This turns out to be a massive attack surface in today's computers. For example the following [story](https://www.vice.com/en/article/ypwkwk/the-nsas-undetectable-hard-drive-hack-was-first-demonstrated-a-year-ago){.reference .external} describes one technique that has been used by the NSA to embed undetectable spyware on disks.
:::

::: {#accessing-the-controller .section}

### [29.1.3. ] {.section-number}Accessing the controller[\#](#accessing-the-controller "Link to this heading") {.headerlink}

The OS talks with the controller by reading and writing registers of the device and by reading and writing data that is buffered by the controller. Certain CPUs, including Intel architecture, contain support for a secondary I/O bus, with a smaller address width and accessed via special instructions. (e.g. "IN 0x100" to read a byte from I/O location 0x100, which has nothing to do with reading a byte from memory location 0x100). This is typically called port mapped I/O.

All architectures support *Memory-mapped I/O*, where devices can be mapped in the physical memory space and accessed via standard load and store instructions.

Depending on the system architecture, the device may be responsible for decoding the full address and determining when it has been selected, or a select signal may indicate when a particular slot on the bus is being accessed. Almost all computers today use a version of the PCI bus, which uses memory-mapped access, and at boot time, assigns each I/O device a physical address range to which it should respond.
:::

::: {#polled-vs-interrupt-driven-i-o .section}

### [29.1.4. ] {.section-number}Polled vs. Interrupt-driven I/O[\#](#polled-vs-interrupt-driven-i-o "Link to this heading") {.headerlink}

![[Fig. 29.5 ]{.caption-number}[Polled I/O]{.caption-text}[\#](#fig-iobus-polled "Link to this image"){.headerlink}](../_images/iobus-polled.png){style="width: 70%;"}

The simplest way to control an I/O device is for the CPU to issue commands and then wait, polling a device status register until the operation is complete. In [[Fig. 29.5]{.std .std-numref}](#fig-iobus-polled){.reference .internal} (a) an application requests I/O via e.g. a `read`{.docutils .literal .notranslate} system call; the OS (step 1) then writes to the device command register to start an operation, after which (step 2) it begins to poll the status register to detect completion. Meanwhile (step 3) the device carries out the operation, after which (step 4) polling by the OS detects that it is complete, and finally (step 5) the original request (e.g. `read`{.docutils .literal .notranslate}) can return to the application.

![[Fig. 29.6 ]{.caption-number}[Interrupt
driven I/O]{.caption-text}[\#](#fig-iobus-inter "Link to this image"){.headerlink}](../_images/iobus-irq.png){style="width: 70%;"}

The alternate is interrupt-driven I/O, as shown in [[Fig. 29.6]{.std .std-numref}](#fig-iobus-inter){.reference .internal} (b). After (step 1) issuing a request to the hardware, the OS (step 2) puts the calling process to sleep and switches to another process while (step 3) the hardware handles the request. When the I/O is complete, the device (step 4) raises an interrupt. The interrupt handler then finishes the request. In the illustrated example, the interrupt handler (step 5) reads data that has become available, and then (step 6) wakes the waiting process, which returns from the I/O call (step 7) and continues.
:::

::: {#interrupts .section}

### [29.1.5. ] {.section-number}Interrupts[\#](#interrupts "Link to this heading") {.headerlink}

We have already mentioned Interrupts many times, but nows a good time to flesh them out in a bit more detail. To handle asynchronous I/O events, CPUs provide an *interrupt* mechanism. In response to a signal from an I/O device the CPU executes an *interrupt handler* function, returning to its current execution when the handler is done. The CPU essentially performs a forced function call, saving the address of the next instruction on the stack and jumping to the interrupt handler; the difference is that instead of doing this in response to a CALL instruction, it does it at some arbitrary time (but *between* two instructions) when the interrupt signal is asserted.

Most CPUs have several interrupt inputs; these correspond to an *interrupt vector table* in memory, either at a fixed location or identified by a special register, giving the addresses of the corresponding interrupt handlers. As an example, below we see the corresponding table for an 8088 CPU as found in the original IBM PC, which provides handler addresses for external hardware interrupts as well as *exceptions* which halt normal program execution, such as dividing by zero or attempting to execute an illegal instruction.

::: {.highlight-default .notranslate}
::: highlight
Index          Description          DOS name
------- ------------------------- ------------
0            divide by zero
1              single step
2             non-maskable
3              debug break
4        debug break on overflow
5               -unused-
6            invalid instr.
7               -unused-
8             system timer            IRQ0
9            keyboard input           IRQ1
10           line printer 2        IRQ2, LPT2
11            serial port 2        IRQ3, COM2
12            serial port 1        IRQ4, COM1
13              hard disk             IRQ5
14             floppy disk            IRQ6
15           line printer 1        IRQ7, LPT1
16-         software-defined
255            interrupts

```
  : 8086/8088 interrupts as defined by the IBM PC hardware.
```

:::
:::

The simplest interrupt-generating device is a *timer*, which does nothing except generate an interrupt at a periodic interval. As shown below, we see why it is called a timer---one of its most common uses is to keep track of time.

::: {.highlight-default .notranslate}
::: highlight
extern int time_in_ticks;
timer_interrupt_handler() {
time_in_ticks++;
}
:::
:::

Another simple use for interrupts is for notification of keyboard input. Besides being useful for a "cancel" command like control-C, this is also very useful for *type-ahead*. On slower computers (e.g. the original IBM PC executed less than half a million instructions per second) a fast typist can hit multiple keys while a program is busy. A simple keyboard interface only holds one keystroke, causing additional ones to be lost. By using the keyboard interrupt, the operating system can read these keystrokes and save them, making them available to the program the next time it checks for input.
:::

::: {#direct-memory-access-dma .section}

### [29.1.6. ] {.section-number}Direct Memory Access (DMA)[\#](#direct-memory-access-dma "Link to this heading") {.headerlink}

The CPU could copying data between I/O devices and memory using normal memory load and store instructions. Such an approach works well on computers such as the Apple II or the original IBM PC which run at a few MHz, where the address and data buses can be extended at full speed to external I/O cards. A modern CPU runs at over 3 GHz, however; during a single clock cycle light can only travel about 4 inches, and electrical signals even less. [[Fig. 29.7]{.std .std-numref}](#fig-iobus-latency){.reference .internal} shows example latencies for a modern CPU (in this case an Intel i5, with L3 cache omitted) to read a data value from L1 and L2 cache, a random location in memory (sequential access is faster), and a register on a device on the PCIe bus. (e.g. the disk or ethernet controller) In such a system, reading data from a device in 4-byte words would result in a throughput of 5 words every microsecond, or 20MB/s --- far slower than a modern network adapter or disk controller.

![[Fig. 29.7 ]{.caption-number}[Latency between CPU and various levels of memory/IO hierarchy]{.caption-text}[\#](#fig-iobus-latency "Link to this image"){.headerlink}](../_images/iobus-latency.png){style="width: 70%;"}

![[Fig. 29.8 ]{.caption-number}[DMA access for high-speed data transfer]{.caption-text}[\#](#fig-iobus-dma "Link to this image"){.headerlink}](../_images/iobus-dma.png){style="width: 70%;"}

As CPU speeds have become faster and faster, RAM and I/O devices have only slowly increased in speed. The strategies for coping with the high relative latency of RAM and I/O are very different, however---caching works quite well with RAM, which stores data generated by the CPU, while I/O (at least the input side) involves reading new data; here latency is overcome by pipelining, instead.

Almost all computers today use the PCIe bus. Transactions on the PCIe bus require a negotiation stage, when the CPU (or a device) requests access to bus resources, and then is able to perform a transaction after being granted access. In addition to basic read and write requests, the bus also supports Direct Memory Access (DMA), where I/O devices are able to read or write memory directly without CPU intervention. [[Fig. 29.8]{.std .std-numref}](#fig-iobus-dma){.reference .internal} shows a single programmed-I/O read (top) compared to a DMA burst transfer (bottom). While the read request requires a round trip to read each and every 4-byte word, once the DMA transfer is started it is able to transfer data at a rate limited by the maximum bus speed. (For an 8 or 16-lane PCIe card this limit is many GB/s)

A device typically requires multiple parameters to perform an operation and transfer the data to or from memory. In the case of a disk controller, for instance, these parameters would include the type of access (read or write), the disk locations to be accessed, and the memory address where data will be stored or retrieved from. Rather than writing each of these parameters individually to device registers, the parameters are typically combined in memory in what is called a *DMA descriptor*, such as the one shown in [[Fig. 29.9]{.std .std-numref}](#fig-iobus-desc){.reference .internal}. A single write is then used to tell the device the address of this descriptor, and the device can read the entire descriptor in a single DMA read burst. In addition to being more efficient than multiple programmed I/O writes, this approach also allows multiple requests to be queued for a device. (In the case of queued disk commands, the device may even process multiple such requests simultaneously.) When an I/O completes, the device notifies the CPU via an interrupt, and writes status information (such as success/failure) into a field in the DMA descriptor. (or sometimes in a device register, for simple devices which do not allow multiple outstanding requests.) The interrupt handler can then determine which operations have completed, free their DMA descriptors, and notify any waiting processes.

**Cache-coherent I/O:** The PCIe bus is *cache-consistent*; many earlier I/O buses weren't. Consider what would happen if the CPU wrote a value to location 1000 (say that's the command/status field of a DMA descriptor), then the device wrote a new value to that same location, and finally the CPU tried to read it back?

![[Fig. 29.9 ]{.caption-number}[List of typical DMA descriptors]{.caption-text}[\#](#fig-iobus-desc "Link to this image"){.headerlink}](../_images/iobus-desc.png){style="width: 70%;"}
:::
:::

::: {#i-o-software-and-device-drivers .section}

## [29.2. ] {.section-number}I/O Software and Device Drivers[\#](#i-o-software-and-device-drivers "Link to this heading") {.headerlink}

::: {#fundamental-goals .section}

### [29.2.1. ] {.section-number}Fundamental Goals[\#](#fundamental-goals "Link to this heading") {.headerlink}

The operating system software that interacts with devices must:

- **Provide Device Independence:** Programs should be able to access any similar device without worrying about the specific device available. For example, you should be able to read data from a floppy, hard drive, or CD-ROM without caring which device is available. As another example, your *vim* editor should be able to work if you are connecting a dumb terminal to your computer, or if you are using an emulated terminal provided by our course staff.
- **Handle Errors:** Many errors are transient, and we want to handle them as close to the hardware as possible. For example, if a network is unavailable for a brief period of time, we don't want to close all the connections. If we get an error reading a disk block, the OS might try re-reading assuming that there was a transient failure, or correct the error using some form of error correcting code.
- **Support synchronous interfaces:** In reality, all devices interact with the OS asynchronously, where some character appears from a terminal when a user hits a key, or a network packet arrives when clients make new requests to a server. On the other hand, generally the programming interfaces users have are synchronous, for example, using a `read`{.docutils .literal .notranslate} to a network socket or file system. The OS keeps translates between the blocking calls by applications and the innate events that come in from devices.
- **Buffering:** Related to asynchronous interactions, the operating system normally manages buffers to enable data to be transferred to and from the devices to match the performance needs of the device. We have already seen how memory management creates a massive buffer cache to buffer millions of blocks in memory. On the other hand, if a program is dumping huge files to a slow character device, the OS needs to buffer the data, and feed it to the device at the rate that the device can handle.

![[Fig. 29.10 ]{.caption-number}[OS layers]{.caption-text}[\#](#fig-dev-layers "Link to this image"){.headerlink}](../_images/dev-layers.png){style="width: 70%;"}

To perform this functionality, much like when we discussed the VFS layer in file systems, as shown in [[Fig. 29.10]{.std .std-numref}](#fig-dev-layers){.reference .internal} there is generic I/O code that provides services like buffering, generalized error reporting, and enables a set of standardized device interfaces. The three kind of standard device types are:

1. Block devices: e.g. SSDs, Hard drives, CDROMs
2. Character devices: ttys, pipes, ...
3. Network devices: ethernet, token ring,...

There are many many devices drivers of each type. In fact, over 60% of Linux source code today with device drivers involving 10s of millions of LOC. Much of this code is provided by device manufacturers, and is the most buggy part of the OS.

Drivers responsibilities include:

- Device initialization
- Accept read-write request from the OS: i.e., take commands from higher levels in the OS and translate them into hardware requests
- Start the device if necessary (e.g., start spinning the CD-ROM)
- Check if device is available: if not, wait
- Wait for results; typically blocking client request until interrupt occurs
- Check for possible errors
- Return results, and finally
- Power management -- put the device to sleep when it's not being used
  :::
  :::

::: {#putting-it-all-together .section}

## [29.3. ] {.section-number}Putting it all together[\#](#putting-it-all-together "Link to this heading") {.headerlink}

[[Fig. 29.11]{.std .std-numref}](#fig-iobus-driver){.reference .internal} illustrates the I/O process for a typical device from user-space application request through the driver, hardware I/O operation, interrupt, and finally back to user space.

![[Fig. 29.11 ]{.caption-number}[Putting it together]{.caption-text}[\#](#fig-iobus-driver "Link to this image"){.headerlink}](../_images/iobus-driver.png){style="width: 70%;"}

In more detail:

- The user process executes a `read`{.docutils .literal .notranslate} system call, which in turn invokes the driver `read`{.docutils .literal .notranslate} operation, found via the `read`{.docutils .literal .notranslate} method of the file operations structure.
- The driver fills in a DMA descriptor (in motherboard RAM), writes the physical address of the descriptor to a device register (generating a Memory Write operation across the PCIe bus), and then goes to sleep.
- The device issues a PCIe Memory Read Multiple command to read the DMA descriptor from RAM.
- The device does some sort of I/O. (e.g. read from a disk, or receive a network packet)
- A Memory Write and Invalidate operation is used to write the received data back across the PCIe bus to the motherboard RAM, and to tell the CPU to invalidate any cached copies of those addresses.
- A hardware interrupt from the device causes the device driver interrupt handler to run.
- The interrupt handler wakes up the original process, which is currently in kernel space in the device driver read method, in a call to something like `interruptible_sleep_on`{.docutils .literal .notranslate}. After waking up, the read method copies the data to the user buffer and returns.

---

[[\[]{.fn-bracket}[1](#id1){role="doc-backlink"}[\]]{.fn-bracket}]{.label}

The primary difference between this figure and contemporary systems is that (a) the memory bus is DDR3 or DDR4, and (b) the north bridge is located on the CPU chip, with no external front-side bus.
:::
:::

::: prev-next-area
[](../sync/review.html "previous page"){.left-prev}

::: prev-next-info
previous

[28. ]{.section-number}Review
:::

[](disk2.html "next page"){.right-next}

::: prev-next-info
next

[30. ]{.section-number}More on Disks
:::
:::
:::

::: {.bd-sidebar-secondary .bd-toc}
::: {.sidebar-secondary-items .sidebar-secondary__inner}
::: sidebar-secondary-item
::: {.page-toc .tocsection .onthispage}
Contents
:::

- [29.1. IO Hardware](#io-hardware){.reference .internal .nav-link}
  - [29.1.1. Structure of a computer](#structure-of-a-computer){.reference .internal .nav-link}
  - [29.1.2. Controllers](#controllers){.reference .internal .nav-link}
  - [29.1.3. Accessing the controller](#accessing-the-controller){.reference .internal .nav-link}
  - [29.1.4. Polled vs. Interrupt-driven I/O](#polled-vs-interrupt-driven-i-o){.reference .internal .nav-link}
  - [29.1.5. Interrupts](#interrupts){.reference .internal .nav-link}
  - [29.1.6. Direct Memory Access (DMA)](#direct-memory-access-dma){.reference .internal .nav-link}
- [29.2. I/O Software and Device Drivers](#i-o-software-and-device-drivers){.reference .internal .nav-link}
  - [29.2.1. Fundamental Goals](#fundamental-goals){.reference .internal .nav-link}
- [29.3. Putting it all together](#putting-it-all-together){.reference .internal .nav-link}
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
