---
docsearch:language: en
lang: en
title: 25.1. Cooperating Processes and Inter-process Communication --- Introduction to Operating Systems
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

-   [24. Introduction](sync.html){.reference .internal}
-   [25. Basic Synchronization](basic.html){.reference .internal}
    []{.toctree-toggle role="presentation"}
    -   [25.1. Cooperating Processes and Inter-process Communication](#){.current .reference .internal}
    -   [25.2. The Critical Section Problem](criticalsection.html){.reference .internal}
    -   [25.3. Implementing Locks](locks.html){.reference .internal}
    -   [25.4. Ordering Thread Events](ordering.html){.reference .internal}
-   [26. Common Concurrency Bugs](concurrency_bugs.html){.reference .internal}
-   [27. Advanced Synchronization](advanced.html){.reference .internal}
    []{.toctree-toggle role="presentation"}
    -   [27.1. Read-Dominated Workloads](readmostly.html){.reference .internal}
    -   [27.2. Challenges of Modern Hardware](hardware_challenges.html){.reference .internal}
    -   [27.3. Locking in the Linux Kernel](linux_locking.html){.reference .internal}
-   [28. Review](review.html){.reference .internal}

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

-   [[ ![JupyterHub logo](../_static/images/logo_jupyterhub.svg) ]{.btn__icon-container} [JupyterHub]{.btn__text-container}](https://jupyterhub-opf-jupyterhub.apps.smaug.na.operate-first.cloud/hub/user-redirect/git-pull?repo=https%3A//github.com/OpenOSOrg/openos&urlpath=lab/tree/openos/content/sync/sharing.ipynb&branch=main "Launch on JupyterHub"){.btn .btn-sm .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
:::

::: {.dropdown .dropdown-source-buttons}

-   [[ ]{.btn__icon-container} [Repository]{.btn__text-container}](https://github.com/OpenOSOrg/openos "Source repository"){.btn .btn-sm .btn-source-repository-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
-   [[ ]{.btn__icon-container} [Suggest edit]{.btn__text-container}](https://github.com/OpenOSOrg/openos/edit/main/content/sync/sharing.ipynb "Suggest edit"){.btn .btn-sm .btn-source-edit-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
-   [[ ]{.btn__icon-container} [Open issue]{.btn__text-container}](https://github.com/OpenOSOrg/openos/issues/new?title=Issue%20on%20page%20%2Fsync/sharing.html&body=Your%20issue%20content%20here. "Open an issue"){.btn .btn-sm .btn-source-issues-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
:::

::: {.dropdown .dropdown-download-buttons}

-   [[ ]{.btn__icon-container} [.ipynb]{.btn__text-container}](../_sources/sync/sharing.ipynb "Download source file"){.btn .btn-sm .btn-download-source-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
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
# Cooperating Processes and Inter-process Communication

::: {#print-main-content}
::: {#jb-print-toc}
<div>

## Contents

</div>

-   [25.1.1. Shared Memory](#shared-memory){.reference .internal .nav-link}
-   [25.1.2. Multi-threaded Processes](#multi-threaded-processes){.reference .internal .nav-link}
-   [25.1.3. Issues with Concurrent Execution](#issues-with-concurrent-execution){.reference .internal .nav-link}
-   [25.1.4. Race Conditions](#race-conditions){.reference .internal .nav-link}
:::
:::
:::

::: {#searchbox}
:::

::: {.cell .tag_remove-input .docutils .container}
:::

::: {#cooperating-processes-and-inter-process-communication .section .tex2jax_ignore .mathjax_ignore}
[]{#cont-sync-sharing}

# [25.1. ]{.section-number}Cooperating Processes and Inter-process Communication[\#](#cooperating-processes-and-inter-process-communication "Link to this heading"){.headerlink}

The process abstraction is designed to give the illusion that a program executes on its own private, isolated (virtual) machine. The OS scheduling mechanism hides the fact that the physical CPU is, in fact, shared by multiple processes. From the perspective of any given process, it appears as though its instructions execute one after the other, in the order that they appear in the program, on a dedicated CPU, without interruption or interference by the execution of other processes. The process also has sole access to a virtual address space, where it can store, and operate on, its data -- there is no concern about access to the process's memory from other processes, or that the process may inadvertently access memory that does not belong to it.

But, sometimes we want multiple processes to work together to solve a problem. How can they cooperate if they are completely isolated from each other? The short answer is, they can't. For processes to cooperate, they need some way to communicate with each other, so that they can exchange information and coordinate their activities. Let's think about some ways that multiple processes can work together, and how they can communicate.

[[Unix command pipelines]{.std .std-ref}](../intro/abstractions.html#cont-gs-abstractions-pipes){.reference .internal}

:   Each program is designed to do one thing well, and more complex operations can be created by composing multiple simple programs. Here, communication is supported by the `pipe()`{.docutils .literal .notranslate} system call, which creates a communication channel between processes. With some manipulation of file descriptors, the shell can arrange for the standard output of one process to become the standard input of the next process in the pipeline. The pipe provides both a way to pass data from one process to the next and a way to control the order in which processes execute, because a downstream process cannot read its input until after the previous process in the pipeline has started to produce some output.

Complex services

:   A complex service, such as a banking service, may have multiple logical operations that it needs to carry out, such as handling user input, executing account operations like deposits, calculating daily interest, running fraud detection analytics, etc. It is often convenient to implement the service as a collection of processes, with each process carrying out one of the major tasks of the service and the operating system [[scheduler]{.std .std-ref}](../scheduling/scheduling.html#cont-vp-scheduling){.reference .internal} ensuring that all tasks make progress concurrently. The processes may communicate by reading and writing shared files in the file system. By

Parallel computation

:   In this case, the goal is to complete a single task in less time by using multiple physical compute cores. As a trivial example, consider sorting a very large set of values. On a multi-core machine, you could create one process per core, arrange for each process to sort a portion of the input, and then merge the results together after all the individual sorts were complete. Here, processes might communicate using a combination of files in the file system (e.g., to read the original, unsorted input, and write the intermediate results from each sorting process) and pipes (e.g., to notify the merging process when each sorting process was finished).

::: {#shared-memory .section}
## [25.1.1. ]{.section-number}Shared Memory[\#](#shared-memory "Link to this heading"){.headerlink}

To support more efficient, fine-grained inter-process communication, the operating system also provides system calls to let processes explicitly share a portion of their virtual address space. This allows processes to exchange information simply by reading or writing variables that are allocated in the shared part of the address space. There are actually two ways to do this on Unix systems. The first comes from UNIX System V:

-   `segment_id = shmget(key, size, shmflg)`{.docutils .literal .notranslate} : return the identifier of the System V shared memory segment associated with the value of the argument `key`{.docutils .literal .notranslate}; may be used either to obtain the identifier of a previously created shared memory segment (when `shmflg`{.docutils .literal .notranslate} is zero and `key`{.docutils .literal .notranslate} does not have the value `IPC_PRIVATE`{.docutils .literal .notranslate}), or to create a new shared memory segment.

-   `shared_startvaddr = shmat(shmid, *shmaddr, shmflg)`{.docutils .literal .notranslate} : attach the System V shared memory segment identified by `shmid`{.docutils .literal .notranslate} to the address space of the calling process at `shmaddr`{.docutils .literal .notranslate} or an address chosen by the OS if `shmaddr`{.docutils .literal .notranslate} is `NULL`{.docutils .literal .notranslate}; return the actual starting virtual address of the shared segment in the process address space.

-   `err = shmdt(shmaddr)`{.docutils .literal .notranslate} : detach the shared memory segment located at the address specified by `shmaddr`{.docutils .literal .notranslate} from the address space of the calling process; the to-be-detached segment must be currently attached with `shmaddr`{.docutils .literal .notranslate} equal to the value returned by the attaching `shmat()`{.docutils .literal .notranslate} call.

The use of segment identifiers makes it possible for unrelated processes to share memory, however after one process creates a shared memory segment with `shmget`{.docutils .literal .notranslate}, it needs to communicate the segment id to the other processes that are allowed to share it. One way to do this is by writing the segment id into a file that can be read by the other processes. The other method for requesting shared memory comes from BSD UNIX and requires a parent process to create a shared mapping in its address space before forking child processes. The mapped segments are then shared with child processes, rather than creating a copy in the child address space.

-   `shared_startvaddr = mmap(*addr, length, prot, MAP_SHARED | MAP_ANONYMOUS, ...)`{.docutils .literal .notranslate} : create a new mapping of `length`{.docutils .literal .notranslate} bytes in the virtual address space of the calling process starting at `addr`{.docutils .literal .notranslate} or an address chosen by the OS if `addr`{.docutils .literal .notranslate} is `NULL`{.docutils .literal .notranslate}; return the actual starting virtual address of the shared segment in the process address space.

Note that `mmap`{.docutils .literal .notranslate} is often used to access persistent files using a virtual memory interface rather than the file system `read()`{.docutils .literal .notranslate} and `write()`{.docutils .literal .notranslate} interface. In the example above, `MAP_ANONYMOUS`{.docutils .literal .notranslate} indicates that the mapping is for a non-persistent virtual memory region, which is not backed by any file. (Remember that you can use `man`{.docutils .literal .notranslate} for the full details of these system calls.)

The shared memory segments are implemented in the operating system using the virtual memory mechanisms. Each process that shares the memory segment has its page tables pointing to the same underlying physical pages, so that any load or store access to a virtual address in the shared segment will be translated to the same physical location in the machine memory.
:::

::: {#multi-threaded-processes .section}
[]{#cont-sync-sharing-shared-mem}

## [25.1.2. ]{.section-number}Multi-threaded Processes[\#](#multi-threaded-processes "Link to this heading"){.headerlink}

Recall from [[Section 9]{.std .std-numref}](../scheduling/threads.html#cont-vp-threads){.reference .internal} that a process can have multiple *threads*, and that all threads in a process share the same virtual address space. This means that multi-threaded processes do not need to do any extra work to communicate using shared memory. The operating system itself is multi-threaded: every user-level process has at least one thread in the kernel, and other threads carry out asynchronous operating system activities, such as writing dirty file system blocks back to the disk. All of these kernel threads share the same operating system code and data structures. We will see later how user-level communication through pipes is implemented in the operating system by threads writing to, and reading from, a shared buffer of memory. In our discussion of concurrency and synchronization, we will use examples in multi-threaded user-level processes, since they can be presented as simple, stand-alone programs. Keep in mind that everything we say about multi-threaded processes also applies to the implementation of the operating system.

Since each thread is an independent execution entity, they need to have their own execution state. This includes a per-thread execution stack to hold local variables. In contrast, global variables and heap-allocated variables are shared by all threads in a process. Note that although each thread has its own execution stack, these are still all part of the same virtual address space, and threads in the same process are not protected from each other by the operating system. Thus, it is possible for a buggy thread to accidentally scribble on another thread's stack space, leading to bizarre behavior.
:::

::: {#issues-with-concurrent-execution .section}
[]{#cont-sync-sharing-issues}

## [25.1.3. ]{.section-number}Issues with Concurrent Execution[\#](#issues-with-concurrent-execution "Link to this heading"){.headerlink}

Regardless of whether we are using multiple processes, or a single multi-threaded process, whether we are implementing user-level programs or the operating system, we need a way to coordinate multiple concurrent activities.

*Concurrency* in computer systems means that the execution of multiple (i.e., two or more) tasks *overlaps in time*. The context switch mechanism gives us concurrent execution of multiple processes, even on a single physical CPU. *Parallelism* means that multiple tasks are executing *at the same time*. Parallelism requires multiple physical CPUs.

The operating system scheduler controls when, and for how long, any given thread is allowed to execute. Although each thread's instructions execute in program order, its execution is interleaved with other threads. And when threads share resources, such as data structures in shared memory, the arbitrary interleaving of operations from multiple threads can lead to unpredictable, and undesirable, outcomes. **Synchronization** is the mechanism that allows us to restrict the possible interleavings of threads, so that we can control how they use shared resources, reason about their behavior, and prevent undesirable outcomes. There are two main problems that synchronization helps us to solve: how to ensure that threads do not interfere with each other when they use a shared resource, and how to ensure that threads execute their operations in the correct order. For example, consider the simple program in [[Listing 25.1]{.std .std-numref}](#listing-sync-outputs){.reference .internal}, below, in which two threads each output a string:

::: {#listing-sync-outputs .literal-block-wrapper .docutils .container}
::: code-block-caption
[Listing 25.1 ]{.caption-number}[output_example.c - Uncontrolled thread interleaving example using output to the terminal.]{.caption-text}[\#](#listing-sync-outputs "Link to this code"){.headerlink}
:::

::: {.highlight-default .notranslate}
::: highlight
     1#include <pthread.h>
     2#include <stdlib.h>
     3#include <sys/types.h>
     4#include <unistd.h>
     5#include <string.h>
     6#include <stdio.h>
     7
     8/* This function is intended so simulate a thread needing to do some other 
     9 * work in between output statements.
    10 */
    11static long waste_cpu()
    12{
    13    long dummy = 0;
    14    for (int i = 0; i < 10000; i++) {
    15        dummy += rand();
    16    }
    17    return dummy;
    18}
    19
    20/* Start of function executed by each thread.
    21 * Each character of the argument string is printed out one-by-one
    22 * in a separate system call. 
    23 * To increase the number of interleavings, we voluntarily yield the 
    24 * CPU after each character is output.
    25 */
    26static void *write_one_by_one(void *arg)
    27{
    28    char *mystr = (char *)arg;
    29      
    30    for (int i = 0; i < strlen(mystr); i++) {
    31        write(STDOUT_FILENO, &mystr[i], 1); 
    32        waste_cpu();
    33    }
    34  
    35    return (void *)0;       
    36}
    37/* End of function executed by each thread. */
    38
    39
    40int main(int argc, char **argv)
    41{
    42    pthread_t tid1, tid2;
    43    char *str1 = "Hello";
    44    char *str2 = "Goodbye";
    45
    46    /* Normally we'd want to test the return value of pthread_create. */
    47
    48    (void)pthread_create(&tid1, NULL, write_one_by_one, (void *)str1 );
    49    (void)pthread_create(&tid2, NULL, write_one_by_one, (void *)str2 );
    50
    51    /* Wait for child threads to finish */
    52    pthread_join(tid1, NULL);
    53    pthread_join(tid2, NULL);
    54
    55    (void)write(STDOUT_FILENO, "\n", 1);    
    56    return 0;
    57}
    58
:::
:::
:::

When this program is run, the main function creates two new threads, passing each a string to output on the terminal. Once created, the threads start executing concurrently in the `write_one_by_one`{.docutils .literal .notranslate} function. Each thread loops over its input string, calling the `write()`{.docutils .literal .notranslate} system call to output the characters one by one. (We could, of course, call `write()`{.docutils .literal .notranslate} to output the entire string at once, or use the C library `printf`{.docutils .literal .notranslate} function, but we want to see what could happen when we don't have the internal synchronization that these functions provide.)

What do you expect the result of running this program to be? Let's give it a try a few times!

::: {.cell .tag_remove-input .docutils .container}
::: {.cell_output .docutils .container}
:::
:::

The output doesn't look great. Not only is the output unreadable, it is also different from one run to the next. (And each time we build this book, we don't know exactly what output you will be seeing! Maybe some of the runs even produce something reasonable.) What we want to see is either "HelloGoodbye" or "GoodbyeHello" --- by adding synchronization, we can restrict the interleavings of the output to just these two possibilities. And, if we wanted to ensure that "Hello" always appeared on the terminal before "Goodbye", another form of synchronization would allow us to enforce that ordering as well. In fact, the C library `printf()`{.docutils .literal .notranslate} family of functions, and the internal implementation of the `write()`{.docutils .literal .notranslate} system call, contain synchronization to ensure that output from one call is not interleaved with another, but if we wanted to ensure that "Hello" is displayed before "Goodbye", we would still need to add more synchronization on top of the `write()`{.docutils .literal .notranslate} or `printf()`{.docutils .literal .notranslate} functions.

Let's look at another illustrative example of the problems that can arise when we don't control concurrent execution.

::: {#listing-sync-bank .literal-block-wrapper .docutils .container}
::: code-block-caption
[Listing 25.2 ]{.caption-number}[deposit function from bank_deposit.c - Simple bank account example.]{.caption-text}[\#](#listing-sync-bank "Link to this code"){.headerlink}
:::

::: {.highlight-default .notranslate}
::: highlight
    1static void deposit(int account, money_t amount)
    2{
    3    money_t balance = get_balance(account);
    4    balance += amount;
    5    put_balance(account, balance);
    6
    7    return;        
    8}
:::
:::
:::

In [[Listing 25.2]{.std .std-numref}](#listing-sync-bank){.reference .internal} we see a simplified example of a function that is part of a program to maintain a bank account balance at the Bank of Lost Funds. When running on a single thread, the `deposit`{.docutils .literal .notranslate} function is trivially correct: after it completes execution, the value of `balance`{.docutils .literal .notranslate} stored back to the `account`{.docutils .literal .notranslate} will be `amount`{.docutils .literal .notranslate} greater than it was before the function was invoked. Problems arise, however, when multiple threads run this function concurrently.

![[Fig. 25.1 ]{.caption-number}[(a) The body of the `deposit()`{.docutils .literal .notranslate} function executed by two threads, (b) one possible interleaving of the execution of the threads, and (c) a second possible interleaving.]{.caption-text}[\#](#fig-sync-badbank "Link to this image"){.headerlink}](../_images/bank_deposit_interleaving.drawio.png){style="width: 85%;"}

In [[Fig. 25.1]{.std .std-numref}](#fig-sync-badbank){.reference .internal}(b), we see one possible interleaving when this function is invoked by two threads nearly simultaneously. In this case Thread 1 is interrupted after it has read the current value of `balance`{.docutils .literal .notranslate}, but before it could store the new value back to memory. Thread 2 then gets to run and completes its execution of the `deposit()`{.docutils .literal .notranslate} function before being interrupted. Finally, Thread 1 can run again and complete its execution of `deposit()`{.docutils .literal .notranslate} by storing its local `balance`{.docutils .literal .notranslate} variable back to the account. The result is that the update performed by Thread 2 is lost, being over-written by Thread 1's computation. After depositing a total of \$150 to the account we have a final balance of \$50. Context switches are unpredictable, however, and other interleavings of the thread executions are also possible. In [[Fig. 25.1]{.std .std-numref}](#fig-sync-badbank){.reference .internal}(c) we see another possible schedule, where Thread 1's update to the account balance is overwritten by Thread 2.

Let's try running the bank deposit program a few times and see what happens.

::: {.dropdown .admonition}
Click to show the full source code of the bank balance program.

Here is the complete code for the bank balance example, including the creation of two threads to run the deposit function on the same account with different amounts.

::: {#listing-sync-bank-full .literal-block-wrapper .docutils .container}
::: code-block-caption
[Listing 25.3 ]{.caption-number}[bank_deposit.c - Full source code for simple bank account example]{.caption-text}[\#](#listing-sync-bank-full "Link to this code"){.headerlink}
:::

::: {.highlight-default .notranslate}
::: highlight
      1#include <pthread.h>
      2#include <stdlib.h>
      3#include <sys/types.h>
      4#include <unistd.h>
      5#include <string.h>
      6#include <stdio.h>
      7
      8#define money_t double
      9#define MAX_ACCOUNTS 1000
     10
     11struct deposit_s {
     12    int account_num;
     13    money_t amount;
     14};
     15
     16money_t accounts[MAX_ACCOUNTS];
     17
     18/* This function is intended so simulate the work of retrieving the current balance
     19 * for a given account number. It just spins and yields a random number of times.
     20 */
     21static money_t get_balance(int account_num)
     22{
     23    long dummy = 0;
     24    int nyield = rand() % 10;
     25    int nspin = rand() % 1000;
     26
     27
     28    for (int i = 0; i < nyield; i++) {
     29        sched_yield();
     30        for (int j = 0; j < nspin; j++) {
     31            dummy += rand();
     32        }
     33    }
     34
     35    return accounts[account_num];
     36}
     37
     38/* This function is intended so simulate the work of saving the current balance
     39 * back to a given account number. It just spins and yields a random number of times.
     40 */
     41static void put_balance(int account_num, money_t balance)
     42{
     43    long dummy = 0;
     44    int nyield = rand() % 10;
     45    int nspin = rand() % 1000;
     46
     47
     48    for (int i = 0; i < nyield; i++) {
     49        sched_yield();
     50        for (int j = 0; j < nspin; j++) {
     51            dummy += rand();
     52        }
     53    }
     54
     55    accounts[account_num] = balance;
     56    return;
     57}
     58
     59/* Start of deposit function */
     60static void deposit(int account, money_t amount)
     61{
     62    money_t balance = get_balance(account);
     63    balance += amount;
     64    put_balance(account, balance);
     65
     66    return;        
     67}
     68/* End of deposit function */
     69
     70static void *deposit_thread(void *arg)
     71{
     72    struct deposit_s *my_deposit = (struct deposit_s *)arg;
     73    deposit(my_deposit->account_num, my_deposit->amount);
     74
     75    return (void *)0;
     76}
     77
     78int main(int argc, char **argv)
     79{
     80    pthread_t tid1, tid2;
     81    int account_num = 100;
     82    money_t amt1 = 50.00;
     83    money_t amt2 = 100.00; 
     84
     85    struct deposit_s dep1 = {account_num, amt1};
     86    struct deposit_s dep2 = {account_num, amt2}; 
     87
     88    /* Normally we'd want to test the return value of pthread_create. */
     89
     90    (void)pthread_create(&tid1, NULL, deposit_thread, (void *)&dep1 );
     91    (void)pthread_create(&tid2, NULL, deposit_thread, (void *)&dep2 );
     92
     93    /* Wait for child threads to finish */
     94    pthread_join(tid1, NULL);
     95    pthread_join(tid2, NULL);
     96
     97    printf("Final balance of account #%d after depositing $%.2lf and $%.2lf is $%.2lf\n",
     98           account_num, amt1, amt2, accounts[account_num] );
     99    return 0;
    100}
:::
:::
:::
:::

::: {.highlight-default .notranslate}
::: highlight
:::
:::

::: {.cell .tag_remove-input .docutils .container}
::: {.cell_output .docutils .container}
:::
:::
:::

::: {#race-conditions .section}
## [25.1.4. ]{.section-number}Race Conditions[\#](#race-conditions "Link to this heading"){.headerlink}

The unpredictable and undesirable outcomes that we have seen in the previous examples arise because of **race conditions**. A race condition occurs whenever two or more threads access a shared resource (like the terminal device, or the variable that stores the bank account balance), and the outcome depends on the order in which the accesses occur. Clearly, this implies that at least one of the accesses must be a write operation, since the outcome of concurrent read operations is not dependent on the order they occur. Logically, the threads are racing with each other to use the resource, and we don't know which one will come first. Sometimes, the result of the race will be the one we want, and sometimes things can go horribly wrong. Race condition bugs are extremely tricky to diagnose and fix, since the program might produce the correct results millions of times before failing.

Race conditions happen even on a single CPU because asynchronous events occur arbitrarily during thread execution. For example, the network controller raises an interrupt upon arrival of a network packet, which causes the current thread to be suspended while the interrupt handler runs. Or a timer interrupt occurs and the OS scheduler switches the CPU from the current thread to another thread. With multiple CPUs, threads running in parallel on different CPUs can read and write the same memory location. Multi-threaded programs must be designed so that they can execute correctly in the face of such asynchrony.

In our simple example programs, we added extra code to make it more likely for the negative consequences of race conditions to manifest. Without those added operations, the code executed by each thread is short enough to complete in a single time slice, and the threads are less likely to interfere with each other. However, the race condition is still there, lurking in our code.

Consider the example in [[Listing 25.4]{.std .std-numref}](#listing-sync-counter){.reference .internal}, in which two threads either increment or decrement a shared counter some number of times. The arguments to this program let you try different numbers of threads, and different numbers of iterations for each thread to either increment or decrement the shared counter. The program always creates an equal number of incrementing or decrementing threads, and each thread does the same amount of work, so we would expect the final value of the counter to be the same as its initial value when all the threads are done.

::: {#listing-sync-counter .literal-block-wrapper .docutils .container}
::: code-block-caption
[Listing 25.4 ]{.caption-number}[counter.c - Two threads increment and decrement a shared counter without synchronization.]{.caption-text}[\#](#listing-sync-counter "Link to this code"){.headerlink}
:::

::: {.highlight-default .notranslate}
::: highlight
    #include <pthread.h>
    #include <stdlib.h>
    #include <sys/types.h>
    #include <unistd.h>
    #include <string.h>
    #include <stdio.h>

    volatile long shared_counter;

    static void *increment_thread(void *arg)
    {
        long niters = (long)arg;
        for (long i = 0; i < niters; i++) {
            shared_counter++;
        }

        return (void *)0;
    }

    static void *decrement_thread(void *arg)
    {
        long niters = (long)arg;

        for (long i = 0; i < niters; i++) {
            shared_counter--;
        }

        return (void *)0;
    }

    int main(int argc, char **argv)
    {
        pthread_t *tids;
        long niters;
        int nthreads;
        
        if (argc != 3) {
            fprintf(stderr,"Usage: %s <num_threads> <num_iters>\n",argv[0]);
            return 1;
        }

        nthreads = atoi(argv[1]);
        niters = atoi(argv[2]);
        shared_counter = 0;
        
        printf("Main thread: Beginning test with %d threads\n", nthreads);
        
        tids = (pthread_t *)malloc(nthreads * sizeof(pthread_t));
        
        /* We create the same number of increment and decrement threads, each doing the same number of iterations. 
         * When all threads have completed, we expect the final value of the shared counter to be the same as its
         * initial value (i.e., 0).
         */
        for (int i = 0; i < nthreads; i+=2) {
            (void)pthread_create(&tids[i], NULL, increment_thread, (void *)niters );
            (void)pthread_create(&tids[i+1], NULL, decrement_thread, (void *)niters );
        }
        
        /* Wait for child threads to finish */
        for (int i = 0; i < nthreads; i+=2) {
            pthread_join(tids[i], NULL);
            pthread_join(tids[i+1], NULL);
        }
        
        printf("Main thread: Final value of shared counter is %ld\n", shared_counter);

        return 0;
    }
:::
:::
:::

::: {.cell .tag_remove-input .docutils .container}
::: {.cell_output .docutils .container}
:::
:::

Even though it looks like the racing thread accesses to the shared counter variable are each just a single line of code, we still have unpredictable final results. The reason is because that single line of C source code, `shared_counter++`{.docutils .literal .notranslate} or `shared_counter--`{.docutils .literal .notranslate} becomes three lines of machine code when the program is compiled, as shown in [[Listing 25.5]{.std .std-numref}](#listing-sync-counter-assembly){.reference .internal}. (Try `make counter.s`{.docutils .literal .notranslate}, and see if you can find these lines in the assembly file `counter.s`{.docutils .literal .notranslate}.) The highlighted lines load the value of the counter from memory into a register, decrement the value in the register, and then store the register value back to memory. Context switches can occur between any of these statements, leading to exactly the same interleaving problems that we saw in the bank account example.

::: {#listing-sync-counter-assembly .literal-block-wrapper .docutils .container}
::: code-block-caption
[Listing 25.5 ]{.caption-number}[Assembly code snippet of loop in `decrement_thread()`{.docutils .literal .notranslate} function.]{.caption-text}[\#](#listing-sync-counter-assembly "Link to this code"){.headerlink}
:::

::: {.highlight-default .notranslate}
::: highlight
     1decrement_thread:
     2.LFB63:
     3 .cfi_startproc
     4 endbr64
     5 testq   %rdi, %rdi
     6 jle .L7
     7 xorl    %edx, %edx
     8 .p2align 4,,10
     9 .p2align 3
    10.L8:
    11   movq    shared_counter(%rip), %rax
    12  addq    $1, %rdx
    13   subq    $1, %rax
    14    movq    %rax, shared_counter(%rip)
    15  cmpq    %rdx, %rdi
    16 jne .L8
    17.L7:
    18 xorl    %eax, %eax
    19 ret
    20 .cfi_endproc
:::
:::
:::

Clearly, uncontrolled sharing can lead to serious problems. In the next chapter, we define the problem a bit more formally. The subsequent chapters look at some ways to solve the problem.
:::
:::

::: prev-next-area
[](basic.html "previous page"){.left-prev}

::: prev-next-info
previous

[25. ]{.section-number}Basic Synchronization
:::

[](criticalsection.html "next page"){.right-next}

::: prev-next-info
next

[25.2. ]{.section-number}The Critical Section Problem
:::
:::
:::

::: {.bd-sidebar-secondary .bd-toc}
::: {.sidebar-secondary-items .sidebar-secondary__inner}
::: sidebar-secondary-item
::: {.page-toc .tocsection .onthispage}
Contents
:::

-   [25.1.1. Shared Memory](#shared-memory){.reference .internal .nav-link}
-   [25.1.2. Multi-threaded Processes](#multi-threaded-processes){.reference .internal .nav-link}
-   [25.1.3. Issues with Concurrent Execution](#issues-with-concurrent-execution){.reference .internal .nav-link}
-   [25.1.4. Race Conditions](#race-conditions){.reference .internal .nav-link}
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
