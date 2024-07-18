---
docsearch:language: en
lang: en
title: 25.2. The Critical Section Problem --- Introduction to Operating Systems
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
    -   [25.1. Cooperating Processes and Inter-process Communication](sharing.html){.reference .internal}
    -   [25.2. The Critical Section Problem](#){.current .reference .internal}
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

-   [[ ![JupyterHub logo](../_static/images/logo_jupyterhub.svg) ]{.btn__icon-container} [JupyterHub]{.btn__text-container}](https://jupyterhub-opf-jupyterhub.apps.smaug.na.operate-first.cloud/hub/user-redirect/git-pull?repo=https%3A//github.com/OpenOSOrg/openos&urlpath=lab/tree/openos/content/sync/criticalsection.ipynb&branch=main "Launch on JupyterHub"){.btn .btn-sm .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
:::

::: {.dropdown .dropdown-source-buttons}

-   [[ ]{.btn__icon-container} [Repository]{.btn__text-container}](https://github.com/OpenOSOrg/openos "Source repository"){.btn .btn-sm .btn-source-repository-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
-   [[ ]{.btn__icon-container} [Suggest edit]{.btn__text-container}](https://github.com/OpenOSOrg/openos/edit/main/content/sync/criticalsection.ipynb "Suggest edit"){.btn .btn-sm .btn-source-edit-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
-   [[ ]{.btn__icon-container} [Open issue]{.btn__text-container}](https://github.com/OpenOSOrg/openos/issues/new?title=Issue%20on%20page%20%2Fsync/criticalsection.html&body=Your%20issue%20content%20here. "Open an issue"){.btn .btn-sm .btn-source-issues-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
:::

::: {.dropdown .dropdown-download-buttons}

-   [[ ]{.btn__icon-container} [.ipynb]{.btn__text-container}](../_sources/sync/criticalsection.ipynb "Download source file"){.btn .btn-sm .btn-download-source-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
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
# The Critical Section Problem

::: {#print-main-content}
::: {#jb-print-toc}
<div>

## Contents

</div>

-   [25.2.1. Problem Definition](#problem-definition){.reference .internal .nav-link}
-   [25.2.2. Abstracting the Problem](#abstracting-the-problem){.reference .internal .nav-link}
:::
:::
:::

::: {#searchbox}
:::

::: {.cell .tag_remove-input .docutils .container}
:::

::: {#the-critical-section-problem .section .tex2jax_ignore .mathjax_ignore}
[]{#cont-sync-criticalsection}

# [25.2. ]{.section-number}The Critical Section Problem[\#](#the-critical-section-problem "Link to this heading"){.headerlink}

The problem of controlling concurrent access to shared data was recognized very early. In an \[undated lecture\]`https://www.cs.utexas.edu/users/EWD/translations/EWD35-English.html`{.docutils .literal .notranslate} from 1962 or 1963, Dutch computer scientist Edsger W. Dijkstra described what has come to be known as the *critical section problem*. Each thread executes some *critical section* of code that must be guarded against concurrent execution, i.e., only one thread is allowed to be executing in its critical section at any given time. The problem is to design a protocol that threads must execute prior to entering their critical section that will enforce the single-access rule. The term *critical section* is unfortunately misleading, as it should be obvious that it is the *shared data* that must be protected from concurrent access, and not the code. Think of the critical section as the code that must execute without interference in order to use the shared data correctly. In the shared counter example, the loop body in the `increment_thread()`{.docutils .literal .notranslate} and `decrement_thread()`{.docutils .literal .notranslate} functions are the critical sections for the counter variable. To identify the critical sections of code, we need to identify all the cases where shared data must be protected against simultaneous modification or access to prevent race conditions. Note also that the same code can be invoked to operate on different data -- for example, `deposit()`{.docutils .literal .notranslate} called for account #100 in Thread 1, and `deposit()`{.docutils .literal .notranslate} called for account #200 in Thread 2 will not interfere with each other. In this case, we have critical sections for two different resources (i.e., two different bank accounts) and they do not need to be protected from each other.

These ideas will become more concrete by the end of this Chapter, but initially we will reason about a single shared resource (like our `counter`{.docutils .literal .notranslate} variable), accessed repeatedly by multiple threads, with some additional code before and after the critical section that does not make any accesses to the shared variable.

::: {#problem-definition .section}
## [25.2.1. ]{.section-number}Problem Definition[\#](#problem-definition "Link to this heading"){.headerlink}

In its classical form, a solution to the critical section problem must meet the following requirements:

Mutual Exclusion

:   Only one thread can be executing in its critical section at a time.

Progress

:   If no thread is executing in its critical section, and some threads want to enter their critical section, then eventually some thread must be granted entry to its critical section. Threads that are executing in their *remainder* code (i.e., code that is unrelated to the critical section) must not delay threads that want to enter the critical section.

Bounded Waiting (No Starvation)

:   Once a thread has requested entry to its critical section, there is a limit on how many times other threads are allowed to enter their critical sections ahead of it.

The *mutual exclusion* requirement is fairly obvious---we want to ensure that only one thread at a time can be manipulating the shared data. The *progress* requirement disallows solutions that meet the mutual exclusion requirement by not allowing *any* thread to enter the critical section. Finally, the *bounded waiting* requirement ensures that every thread has a fair chance to use the shared data.

To these basic requirements, we will add a fourth consideration:

Performance

:   The overhead of entering and exiting the critical section should be small with respect to the work being done within it.

In some solutions that we will look at the bounded waiting requirement is not met, but it is statistically unlikely in real systems that a thread will be continually passed over in favor of other threads entering the critical section.

We also make a number of assumptions:

1.  Each thread is executing at non-zero speed, but we make no assumptions about the relative speed of the threads.

2.  We assume that individual machine instructions such as `load`{.docutils .literal .notranslate}, `store`{.docutils .literal .notranslate}, or `add`{.docutils .literal .notranslate} are *atomic*, meaning that they are indivisible. The execution of multiple threads is interleaved at the level of individual machine instructions. For example, if Thread 1 reads a variable and Thread 2 writes the variable at nearly the same time, then Thread 1 will read either the old value, or the new value, but not some mixture of the old and new values.

3.  The operations in each thread are executed in the order that they appear in the program code, and the result of concurrent execution is equivalent to some interleaving of operations from each of the concurrent threads. (Note that this last assumption is not true of modern cpu architectures, but we will omit the topic of memory consistency models for now.)

With these requirements and assumptions in place, we now turn our attention to designing a protocol that threads can use to coordinate their use of shared data. Once we have identified the critical sections, we insert an *entry section* before the critical section, and an *exit section* immediately after the critical section. Each thread must request permission to enter its critical section, by executing the protocol in its entry section. When it completes the entry, the thread is guaranteed to have exclusive access to the shared data accessed within the critical section. When it finishes the critical section, the thread executes the code in the exit section to make the critical section available to other threads. Each thread may request entry to its critical section repeatedly. All other code executed by the thread, either before entry to, or after exit from, the critical section will be referred to as the *remainder* of the code.

[[Fig. 25.2]{.std .std-numref}](#fig-sync-criticalsection){.reference .internal} illustrates these concepts with a concrete code example from the `increment_thread`{.docutils .literal .notranslate} function in the shared counter program. In this figure, we are showing where the entry and exit sections need to be added around the critical section of code that accesses the shared variable, without specifying what goes into those sections.

![[Fig. 25.2 ]{.caption-number}[Abstract view of a critical section of code, surrounded by entry and exit sections (left), and example of these concepts in the `increment_thread`{.docutils .literal .notranslate} function (right).]{.caption-text}[\#](#fig-sync-criticalsection "Link to this image"){.headerlink}](../_images/critical_section.drawio.png){style="width: 85%;"}
:::

::: {#abstracting-the-problem .section}
[]{#cont-sync-criticalsection-locks}

## [25.2.2. ]{.section-number}Abstracting the Problem[\#](#abstracting-the-problem "Link to this heading"){.headerlink}

We can encapsulate solutions to the critical section problem into a *lock* abstract data type, with the following operations:

-   `acquire()`{.docutils .literal .notranslate} : Obtain exclusive access to a critical section; this function returns only when the calling thread is granted entry to the critical section.

-   `release()`{.docutils .literal .notranslate} : Leave the critical region, making it available to other threads.

The lock data type may also have some private data, which can be used by the `acquire()`{.docutils .literal .notranslate} and `release()`{.docutils .literal .notranslate} functions, but is not otherwise visible. Exactly what this data might be will depend on the implementation of these functions.

We associate a lock object with the shared data that we need to protect. Threads must invoke the `lock.acquire()`{.docutils .literal .notranslate} function to enter the critical section, and the `lock.release()`{.docutils .literal .notranslate} function to leave the critical section, as shown in [[Fig. 25.3]{.std .std-numref}](#fig-sync-criticalsection-withlock){.reference .internal}. Note that we can have multiple lock objects that protect different data objects, such as a separate lock for each bank account. Threads simply simply have to invoke the acquire() and release() operations on the right lock object.

The lock data type is sometimes called a *mutex*, because it is used to guarantee *mut*ual *ex*clusion, and the operations on a mutex are often called `lock()`{.docutils .literal .notranslate} and `unlock()`{.docutils .literal .notranslate}, with the same semantics as the `acquire`{.docutils .literal .notranslate} and `release`{.docutils .literal .notranslate} functions.

![[Fig. 25.3 ]{.caption-number}[e w Encapsulating critical section entry and exit with operations on a lock object.]{.caption-text}[\#](#fig-sync-criticalsection-withlock "Link to this image"){.headerlink}](../_images/critical_section_with_lock.drawio.png){style="width: 85%;"}

The pthreads specification includes the `pthread_mutex_t`{.docutils .literal .notranslate} data type, and operations `pthread_mutex_lock(mutex)`{.docutils .literal .notranslate} and `pthread_mutex_unlock(mutex)`{.docutils .literal .notranslate} to acquire and release the mutex, respectively. The code in [[Listing 25.6]{.std .std-numref}](#listing-sync-pthread-mutex){.reference .internal} shows how we use the pthreads mutex to protect access to the shared counter variable.

::: {#listing-sync-pthread-mutex .literal-block-wrapper .docutils .container}
::: code-block-caption
[Listing 25.6 ]{.caption-number}[Protecting access to the shared counter using a pthread mutex.]{.caption-text}[\#](#listing-sync-pthread-mutex "Link to this code"){.headerlink}
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
     8pthread_mutex_t mutex = PTHREAD_MUTEX_INITIALIZER;
     9volatile long shared_counter;
    10
    11static void *increment_thread(void *arg)
    12{
    13    long niters = (long)arg;
    14    for (int i = 0; i < niters; i++) {
    15        pthread_mutex_lock(&mutex);
    16        shared_counter++;
    17        pthread_mutex_unlock(&mutex);
    18    }
    19
    20    return (void *)0;
    21}
    22
    23static void *decrement_thread(void *arg)
    24{
    25    long niters = (long)arg;
    26
    27    for (int i = 0; i < niters; i++) {
    28        pthread_mutex_lock(&mutex);
    29        shared_counter--;
    30        pthread_mutex_unlock(&mutex);
    31    }
    32
    33    return (void *)0;
    34}
    35
    36int main(int argc, char **argv)
    37{
    38    pthread_t *tids;
    39    long niters;
    40    int nthreads, i;
    41    
    42    if (argc != 3) {
    43        fprintf(stderr,"Usage: %s <num_threads> <num_iters>\n",argv[0]);
    44        return 1;
    45    }
    46
    47    nthreads = atoi(argv[1]);
    48    niters = atoi(argv[2]);
    49    shared_counter = 0;
    50    
    51    printf("Main thread: Beginning test with %d threads\n", nthreads);
    52    
    53    tids = (pthread_t *)malloc(nthreads * sizeof(pthread_t));
    54    
    55    /* We create the same number of increment and decrement threads, each doing the same number of iterations. 
    56     * When all threads have completed, we expect the final value of the shared counter to be the same as its
    57     * initial value (i.e., 0).
    58     */
    59    for (i = 0; i < nthreads; i+=2) {
    60        (void)pthread_create(&tids[i], NULL, increment_thread, (void *)niters );
    61        (void)pthread_create(&tids[i+1], NULL, decrement_thread, (void *)niters );
    62    }
    63    
    64    /* Wait for child threads to finish */
    65    for (i = 0; i < nthreads; i+=2) {
    66        pthread_join(tids[i], NULL);
    67        pthread_join(tids[i+1], NULL);
    68    }
    69    
    70    printf("Main thread: Final value of shared counter is %ld\n", shared_counter);
    71
    72    return 0;
    73}
:::
:::
:::

Now, let's try running this code and see if we get the expected final counter value, 0.

::: {.cell .tag_remove-input .docutils .container}
::: {.cell_output .docutils .container}
:::
:::

That looks a lot better! So, armed with a lock abstraction (called mutex in the pthreads library), we have a working solution to the critical section problem. In the next chapter, we will explore the internal implementation of the `acquire()`{.docutils .literal .notranslate} and `release()`{.docutils .literal .notranslate} functions.
:::
:::

::: prev-next-area
[](sharing.html "previous page"){.left-prev}

::: prev-next-info
previous

[25.1. ]{.section-number}Cooperating Processes and Inter-process Communication
:::

[](locks.html "next page"){.right-next}

::: prev-next-info
next

[25.3. ]{.section-number}Implementing Locks
:::
:::
:::

::: {.bd-sidebar-secondary .bd-toc}
::: {.sidebar-secondary-items .sidebar-secondary__inner}
::: sidebar-secondary-item
::: {.page-toc .tocsection .onthispage}
Contents
:::

-   [25.2.1. Problem Definition](#problem-definition){.reference .internal .nav-link}
-   [25.2.2. Abstracting the Problem](#abstracting-the-problem){.reference .internal .nav-link}
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
