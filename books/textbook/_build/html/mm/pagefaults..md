---
docsearch:language: en
lang: en
title: 14.6. Memory Management Page Faults --- Introduction to Operating Systems
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

-   [12. Introduction](intro.html){.reference .internal}
-   [13. Memory management before paged virtual memory](phys-and-seg.html){.reference .internal}
-   [14. Paged Virtual memory](pagvm.html){.reference .internal}
    []{.toctree-toggle role="presentation"}
    -   [14.1. Abstracting a useful interface for memory management.](vmabs.html){.reference .internal}
    -   [14.2. Paging](virt-paging.html){.reference .internal}
    -   [14.3. Page Tables](page-tables.html){.reference .internal}
    -   [14.4. Memory reclaiming algorithms.](reclamation.html){.reference .internal}
    -   [14.5. Page Sizes](page-size.html){.reference .internal}
    -   [14.6. Memory Management Page Faults](#){.current .reference .internal}
-   [15. Buffer Cache](buffer-cache.html){.reference .internal}
-   [16. Memory management in the real world](realworld.html){.reference .internal}
-   [17. Conclusion](concl.html){.reference .internal}
-   [18. Review](review.html){.reference .internal}

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

-   [[ ![JupyterHub logo](../_static/images/logo_jupyterhub.svg) ]{.btn__icon-container} [JupyterHub]{.btn__text-container}](https://jupyterhub-opf-jupyterhub.apps.smaug.na.operate-first.cloud/hub/user-redirect/git-pull?repo=https%3A//github.com/OpenOSOrg/openos&urlpath=lab/tree/openos/content/mm/pagefaults.ipynb&branch=main "Launch on JupyterHub"){.btn .btn-sm .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
:::

::: {.dropdown .dropdown-source-buttons}

-   [[ ]{.btn__icon-container} [Repository]{.btn__text-container}](https://github.com/OpenOSOrg/openos "Source repository"){.btn .btn-sm .btn-source-repository-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
-   [[ ]{.btn__icon-container} [Suggest edit]{.btn__text-container}](https://github.com/OpenOSOrg/openos/edit/main/content/mm/pagefaults.ipynb "Suggest edit"){.btn .btn-sm .btn-source-edit-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
-   [[ ]{.btn__icon-container} [Open issue]{.btn__text-container}](https://github.com/OpenOSOrg/openos/issues/new?title=Issue%20on%20page%20%2Fmm/pagefaults.html&body=Your%20issue%20content%20here. "Open an issue"){.btn .btn-sm .btn-source-issues-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
:::

::: {.dropdown .dropdown-download-buttons}

-   [[ ]{.btn__icon-container} [.ipynb]{.btn__text-container}](../_sources/mm/pagefaults.ipynb "Download source file"){.btn .btn-sm .btn-download-source-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
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
# Memory Management Page Faults

::: {#print-main-content}
::: {#jb-print-toc}
<div>

## Contents

</div>

-   [14.6.1. Page Faulting](#page-faulting){.reference .internal .nav-link}
    -   [14.6.1.1. Page Faults](#page-faults){.reference .internal .nav-link}
    -   [14.6.1.2. Process Address Space, Revisited](#process-address-space-revisited){.reference .internal .nav-link}
        -   [14.6.1.2.1. Executable file and process address space](#executable-file-and-process-address-space){.reference .internal .nav-link}
    -   [14.6.1.3. Page Faults in the Kernel](#page-faults-in-the-kernel){.reference .internal .nav-link}
    -   [14.6.1.4. copy-on-write page faults](#copy-on-write-page-faults){.reference .internal .nav-link}
        -   [14.6.1.4.1. Review questions](#review-questions){.reference .internal .nav-link}
:::
:::
:::

::: {#searchbox}
:::

This chapter describes page faults, what they are, various types, how they work and how they allow virtual address spaces that are much larger than physical memory.

::: {#memory-management-page-faults .section .tex2jax_ignore .mathjax_ignore}
# [14.6. ]{.section-number}Memory Management Page Faults[\#](#memory-management-page-faults "Link to this heading"){.headerlink}

There are 3 basic types of page faults:

-   File backed page faults

-   Anonymous page faults

-   Copy On Write page faults

::: {#page-faulting .section}
## [14.6.1. ]{.section-number}Page Faulting[\#](#page-faulting "Link to this heading"){.headerlink}

In the previous section you saw how the MMU in a Pentium-like CPU determines whether a memory access will succeed:

::: {.highlight-default .notranslate}
::: highlight
    if the top-level entry has P=1
       and is(read) or W=1
       and is(supervisor) or U=1:

       if the 2nd-level entry has P=1
          and is(read) or W=1
          and is(supervisor) or U=1:

            use translated address.
:::
:::

If translation fails at any one of the six possible points above (P, W, or U at each level) then a page fault is generated.

::: {#page-faults .section}
### [14.6.1.1. ]{.section-number}Page Faults[\#](#page-faults "Link to this heading"){.headerlink}

A page fault is a special form of exception that has the following two characteristics: first, it is generated when an address translation fails, and second, it occurs in the middle of an instruction, not after it is done, so that the instruction can be continued after fixing the problem which caused the page fault. Typical information that the MMU passes to the page fault handler is:

1.  The instruction address when the page fault occurred. (this is the return address pushed on the stack as part of the exception handling process)

2.  The address that caused the page fault

3.  Whether the access attempt was a read or a write

4.  Whether the access was attempted in user or supervisor mode

After the page fault handler returns, the instruction that caused the fault resumes, and it retries the memory access that caused the fault in the first place.

::: {.admonition .note}
Note

15 Many of the examples in this section are illustrated using Linux, as the source code is readily available, but same principles (although not details) hold true for other modern OSes such as Windows, Mac OS X, or Solaris.

In addition, keep in mind that the virtual memory map for a process is a software concept, and will almost certainly differ between two unrelated operating systems. In contrast, the page table structure is defined by the CPU itself, and must be used in that form by any operating system running on that CPU.
:::

A single instruction can cause multiple, different page faults, of which there are two different types:

-   **Instruction fetch:** A fault can occur when the CPU tries to fetch the instruction at a particular address. If the instruction "straddles" a page boundary (i.e., a 6-byte instruction that starts 2 bytes before the end of a page) then you could (in the worst case) get two page faults while trying to fetch an instruction.

-   **Memory access:** Once the instruction has been fetched and decoded, it may require one or more memory accesses that result in page faults. These memory accesses include those to the stack (e.g., for CALL and RET instructions) in addition to load and store instructions. As before, accessing memory that straddles a page boundary will result in additional faults.
:::

::: {#process-address-space-revisited .section}
### [14.6.1.2. ]{.section-number}Process Address Space, Revisited[\#](#process-address-space-revisited "Link to this heading"){.headerlink}

How does the OS know how to handle a page fault? By examining its internal memory map for a process. We've talked briefly about process memory maps earlier, but now we will look in more detail at a specific one, from a fairly recent (kernel 2.6 or 3.0) 32-bit Linux system. A more thorough description of the Linux memory layout can be found [here](http://duartes.org/gustavo/blog/post/anatomy-of-a-program-in-memory){.reference .external}.

![[Fig. 14.22 ]{.caption-number}[Top 1GB is the Kernel address space and bottom 3GB is the user address space.]{.caption-text}[\#](#fig-vm-fig100 "Link to this image"){.headerlink}](../_images/virt-mem-pic100.png){style="width: 25%;"}

In earlier chapters we saw how simple operating systems may use separate portions of the address space for programs and for the operating system. The same approach is often used in dividing up the virtual address space in more complex operating systems, as seen in the 32-bit Linux memory map in [[Fig. 14.22]{.std .std-numref}](#fig-vm-fig100){.reference .internal}. In recent Linux versions running on 32-bit Intel-compatible CPUs, the kernel "owns" the top 1GB, from virtual address 0xC0000000 to 0xFFFFFFFF, and all kernel code, data structures, and temporary mappings go in this range.

The kernel must be part of every address space, so that when exceptions like system calls and page faults change execution from user mode to supervisor mode, all the kernel code and data needed to execute the system call or page fault handler are already available in the current virtual memory map\[\^8\] This is the primary use for the U bit in the page table---by setting the U bit to zero in any mappings for operating system code and data, user processes are prevented from modifying the OS or viewing protected data.

Here is the memory map of a very simple process\[\^9\], as reported in `/proc/<pid>/maps`{.docutils .literal .notranslate}:

::: {.highlight-default .notranslate}
::: highlight
    08048000-08049000 r-xp 00000000 08:03 4072226    /tmp/a.out
    08049000-0804a000 rw-p 00000000 08:03 4072226    /tmp/a.out
    0804a000-0804b000 rw-p 00000000 00:00 0          [anon]
    bffd5000-bfff6000 rw-p 00000000 00:00 0          [stack]
:::
:::

The memory space has four segments:

::: {.highlight-default .notranslate}
::: highlight
    **08048000** (one page) - read-only, executable, mapped from file *a.out*
    **08049000** (one page) - read/write, mapped from file *a.out*
    **0804a000** (one page) - read/write, "anonymous"
    **bffd5000-bfff6000** (33 4KB pages) - read/write, "stack"
:::
:::

Where does this map come from? When the OS creates the new address space in the `exec()`{.docutils .literal .notranslate} system call, it knows it needs to create a stack, but the rest of the information comes from the executable file itself:

::: {.highlight-default .notranslate}
::: highlight
    $ objdump -h a.out
    a.out:     file format elf32-i386

    Idx Name          Size      VMA       LMA       File off  Algn

      0 .text         00000072  08048094  08048094  00000094  2**2
                      CONTENTS, ALLOC, LOAD, READONLY, CODE
      1 .rodata       000006bd  08048108  08048108  00000108  2**2
                      CONTENTS, ALLOC, LOAD, READONLY, DATA
      2 .data         00000030  080497c8  080497c8  000007c8  2**2
                      CONTENTS, ALLOC, LOAD, DATA
      3 .bss          00001000  08049800  08049800  000007f8  2**5
                      ALLOC
    $
:::
:::

Executable files on Linux are stored in the ELF format (Executable and Linking Format), and include a header that describes the file to the OS; the information above came from this header. Looking at the file, the following sections can be seen:

------------------------------------------------------------------------

::: {.highlight-none .notranslate}
::: highlight
              `0 ... x93` various header information   
    `00000094 - 00000107` ".text"                      program code
    `00000108 - 000007c7` ".rodata"                    read/only data (mostly strings)
    `000007c8 - 000007e7` ".data"'                     initialized writable data
                (no data) ".bss"'                      zero-initialized data
:::
:::

------------------------------------------------------------------------

The BSS section corresponds to global variables initialized to zero. Since the BSS section is initialized to all zeros, there is no need to store its initial contents in the executable file. Instead, the exec() system call allocate anonymous memory for any BSS sections thereby reducing the actual size of executable files on storage.

::: {#executable-file-and-process-address-space .section}
#### [14.6.1.2.1. ]{.section-number}Executable file and process address space[\#](#executable-file-and-process-address-space "Link to this heading"){.headerlink}

Here you can see the relationship between the structure of the executable file and the process address space created by the kernel when it runs this executable. One page (08048xxx) is used for read-only code and data, while two pages (08049xxx and 0804Axxx) are used for writable data.

![[Fig. 14.23 ]{.caption-number}[Relationship of executable file header to memory map structure]{.caption-text}[\#](#vm-pic101 "Link to this image"){.headerlink}](../_images/virt-mem-pic101.png){style="width: 40%;"}
:::
:::

::: {#page-faults-in-the-kernel .section}
### [14.6.1.3. ]{.section-number}Page Faults in the Kernel[\#](#page-faults-in-the-kernel "Link to this heading"){.headerlink}

Although common in the past, modern Windows and Linux systems rarely seem to crash due to driver problems. (Although my Mac panics every month or two.) If you ever develop kernel drivers, however, you will become very familiar with them during the debug phase of development.

What happens if there is a page fault while the CPU is running kernel code in supervisor mode? It depends.

If the error is due to a bug in kernel-mode code, then in most operating systems the kernel is unable to handle it. In Linux the system will display an "Oops" message, as shown below, while in Windows the result is typically a "kernel panic", which used to be called a Blue Screen of Death. Most of the time in Linux the process executing when this happens will be terminated, but the rest of the system remains running with possibly reduced functionality.

::: {.highlight-default .notranslate}
::: highlight
    [  397.864759] BUG: unable to handle kernel NULL pointer dereference at 
                                                                    0000000000000004
    [  397.865725] IP: [<ffffffffc01d1027>] track2lba+0x27/0x3f [dm_vguard]
    [  397.866619] PGD 0 
    [  397.866929] Oops: 0000 [#1] SMP 
    [  397.867395] Modules linked in: [...]
    [  397.872730] CPU: 0 PID: 1335 Comm: dmsetup Tainted: G           OE   4.6.0 #3
    [  397.873419] Hardware name: QEMU Standard PC (i440FX + PIIX, 1996), BIOS ...
    [  397.874487] task: ffff88003cd10e40 ti: ffff880037080000 task.ti: ffff88003708
    [  397.875375] RIP: 0010:[<ffffffffc01d1027>]  [<ffffffffc01d1027>] track2lba+0x27
    [  397.876509] RSP: 0018:ffff880037083bd0  EFLAGS: 00010282
    [  397.877193] RAX: 0000000000000001 RBX: 0000000000003520 RCX: 0000000000000000
    [  397.878085] RDX: 0000000000000000 RSI: 0000000000003520 RDI: ffff880036bd70c0
    [  397.879016] RBP: ffff880037083bd0 R08: 00000000000001b0 R09: 0000000000000000
    [  397.879912] R10: 000000000000000a R11: f000000000000000 R12: ffff880036bd70c0
    [  397.880763] R13: 00000000002e46e0 R14: ffffc900001f7040 R15: 0000000000000000
    [  397.881618] FS:  00007f5767938700(0000) GS:ffff88003fc00000(0000) 
    [  397.915186] CS:  0010 DS: 0000 ES: 0000 CR0: 0000000080050033
    [  397.932122] CR2: 0000000000000004 CR3: 000000003d3ea000 CR4: 00000000000406f0
    [  397.949459] Stack:
                          ... stack contents and backtrace omitted ...
:::
:::

But what about addresses passed by the user in a system call? For example, what if the memory address passed to a `read`{.docutils .literal .notranslate} system call has been paged out, or not instantiated yet? It turns out that the same page faulting logic can be used in the kernel, as well---the first access to an unmapped page will result in a fault, the process will be interrupted (in the kernel this time, rather than in user-space code), and then execution will resume after the page fault is handled.

But what if the user passes a bad address? We can't just kill the process partway through the system call, because that would risk leaving internal operating system data structures in an inconsistent state. (Not only that, but the POSIX standard requires that system calls return the EFAULT error in response to bad addresses, not exit.) Instead, all code in the Linux kernel which accesses user-provided memory addresses is supposed to use a pair of functions, `copy_from_user`{.docutils .literal .notranslate} and `copy_to_user`{.docutils .literal .notranslate}, which check that the user-provided memory region is valid for user-mode access\[\^11\].

In very early versions of Linux the kernel ran in a separate address space where virtual addresses mapped directly to physical addresses, and so these functions actually interpreted the page tables to translate virtual addresses to physical (i.e. kernel virtual) addresses, which was slow but made it easy to return an error if an address was bad. Newer Linux versions map the kernel and its data structures into a predefined region of each each process virtual address space, making these functions much faster but more complicated. The speedup is because there is no longer any need to translate page tables in software; instead the two `copy_*_user`{.docutils .literal .notranslate} functions just perform a few checks and then a `memcpy`{.docutils .literal .notranslate}. More complicated because if it fails we don't find out about it in either of these functions, but rather in the page fault handler itself. To make this work, if the page fault (a) occurs in kernel mode, and (b) the handler can't find a translation for the address, it checks to see if the fault occurred while executing the `copy_from_user`{.docutils .literal .notranslate} or `copy_to_user`{.docutils .literal .notranslate} functions, and if so it performs some horrible stack manipulation to cause that function to return an error code\[\^12\].

But what if a page fault occurs in the kernel outside of these two functions? That should never happen, because kernel structures are allocated from memory that's already mapped in the kernel address space. In other words it's a bug, just like the bugs that cause segmentation faults in your C programs. And just like those bugs it causes a crash, resulting in an error message such as the one shown above. If the kernel was running in a process context (e.g. executing system call code) then the currently-running process will be killed. This behavior is really not safe because its likely some corruption of kernel data structures and not likely cause be the process itself. However, it does prevent the whole system from crashing.\
If this occurs during an interrupt the system will crash. The equivalent in Windows is called a Blue Screen of Death (although they changed the color several versions back); since almost all Windows kernel code executes in interrupt context, these errors always result in a system crash.
:::

::: {#copy-on-write-page-faults .section}
### [14.6.1.4. ]{.section-number}copy-on-write page faults[\#](#copy-on-write-page-faults "Link to this heading"){.headerlink}

In all the cases you've seen so far, page sharing has been used to share read-only pages---these are intrinsically safe to share, because processes are unable to modify the pages and thereby affect other processes. But, can writable pages be shared safely? The answer is yes, but it has to be done carefully.

First, some background on why this is important. The Unix operating system uses two system calls to create new processes and execute programs: `fork()`{.docutils .literal .notranslate} and `exec()`{.docutils .literal .notranslate}. `fork()`{.docutils .literal .notranslate} makes a copy of the current process\[\^16\], while `exec(file)`{.docutils .literal .notranslate} replaces the address space of the current process with the program defined by `file`{.docutils .literal .notranslate} and begins executing that program at its designated starting point.

UNIX uses this method because of an arbitrary choice someone made 40 years ago; there are many other ways to do it, each of them with their own problems. However this is how UNIX works, and we're stuck with it, so it's important to be able to do it quickly.

In early versions of Unix, `fork()`{.docutils .literal .notranslate} was implemented by literally copying all the writable sections (e.g., stack, data) of the parent process address space into the child process address space. After doing all this work, most (but not all) of the time, the first thing the child process would do is to call exec(), throwing away the entire contents of the address space that were just copied. It's bad enough when the shell does this, but even worse when a large program (e.g. Chrome) tries to execute a small program (e.g. /bin/ls) in a child process.

We've already seen how to share read-only data, but can we do anything about writable data? In particular, data which is writable, but isn't actually going to be written?

A quick inspection of several Firefox and Safari instances (using pmap on Linux and vmmap on OS X) indicates that a browser with two or three open tabs can easily have over 300MB of writable address space\[\^17\]. When fork is executed these writable pages can't just be given writable mappings in the child process, or changes made in one process would be visible in the other. In certain cases (i.e., the stack) this mutual over-writing of memory would almost certainly be disastrous.

However in practice, most of these writable pages *won't* be written to again. In fact, if the child process only executes a few lines of code and then calls [[exec]{.xref .myst}](#exec){.reference .internal}{.uri}, it may only modify a handful of pages before its virtual address space is destroyed and replaced with a new one.

Copy-on-write is in fact a widely-used strategy in computer systems. It is effectively a "lazy" copy, doing only the minimal amount of work needed and reducing both the cost of copying and the total space consumed. Similar copy-on-write mechanisms can be seen in file systems, storage devices, and some programming language runtime systems.

![[Fig. 14.24 ]{.caption-number}[Copy On Write after fork()]{.caption-text}[\#](#vm-cow "Link to this image"){.headerlink}](../_images/COW.png){style="width: 100%;"}

Linux uses a technique called *copy-on-write* to eliminate the need to copy most of this memory. When a child process is created in the [[fork]{.xref .myst}](#fork){.reference .internal}{.uri} system call, its address space shares not only the read-only pages from the parent process, but the writable pages as well. To prevent the two processes from interfering with each other, these pages are mapped read-only, resulting in a page fault whenever they are accessed by either process, but flagged as copy-on-write in the kernel memory map structures. This results in a page fault when either process tries to write to one of these pages; the page fault handler then "breaks" the sharing for that page, by allocating a new page, copying the old one, and mapping a separate page read-write in each of the processes.

::: {#review-questions .section}
#### [14.6.1.4.1. ]{.section-number}Review questions[\#](#review-questions "Link to this heading"){.headerlink}
:::
:::
:::
:::

::: prev-next-area
[](page-size.html "previous page"){.left-prev}

::: prev-next-info
previous

[14.5. ]{.section-number}Page Sizes
:::

[](buffer-cache.html "next page"){.right-next}

::: prev-next-info
next

[15. ]{.section-number}Buffer Cache
:::
:::
:::

::: {.bd-sidebar-secondary .bd-toc}
::: {.sidebar-secondary-items .sidebar-secondary__inner}
::: sidebar-secondary-item
::: {.page-toc .tocsection .onthispage}
Contents
:::

-   [14.6.1. Page Faulting](#page-faulting){.reference .internal .nav-link}
    -   [14.6.1.1. Page Faults](#page-faults){.reference .internal .nav-link}
    -   [14.6.1.2. Process Address Space, Revisited](#process-address-space-revisited){.reference .internal .nav-link}
        -   [14.6.1.2.1. Executable file and process address space](#executable-file-and-process-address-space){.reference .internal .nav-link}
    -   [14.6.1.3. Page Faults in the Kernel](#page-faults-in-the-kernel){.reference .internal .nav-link}
    -   [14.6.1.4. copy-on-write page faults](#copy-on-write-page-faults){.reference .internal .nav-link}
        -   [14.6.1.4.1. Review questions](#review-questions){.reference .internal .nav-link}
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
