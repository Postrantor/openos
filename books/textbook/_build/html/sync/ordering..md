---
docsearch:language: en
lang: en
title: 25.4. Ordering Thread Events --- Introduction to Operating Systems
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
    -   [25.2. The Critical Section Problem](criticalsection.html){.reference .internal}
    -   [25.3. Implementing Locks](locks.html){.reference .internal}
    -   [25.4. Ordering Thread Events](#){.current .reference .internal}
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

-   [[ ![JupyterHub logo](../_static/images/logo_jupyterhub.svg) ]{.btn__icon-container} [JupyterHub]{.btn__text-container}](https://jupyterhub-opf-jupyterhub.apps.smaug.na.operate-first.cloud/hub/user-redirect/git-pull?repo=https%3A//github.com/OpenOSOrg/openos&urlpath=lab/tree/openos/content/sync/ordering.ipynb&branch=main "Launch on JupyterHub"){.btn .btn-sm .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
:::

::: {.dropdown .dropdown-source-buttons}

-   [[ ]{.btn__icon-container} [Repository]{.btn__text-container}](https://github.com/OpenOSOrg/openos "Source repository"){.btn .btn-sm .btn-source-repository-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
-   [[ ]{.btn__icon-container} [Suggest edit]{.btn__text-container}](https://github.com/OpenOSOrg/openos/edit/main/content/sync/ordering.ipynb "Suggest edit"){.btn .btn-sm .btn-source-edit-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
-   [[ ]{.btn__icon-container} [Open issue]{.btn__text-container}](https://github.com/OpenOSOrg/openos/issues/new?title=Issue%20on%20page%20%2Fsync/ordering.html&body=Your%20issue%20content%20here. "Open an issue"){.btn .btn-sm .btn-source-issues-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
:::

::: {.dropdown .dropdown-download-buttons}

-   [[ ]{.btn__icon-container} [.ipynb]{.btn__text-container}](../_sources/sync/ordering.ipynb "Download source file"){.btn .btn-sm .btn-download-source-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
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
# Ordering Thread Events

::: {#print-main-content}
::: {#jb-print-toc}
<div>

## Contents

</div>

-   [25.4.1. The Bounded Buffer Problem](#the-bounded-buffer-problem){.reference .internal .nav-link}
-   [25.4.2. Semaphores](#semaphores){.reference .internal .nav-link}
-   [25.4.3. Condition Variables](#condition-variables){.reference .internal .nav-link}
:::
:::
:::

::: {#searchbox}
:::

::: {.cell .tag_remove-input .docutils .container}
:::

::: {#ordering-thread-events .section .tex2jax_ignore .mathjax_ignore}
[]{#cont-sync-ordering}

# [25.4. ]{.section-number}Ordering Thread Events[\#](#ordering-thread-events "Link to this heading"){.headerlink}

As we saw in [[Section 25.3.4]{.std .std-numref}](locks.html#cont-sync-locks-sleep-wakeup){.reference .internal}, the `wait_queue`{.docutils .literal .notranslate} data structure provides a way for threads to avoid wasting CPU time while they are waiting for something to happen. The mechanics of atomically putting a thread to sleep on a wait_queue must be handled carefully, and require some interaction with the CPU scheduler. Different operating systems have different ways of doing this, and we will revisit this issue when we discuss locking in the Linux kernel. For now, we will simply use these abstractions to explore other synchronization problems and build some higher-level synchronization primitives.

As a reminder, here are the operations on a `wait_queue`{.docutils .literal .notranslate}:

-   `sleep(wait_queue)`{.docutils .literal .notranslate}: blocks the calling thread; thread is added to `wait_queue`{.docutils .literal .notranslate} and another thread is selected to run.

-   `wakeup(wait_queue)`{.docutils .literal .notranslate}: removes a thread from `wait_queue`{.docutils .literal .notranslate} and adds it to the scheduler Ready queue.

-   `wakeup_all(wait_queue)`{.docutils .literal .notranslate}: moves *all* threads from `wait_queue`{.docutils .literal .notranslate} to the the scheduler Ready queue.

Waiting for a lock to be released is just one possible reason that a thread might need to wait. We saw another example in the code of [[Listing 25.22]{.std .std-numref}](locks.html#listing-sync-check-spinlock-fairness){.reference .internal}, where each child thread spins waiting for the parent to finish creating all the other children. The `wakeup_all()`{.docutils .literal .notranslate} operation is handy in a case like this where we want to allow all the waiting threads to resume activity.

There are many examples where we need to control the order in which threads can execute. In the remainder of this chapter, we will consider some of these problems.

::: {#the-bounded-buffer-problem .section}
## [25.4.1. ]{.section-number}The Bounded Buffer Problem[\#](#the-bounded-buffer-problem "Link to this heading"){.headerlink}

Let's look at one classic example, known as the Bounded Buffer problem (also called the Producer/Consumer problem). In this problem, a set of threads communicate through a shared circular buffer that can hold N items. We maintain a count of the number of items currently in the buffer. Producer threads generate new items and add them to the buffer; consumer threads remove items from the buffer. The items could be an arbitrary structure, or just bytes of data. We will begin by considering the special case of a single producer and a single consumer. This problem is essentially a simplified version of the [[pipe abstraction]{.std .std-ref}](../intro/abstractions.html#cont-gs-abstractions-pipes){.reference .internal}.

![[Fig. 25.5 ]{.caption-number}[The bounded buffer problem. Producers continually add items to the buffer and consumers continually remove items.]{.caption-text}[\#](#fig-sync-ordering-bbuf-setup "Link to this image"){.headerlink}](../_images/bbuf_setup.drawio.png){style="width: 75%;"}

We illustrate this problem setup in [[Fig. 25.5]{.std .std-numref}](#fig-sync-ordering-bbuf-setup){.reference .internal}. We have declared a `struct bounded_buffer`{.docutils .literal .notranslate} data type to encapsulate the properties of the bounded buffer, and we have declared the `count`{.docutils .literal .notranslate} member as an `atomic_int`{.docutils .literal .notranslate} so that simple increment and decrement operations on `count`{.docutils .literal .notranslate} will be performed atomically; we use ordinary int types for the `in`{.docutils .literal .notranslate} and `out`{.docutils .literal .notranslate} members since `in`{.docutils .literal .notranslate} is only used the the producer, and `out`{.docutils .literal .notranslate} is only used by the consumer. In the code snippets, however, there is no coordination (or *synchronization*) between the producer thread and the consumer thread. The producer blindly stuffs items into the buffer, possibly over-writing previous items that the consumer has not had a chance to remove yet. Similarly, the consumer blindly grabs items out of the buffer, without regard for whether the producer has actually filled those buffer slots or not. Clearly, this will not lead to correct results, even if the count is correct! We must introduce some synchronization constraints: the producer must wait if the buffer is full (i.e., if `count == N`{.docutils .literal .notranslate}); the consumer must wait if the buffer is empty (i.e., if `count == 0`{.docutils .literal .notranslate}). In addition, we require the producer to wake up a waiting consumer when the first item is added to the buffer (i.e., when the buffer becomes non-empty), and for the consumer to wake up a waiting producer when an item is removed from a full buffer (i.e., when the buffer becomes non-full).

Let's try using the `sleep()`{.docutils .literal .notranslate} and `wakeup()`{.docutils .literal .notranslate} operations to synchronize our threads, as shown in [[Listing 25.23]{.std .std-numref}](#listing-sync-ordering-bbuf-wq){.reference .internal}. (Note that this code example is incomplete, and is provided for illustration purposes only. The `sleep()`{.docutils .literal .notranslate} function here is our assumed wait_queue sleep operation, and not the C library `sleep()`{.docutils .literal .notranslate}.)

::: {#listing-sync-ordering-bbuf-wq .literal-block-wrapper .docutils .container}
::: code-block-caption
[Listing 25.23 ]{.caption-number}[Bounded buffer with sleep() and wakeup()]{.caption-text}[\#](#listing-sync-ordering-bbuf-wq "Link to this code"){.headerlink}
:::

::: {.highlight-default .notranslate}
::: highlight
    /* For illustration purposes only. 
     * This code is not complete and cannot be compiled into an executable.
     */
    #include <stdatomic.h>
    #include <stdbool.h>
    #include "waitqueue.h"

    extern char produce_item();
    extern void consume_item(char item);

    #define N 2

    struct bounded_buffer {
        char data[N];   /* 'items' in this example are just bytes */
        int in;     /* index where producer inserts items, initially 0 */
        int out;    /* index where consumer removes items, initially 0 */
        atomic_int count;  /* number of items currently in buffer, initially 0 */
        struct wait_queue waitq; /* keep track of waiting threads */
    };

    struct bounded_buffer bb;

    void *producer(void *arg) {
        while(true) {
            char item = produce_item();
            if (bb.count == N)
                sleep(&bb.waitq);
            bb.data[bb.in] = item;
            bb.in = (bb.in + 1) % N;
            bb.count++;
            if (bb.count == 1) 
                wakeup(&bb.waitq);
        }
    }

    void *consumer(void *arg) {
        while(true) {
            if (bb.count == 0) 
                sleep(&bb.waitq);
            char item = bb.data[bb.out];
            bb.out = (bb.out + 1) % N;
            bb.count--;
            if (bb.count == N-1) 
                wakeup(&bb.waitq);
            consume_item(item);
        }
    }
:::
:::
:::

Does this solve the problem? Alas, you may have noticed that both the producer and the consumer make decisions based on the value of `count`{.docutils .literal .notranslate}, and even if the `count`{.docutils .literal .notranslate} variable is updated atomically there is still a race condition. A thread, T1, can be interrupted after it has tested the value of `count`{.docutils .literal .notranslate} and decided that it needs call `sleep()`{.docutils .literal .notranslate}, but before the `sleep()`{.docutils .literal .notranslate} has actually executed. If the other thread, T2, calls `wakeup()`{.docutils .literal .notranslate} at this point, it will have no effect since there is not a waiting thread to wake up. When T1 runs again, it will proceed with the `sleep()`{.docutils .literal .notranslate} and can be blocked forever. This is known as the `lost wakeup`{.docutils .literal .notranslate} problem, and is illustrated in [[Fig. 25.6]{.std .std-numref}](#fig-sync-ordering-lost-wakeup){.reference .internal}. In the figure, we show the interleaved thread execution on the left with the actual values of buffer variables substituted into the code statements. On the right, we show the buffer variables as they are updated by the threads.

![[Fig. 25.6 ]{.caption-number}[The lost wakeup problem.]{.caption-text}[\#](#fig-sync-ordering-lost-wakeup "Link to this image"){.headerlink}](../_images/lost_wakeup_short.drawio.png){style="width: 75%;"}

The producer thread has started to add the first item to the buffer, but has not updated the `count`{.docutils .literal .notranslate} before it is preempted. The consumer thread runs, sees that the buffer is empty and decides to sleep, but is preempted before it calls `sleep()`{.docutils .literal .notranslate}. The producer then updates `count`{.docutils .literal .notranslate} and calls `wakeup`{.docutils .literal .notranslate}, which has no effect. When the consumer runs again, it calls `sleep()`{.docutils .literal .notranslate} and blocks awaiting the `wakeup()`{.docutils .literal .notranslate} which has, unfortunately, already happened. Since the consumer is blocked, the producer runs, adds a second item to the buffer, and then generates a third item to add to the buffer. Now, the producer finds that the buffer is full, so it also calls `sleep()`{.docutils .literal .notranslate}, waiting for the consumer to remove something from the buffer and make space for the third item to be added. At this point, we are completely stuck---both threads are sleeping and waiting for the other thread to do something and wake them up. This is called *deadlock*. We will examine the deadlock problem in more detail later.

Before describing synchronization primitives that are described to solve this problem, let's consider some non-solutions.

You might be tempted to think that we can avoid the lost wakeup by simply having the producer and consumer call `wakeup()`{.docutils .literal .notranslate} on *every* iteration after adding or removing an item, rather than only doing so when the buffer becomes non-empty or non-full. That mostly works in this particular instance, where the producer and consumer are both in an infinite loop, and there is enough space in the buffer for the producer to add a second item. It could still leave the consumer waiting longer than it should, while the producer goes about generating another item to add to the buffer. It is also a brittle solution---if we had only a single slot in the buffer (N==1), then the producer would be stuck after adding the first item and losing the first `wakeup()`{.docutils .literal .notranslate} to the consumer would be fatal. Or if the producer stopped after adding a finite number of items, an unlucky consumer could be stranded forever with an item still left in the buffer.

Now, you might observe that testing the value of `count`{.docutils .literal .notranslate} and taking some action based on the result is a critical section of code that should execute atomically, and locks were our solution to critical section problems. So, what if we added a lock to our bounded buffer structure, and had threads acquire the lock before checking `count`{.docutils .literal .notranslate} and either going to sleep or issuing a wake up? This also doesn't work. If we allow a thread to hold the lock when it calls `sleep()`{.docutils .literal .notranslate}, then the other thread will be blocked forever trying to obtain the lock so that it can issue a `wakeup`{.docutils .literal .notranslate}. On the other hand, if we release the lock prior to calling `sleep()`{.docutils .literal .notranslate}, then we right back where we started---a thread could be preempted right after releasing the lock, and before calling `sleep()`{.docutils .literal .notranslate}, once again missing the `wakeup()`{.docutils .literal .notranslate}.
:::

::: {#semaphores .section}
[]{#cont-sync-ordering-sema}

## [25.4.2. ]{.section-number}Semaphores[\#](#semaphores "Link to this heading"){.headerlink}

We can observe that the *lost wakeup* problem occurs because a `wakeup()`{.docutils .literal .notranslate} has no effect when no one is waiting yet. Perhaps we could avoid the problem if we kept track of the `wakeup()`{.docutils .literal .notranslate} and allowed a thread the return immediately from `sleep()`{.docutils .literal .notranslate} if a `wakeup()`{.docutils .literal .notranslate} had already been sent. This is the key idea behind the *semaphore* synchronization primitive introduced by Djikstra [\[[Dij65](../misc/bib.html#id5){.reference .internal}\]]{#id1}. A semaphore has private data consisting of a non-negative integer count and a queue of waiting threads, which can only be accessed by two **atomic operations**, `sem_wait()`{.docutils .literal .notranslate} and `sem_post()`{.docutils .literal .notranslate}. There is also a `sem_init()`{.docutils .literal .notranslate} operation that sets the semaphore count to some initial value.

::: {.admonition .note}
Note

We are using the POSIX names for the semaphore operations. The original names of the semaphore operations used by Djikstra were `P()`{.docutils .literal .notranslate} and `V()`{.docutils .literal .notranslate}. In other literature they are variously called `down`{.docutils .literal .notranslate} and `up`{.docutils .literal .notranslate}, `wait`{.docutils .literal .notranslate} and `signal`{.docutils .literal .notranslate}, `await`{.docutils .literal .notranslate} and `notify`{.docutils .literal .notranslate}, and even `acquire`{.docutils .literal .notranslate} and `release`{.docutils .literal .notranslate}.
:::

The semaphore operations are defined as follows:

-   `sem_init(sem_t *sem, int pshared, unsigned int value)`{.docutils .literal .notranslate} - initializes the semaphore pointed to by sem with the initial value `value`{.docutils .literal .notranslate}. (The pshared argument should be 0 for semaphores shared by threads in the same process.)

-   `sem_wait(sem_t *sem)`{.docutils .literal .notranslate} - decrements the internal count of the semaphore pointed to by `sem`{.docutils .literal .notranslate}. If the semaphore's value is greater than zero, then the decrement proceeds, and the function returns, immediately. If the semaphore currently has the value zero, then the call blocks until it becomes possible to perform the decrement (i.e., the semaphore value rises above zero).

-   `sem_post(sem_t *sem)`{.docutils .literal .notranslate} - increments the internal count of the semaphore pointed to by `sem`{.docutils .literal .notranslate}. If the semaphore's value consequently becomes greater than zero, then another process or thread blocked in a `sem_wait()`{.docutils .literal .notranslate} call will be woken up.

It is important that the `sem_wait()`{.docutils .literal .notranslate} and `sem_post()`{.docutils .literal .notranslate} calls are atomic, meaning that once a thread starts one of these operations, it cannot be interleaved with the execution of another operation on the same semaphore. For user-level implementations, this generally requires a system call since we may need to change the state of a thread from running to blocked, or from blocked to runnable. In the operating system, we need to ensure that checking the semaphore count and putting a thread to sleep is atomic, either by disabling interrupts on a uniprocessor, or by using a spinlock on a multiprocessor. Once the thread has been enqueued on the semaphore's wait list, the lock can be released before yielding the CPU to another thread.

How does the semaphore synchronization primitive help us solve the bounded buffer problem? Instead of a single count of items in the buffer, we start by breaking apart the conditions that producers and consumers must wait upon. The producer thread can proceed as long as there are empty slots in the buffer to put items into. We can represent this using a semaphore called `sem_empty`{.docutils .literal .notranslate} with initial value N. The consumer can proceed as long as there are filled slots in the buffer to remove items from. We can represent this using a semaphore called `sem_filled`{.docutils .literal .notranslate}. Prior to adding an item, the producer must perform a `sem_wait(&sem_empty)`{.docutils .literal .notranslate}, which will decrement the semaphore's count and return immediately as long as there is space in the buffer. Once the semaphore's value is 0, the producer will block awaiting a `sem_post(&sem_empty)`{.docutils .literal .notranslate} from the consumer to indicate that an item has been removed an an empty slot is now available. Each time an item is added to the buffer, the producer must issue a `sem_post(&sem_filled)`{.docutils .literal .notranslate} to let the consumer know that a slot has been filled and an item is ready to be removed from the buffer. The code for a single producer and consumer using semaphores is shown in [[Listing 25.24]{.std .std-numref}](#listing-sync-ordering-bbuf-sem){.reference .internal}.

::: {#listing-sync-ordering-bbuf-sem .literal-block-wrapper .docutils .container}
::: code-block-caption
[Listing 25.24 ]{.caption-number}[Bounded buffer with semaphores]{.caption-text}[\#](#listing-sync-ordering-bbuf-sem "Link to this code"){.headerlink}
:::

::: {.highlight-default .notranslate}
::: highlight
     1/* For illustration purposes only. 
     2 * This code is not complete and cannot be compiled into an executable.
     3 */
     4#include <semaphore.h>
     5#include <stdbool.h>
     6
     7extern char produce_item();
     8extern void consume_item(char item);
     9
    10#define N 2
    11
    12struct bounded_buffer {
    13    char data[N];   /* 'items' in this example are just bytes */
    14    int in;     /* index where producer inserts items, initially 0 */
    15    int out;    /* index where consumer removes items, initially 0 */
    16    sem_t sem_empty;
    17    sem_t sem_filled;
    18};
    19
    20struct bounded_buffer bb;
    21
    22void *producer(void *arg) {
    23    while(true) {
    24        char item = produce_item();
    25        sem_wait(&bb.sem_empty);
    26        bb.data[bb.in] = item;
    27        bb.in = (bb.in + 1) % N;
    28        sem_post(&bb.sem_filled);
    29    }
    30}
    31
    32void *consumer(void *arg) {
    33    while(true) {
    34        sem_wait(&bb.sem_filled);
    35        char item = bb.data[bb.out];
    36        bb.out = (bb.out + 1) % N;
    37        sem_post(&bb.sem_empty);
    38        consume_item(item);
    39    }
    40}
    41
    42int main()
    43{
    44    sem_init(&bb.sem_empty, 0, N);
    45    sem_init(&bb.sem_filled,0, 0);
    46    
    47    /*** Thread creation stuff here ***/
    48    
    49    return 0;
    50}
:::
:::
:::

As you can see, the code is simplified by the semaphore primitives. The producer waits for a slot in the buffer to be available, add the new item, and then posts a notice that a slot has been filled. The consumer waits for a slot to be filled, takes an item out of the buffer, and posts a notice that an empty slot is now available. Because the semaphores are internally keeping track of the number of empty and filled slots in the buffer, we have removed the `count`{.docutils .literal .notranslate} from the buffer data structure.

The `sem_empty`{.docutils .literal .notranslate} and `sem_filled`{.docutils .literal .notranslate} variables are examples of *counting semaphores* (also called *general semaphores*), where the semaphore value can be any non-negative integer. We also see a common semaphore usage pattern here, where the `sem_wait()`{.docutils .literal .notranslate} is performed by one thread, and the `sem_post()`{.docutils .literal .notranslate} is performed by a different thread. It is also possible to create a *binary* semaphore, where the semaphore value should only be 0 or 1, and use it for mutual exclusion. For example, suppose we wanted to solve a more general producer/consumer problem where we have multiple producer threads and multiple consumer threads. Now, we also need to coordinate among the producers, so that they each insert to a different buffer slot, and among the consumers so that they each remove an item from a different slot. We can add another semaphore, `sem_mutex`{.docutils .literal .notranslate}, with initial value 1, and use it to protect access to the other members of the bounded buffer. Example code is showin in [[Listing 25.25]{.std .std-numref}](#listing-sync-ordering-bbuf-sem-multi){.reference .internal}.

::: {#listing-sync-ordering-bbuf-sem-multi .literal-block-wrapper .docutils .container}
::: code-block-caption
[Listing 25.25 ]{.caption-number}[Bounded buffer with semaphores for multiple producers and consumers.]{.caption-text}[\#](#listing-sync-ordering-bbuf-sem-multi "Link to this code"){.headerlink}
:::

::: {.highlight-default .notranslate}
::: highlight
    /* For illustration purposes only. 
     * This code is not complete and cannot be compiled into an executable.
     */
    #include <semaphore.h>
    #include <stdbool.h>

    extern char produce_item();
    extern void consume_item(char item);

    #define N 2

    struct bounded_buffer {
        char data[N];   /* 'items' in this example are just bytes */
        int in;     /* index where producer inserts items, initially 0 */
        int out;    /* index where consumer removes items, initially 0 */
        sem_t sem_empty;
        sem_t sem_filled;
        sem_t sem_mutex;
    };

    struct bounded_buffer bb;

    void *producer(void *arg) {
        while(true) {
            char item = produce_item();
            sem_wait(&bb.sem_empty);
            sem_wait(&bb.sem_mutex);
            bb.data[bb.in] = item;
            bb.in = (bb.in + 1) % N;
            sem_post(&bb.sem_mutex);
            sem_post(&bb.sem_filled);
        }
    }

    void *consumer(void *arg) {
        while(true) {
            sem_wait(&bb.sem_filled);
            sem_wait(&bb.sem_mutex);
            char item = bb.data[bb.out];
            bb.out = (bb.out + 1) % N;
            sem_post(&bb.sem_mutex);
            sem_post(&bb.sem_empty);
            consume_item(item);
        }
    }

    int main()
    {
        sem_init(&bb.sem_empty, 0, N);
        sem_init(&bb.sem_filled, 0, 0);
        sem_init(&bb.sem_mutex, 0, 1);
        
        /*** Thread creation stuff here ***/
        
        return 0;
    }
:::
:::
:::

The `sem_mutex`{.docutils .literal .notranslate} is used exactly like a lock to protect the `in`{.docutils .literal .notranslate} and `out`{.docutils .literal .notranslate} shared variables that are used by producers and consumers when accessing slots in the buffer. Is it better to use a binary semaphore or a lock in such cases? There really is no functional difference---both provide mutual exclusion. However, there is a semantic difference. Logically, a lock is "held" by the thread that has successfully completed the most recent `acquire()`{.docutils .literal .notranslate} and should only be `release()`{.docutils .literal .notranslate}d by the thread that holds it. Some lock implementations will track lock ownership and enforce this rule, raising an error if a lock is incorrectly released by a thread that did not acquire it first. These errors can be an invaluable debugging tool, which are not available if you use semaphores for mutual exclusion.
:::

::: {#condition-variables .section}
[]{#cont-sync-ordering-cv}

## [25.4.3. ]{.section-number}Condition Variables[\#](#condition-variables "Link to this heading"){.headerlink}

One challenge with using semaphores is that we must encode the state that a thread is waiting upon as a single counter. This worked nicely for the bounded buffer problem with producers using a semaphore to count the number of empty slots, and consumers using another semaphore to count the number of filled slots. For example, suppose we had two types of producer threads, one that produced 'a's and another that produced 'b's, and we wanted to ensure that the buffer was never more than 75% full of either a's or b's. The 'a'-producer would need a check something like the code shown below before it could add another 'a' to the buffer (and similarly for the 'b'-producer).

::: {.highlight-c .notranslate}
::: highlight
    1...
    2if ( (a_count + b_count) == N || (a_count >= N*3/4) )
    3    sleep()
    4...
:::
:::

Expressing this set of conditions using semaphores is tricky (although it can be done), and it is easy to make mistakes. Instead, we would like to separate the checking of the conditions from the act of atomically putting a thread to sleep. However, we saw earlier that we need to hold a lock while testing the shared variables that are involved in deciding whether to sleep or not, and we need to release the lock before we put the thread to sleep. To solve that problem we introduce another synchronization primitive called a *condition variable*. This is, admittedly, a terrible name since the boolean condition that a thread checks is not actually part of the *condition variable* object at all. A condition variable consists of an internal list of waiting threads, and operations `wait`{.docutils .literal .notranslate}, `signal`{.docutils .literal .notranslate} and `broadcast`{.docutils .literal .notranslate}. For concreteness, we will use the POSIX pthread names for the condition variable type, `pthread_cond_t`{.docutils .literal .notranslate}, and operations, `pthread_cond_wait`{.docutils .literal .notranslate}, `pthread_cond_signal`{.docutils .literal .notranslate} and `pthread_cond_broadcast`{.docutils .literal .notranslate}.

-   `pthread_cond_wait(pthread_cond_t *cond, pthread_mutex_t *mutex)`{.docutils .literal .notranslate} : atomically release the `mutex`{.docutils .literal .notranslate} and put the calling thread to sleep on the condition variable `cond`{.docutils .literal .notranslate}; upon waking up, the `mutex`{.docutils .literal .notranslate} is re-acquired before returning. Must be called with `mutex`{.docutils .literal .notranslate} held by the calling thread.

-   `pthread_cond_signal(pthread_cond_t *cond)`{.docutils .literal .notranslate} : Wake up one thread waiting on condition variable `cond`{.docutils .literal .notranslate}. Has no effect if no threads are waiting.

-   `pthread_cond_broadcast(pthread_cond_t *cond)`{.docutils .literal .notranslate} : Wake up all threads waiting on condition variable `cond`{.docutils .literal .notranslate}. Has no effect if no threads are waiting.

Note that locks and condition variables must always be used together. The lock protects the shared data, so that a thread can examine the state of a structure, make decisions about what to do next, and modify the shared data without interference from other threads. The condition variable provides the mechanism to atomically release the lock and put a thread to sleep until it becomes possible for that thread to make progress again. Upon return from a `pthread_cond_wait()`{.docutils .literal .notranslate}, a thread is guaranteed to hold the lock again. However, there is no guarantee that a thread awakened by a `pthread_cond_signal()`{.docutils .literal .notranslate} will be the next thread to acquire the lock---other threads could run first, acquire the lock, change shared variables and invalidate the condition that the thread was waiting for. Hence, a thread should always re-evaluate the boolean expression after returning from `pthread_cond_wait()`{.docutils .literal .notranslate} to make sure it is ok to proceed. In some cases, a thread may need to wait repeatedly.

To illustrate these concepts, let's look first at how we would implement a solution to our original bounded buffer problem using a lock together with condition variables.

::: {#listing-sync-ordering-bbuf-cv .literal-block-wrapper .docutils .container}
::: code-block-caption
[Listing 25.26 ]{.caption-number}[Bounded buffer with condition variables for multiple producers and consumers.]{.caption-text}[\#](#listing-sync-ordering-bbuf-cv "Link to this code"){.headerlink}
:::

::: {.highlight-default .notranslate}
::: highlight
     1/* For illustration purposes only. 
     2 * This code is not complete and cannot be compiled into an executable.
     3 */
     4#include <pthread.h>
     5#include <stdbool.h>
     6
     7extern char produce_item();
     8extern void consume_item(char item);
     9
    10#define N 2
    11
    12struct bounded_buffer {
    13    char data[N];   /* 'items' in this example are just bytes */
    14    int in;     /* index where producer inserts items, initially 0 */
    15    int out;    /* index where consumer removes items, initially 0 */
    16    int count;
    17    pthread_mutex_t buflock;
    18    pthread_cond_t not_full;
    19    pthread_cond_t not_empty;
    20};
    21
    22struct bounded_buffer bb;
    23
    24void *producer(void *arg) {
    25    while(true) {
    26        char item = produce_item();
    27        pthread_mutex_lock(&bb.buflock);
    28        while(bb.count == N) {
    29            pthread_cond_wait(&bb.notfull, &bb.buflock);
    30        }
    31        bb.data[bb.in] = item;
    32        bb.in = (bb.in + 1) % N;
    33        bb.count++;
    34        pthread_cond_signal(&bb.notempty);
    35        pthread_mutex_unlock(&bb.buflock);
    36    }
    37}
    38
    39void *consumer(void *arg) {
    40    while(true) {
    41        pthread_mutex_lock(&bb.buflock);
    42        while (bb.count == 0) {
    43            pthread_cond_wait(&bb.notempty, &bb.buflock);
    44        }
    45        char item = bb.data[bb.out];
    46        bb.out = (bb.out + 1) % N;
    47        bb.count--;
    48        pthread_cond_signal(&bb.notfull);
    49        pthread_mutex_unlock(&bb.buflock);
    50
    51        consume_item(item);
    52    }
    53}
    54
    55int main()
    56{
    57    pthread_mutex_init(&bb.buflock, NULL);
    58    pthread_cond_init(&bb.notfull, NULL);
    59    pthread_cond_init(&bb.notempty, NULL);
    60    
    61    /*** Thread creation stuff here ***/
    62    
    63    return 0;
    64}
:::
:::
:::

Once the producer has created an item to add to the buffer, it first locks the buffer (line 27), then checks if there is space to insert a new item (line 28). If the buffer is full, the producer calls `pthread_cond_wait()`{.docutils .literal .notranslate} to put itself to sleep until the buffer becomes not full (line 29). Upon returning from the wait, the producer re-checks to make sure there is still space in the buffer, and if so, it can proceed to insert it (lines 31-33). Finally, the producer notifies a waiting consumer (if there is one) that the buffer is not empty (line 34) and releases the buffer lock (line 35). The consumer goes through a similar set of steps.

Notice that we use a `while()`{.docutils .literal .notranslate} loop on lines 28 and 42 to check the number of items in the buffer. This is necessary because the buffer lock is released while waiting, and not immediately re-acquired after a signal is sent. *A set of pictures should go here to illustrate the reason.* Suppose we have a full buffer, and two producer threads that want to add an item. Producer [\\(p1\\)]{.math .notranslate .nohighlight} executes lines 26 to 29 and is blocked on the *notfull* condition variable, releasing the lock. While [\\(p1\\)]{.math .notranslate .nohighlight} held the lock, consumer [\\(c1\\)]{.math .notranslate .nohighlight} and producer [\\(p2\\)]{.math .notranslate .nohighlight} also tried to acquire the lock and are queued up waiting for it to be released; when [\\(p1\\)]{.math .notranslate .nohighlight} releases the lock in its call to `pthread_cond_wait()`{.docutils .literal .notranslate}, [\\(c1\\)]{.math .notranslate .nohighlight} will acquire it next. Consumer [\\(c1\\)]{.math .notranslate .nohighlight} executes lines 42-47 to check that the buffer is not empty and remove an item, then signals the *notfull* condition variable since there is now an empty slot in the buffer. The `pthread_cond_signal()`{.docutils .literal .notranslate} operation makes [\\(p1\\)]{.math .notranslate .nohighlight} runnable again, but [\\(p1\\)]{.math .notranslate .nohighlight} must acquire the lock before it can return. When [\\(c1\\)]{.math .notranslate .nohighlight} releases the lock on line 49, it is possible for [\\(p2\\)]{.math .notranslate .nohighlight} to acquire it before [\\(p1\\)]{.math .notranslate .nohighlight}, and fill the only available slot in the buffer. When [\\(p2\\)]{.math .notranslate .nohighlight} releases the lock and [\\(p1\\)]{.math .notranslate .nohighlight} acquires it, returning from the wait on line 29, the buffer will be full again. If [\\(p1\\)]{.math .notranslate .nohighlight} did not re-check the state of the buffer on line 28 (i.e., if we used an `if`{.docutils .literal .notranslate} statement on line 28 instead of a `while`{.docutils .literal .notranslate} statement), then [\\(p1\\)]{.math .notranslate .nohighlight} would proceed to insert its item into the buffer, overwriting an existing item that had not yet been removed by a consumer.

**Exercise for the reader**

Try writing the code for the a/b-producer problem, using a lock and one or more condition variable to enforce the restriction that the buffer cannot be more than 75% full of either 'a's or 'b's. If you use a single condition variable, then when a consumer thread removes an item it can use `pthread_cond_broadcast()`{.docutils .literal .notranslate} to wake up all waiters (only one will actually be able to use the slot that the consumer made available, the others will have to go back to sleep). If you separate a-producers and b-producers by having them wait on different condition variables, the consumer will have to decide which condition variable to signal (can the slot that the consumer made available be used only by an a-producer, a b-producer, or either?).
:::
:::

::: prev-next-area
[](locks.html "previous page"){.left-prev}

::: prev-next-info
previous

[25.3. ]{.section-number}Implementing Locks
:::

[](concurrency_bugs.html "next page"){.right-next}

::: prev-next-info
next

[26. ]{.section-number}Common Concurrency Bugs
:::
:::
:::

::: {.bd-sidebar-secondary .bd-toc}
::: {.sidebar-secondary-items .sidebar-secondary__inner}
::: sidebar-secondary-item
::: {.page-toc .tocsection .onthispage}
Contents
:::

-   [25.4.1. The Bounded Buffer Problem](#the-bounded-buffer-problem){.reference .internal .nav-link}
-   [25.4.2. Semaphores](#semaphores){.reference .internal .nav-link}
-   [25.4.3. Condition Variables](#condition-variables){.reference .internal .nav-link}
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
