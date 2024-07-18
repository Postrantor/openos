---
docsearch:language: en
lang: en
title: 26. Common Concurrency Bugs --- Introduction to Operating Systems
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

- [24. Introduction](sync.html){.reference .internal}
- [25. Basic Synchronization](basic.html){.reference .internal}
  []{.toctree-toggle role="presentation"}
  - [25.1. Cooperating Processes and Inter-process Communication](sharing.html){.reference .internal}
  - [25.2. The Critical Section Problem](criticalsection.html){.reference .internal}
  - [25.3. Implementing Locks](locks.html){.reference .internal}
  - [25.4. Ordering Thread Events](ordering.html){.reference .internal}
- [26. Common Concurrency Bugs](#){.current .reference .internal}
- [27. Advanced Synchronization](advanced.html){.reference .internal}
  []{.toctree-toggle role="presentation"}
  - [27.1. Read-Dominated Workloads](readmostly.html){.reference .internal}
  - [27.2. Challenges of Modern Hardware](hardware_challenges.html){.reference .internal}
  - [27.3. Locking in the Linux Kernel](linux_locking.html){.reference .internal}
- [28. Review](review.html){.reference .internal}

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

- [[ ![JupyterHub logo](../_static/images/logo_jupyterhub.svg) ]{.btn__icon-container} [JupyterHub]{.btn__text-container}](https://jupyterhub-opf-jupyterhub.apps.smaug.na.operate-first.cloud/hub/user-redirect/git-pull?repo=https%3A//github.com/OpenOSOrg/openos&urlpath=lab/tree/openos/content/sync/concurrency_bugs.ipynb&branch=main "Launch on JupyterHub"){.btn .btn-sm .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
  :::

::: {.dropdown .dropdown-source-buttons}

- [[ ]{.btn__icon-container} [Repository]{.btn__text-container}](https://github.com/OpenOSOrg/openos "Source repository"){.btn .btn-sm .btn-source-repository-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
- [[ ]{.btn__icon-container} [Suggest edit]{.btn__text-container}](https://github.com/OpenOSOrg/openos/edit/main/content/sync/concurrency_bugs.ipynb "Suggest edit"){.btn .btn-sm .btn-source-edit-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
- [[ ]{.btn__icon-container} [Open issue]{.btn__text-container}](https://github.com/OpenOSOrg/openos/issues/new?title=Issue%20on%20page%20%2Fsync/concurrency_bugs.html&body=Your%20issue%20content%20here. "Open an issue"){.btn .btn-sm .btn-source-issues-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
  :::

::: {.dropdown .dropdown-download-buttons}

- [[ ]{.btn__icon-container} [.ipynb]{.btn__text-container}](../_sources/sync/concurrency_bugs.ipynb "Download source file"){.btn .btn-sm .btn-download-source-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}

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

# Common Concurrency Bugs

::: {#print-main-content}
::: {#jb-print-toc}

<div>

## Contents

</div>

- [26.1. Atomicity Violations](#atomicity-violations){.reference .internal .nav-link}
- [26.2. Order Violations](#order-violations){.reference .internal .nav-link}
- [26.3. Deadlocks](#deadlocks){.reference .internal .nav-link}
  - [26.3.1. What is a resource?](#what-is-a-resource){.reference .internal .nav-link}
  - [26.3.2. Visualizing and Modeling Deadlocks](#visualizing-and-modeling-deadlocks){.reference .internal .nav-link}
  - [26.3.3. The Four Conditions for Deadlock](#the-four-conditions-for-deadlock){.reference .internal .nav-link}
  - [26.3.4. Breaking Mutual Exclusion](#breaking-mutual-exclusion){.reference .internal .nav-link}
  - [26.3.5. Breaking Hold-and-Wait](#breaking-hold-and-wait){.reference .internal .nav-link}
  - [26.3.6. Allowing Preemption (breaking the no preemption condition)](#allowing-preemption-breaking-the-no-preemption-condition){.reference .internal .nav-link}
  - [26.3.7. Breaking Circular Wait](#breaking-circular-wait){.reference .internal .nav-link}
  - [26.3.8. Reality Check](#reality-check){.reference .internal .nav-link}
- [26.4. Livelock, Starvation and Other Bugs](#livelock-starvation-and-other-bugs){.reference .internal .nav-link}
  :::
  :::
  :::

::: {#searchbox}
:::

::: {.cell .tag_remove-input .docutils .container}
:::

::: {#common-concurrency-bugs .section .tex2jax_ignore .mathjax_ignore}
[]{#cont-sync-concurrency-bugs}

# [26. ] {.section-number}Common Concurrency Bugs[\#](#common-concurrency-bugs "Link to this heading") {.headerlink}

In the previous chapters, we have already seen some examples of how things can go wrong without correct synchronization. In this chapter, we examine the three most common types of concurrency bugs: *atomicity violations*, *order violations*, and *deadlocks*. We will also briefly discuss other, less common, concurrency bugs. We will focus on deadlocks, since we have already seen the tools needed to address the other two main types of bugs.

Our bug classifications, and real-world examples, are drawn from Lu et al.'s 2008 study of concurrency bugs [\[[LPSZ08](../misc/bib.html#id10 "Shan Lu, Soyeon Park, Eunsoo Seo, and Yuanyuan Zhou. Learning from mistakes: a comprehensive study on real world concurrency bug characteristics. In Proceedings of the 13th International Conference on Architectural Support for Programming Languages and Operating Systems, ASPLOS XIII, 329–339. New York, NY, USA, 2008. Association for Computing Machinery. URL: https://doi.org/10.1145/1346281.1346323, doi:10.1145/1346281.1346323."){.reference .internal}\]]{#id1}, which examined 105 randomly selected concurrency bugs drawn from the bug databases of four open-source applications (MySQL, Apache, Mozilla, and OpenOffice). In [[Table 26.1]{.std .std-numref}](#table-sync-bugs-breakdown){.reference .internal}, we break down these bugs by category.

::: pst-scrollable-table-container
Bug Category          Bug Count

---

Deadlock              31
Atomicity Violation   51
Order Violation       24
Other                 2

: [Table 26.1 ]{.caption-number}[Concurrency Bug Breakdown (3 bugs are counted as both atomicity violation and order violation)]{.caption-text}[\#](#table-sync-bugs-breakdown "Link to this table"){.headerlink}
:::

One key takeaway from this study is that concurrent programming is *hard*---even mature, widely used projects have concurrency bugs. Developing tools to help detect, diagnose, and correct these concurrency bugs is an active area of research, but so far, there is no silver bullet.

::: {#atomicity-violations .section}

## [26.1. ] {.section-number}Atomicity Violations[\#](#atomicity-violations "Link to this heading") {.headerlink}

> <div>
>
> The desired serializability among multiple memory accesses is violated (i.e., a code region is intended to be atomic, but the atomicity is not enforced during execution).[\[[LPSZ08](../misc/bib.html#id10 "Shan Lu, Soyeon Park, Eunsoo Seo, and Yuanyuan Zhou. Learning from mistakes: a comprehensive study on real world concurrency bug characteristics. In Proceedings of the 13th International Conference on Architectural Support for Programming Languages and Operating Systems, ASPLOS XIII, 329–339. New York, NY, USA, 2008. Association for Computing Machinery. URL: https://doi.org/10.1145/1346281.1346323, doi:10.1145/1346281.1346323."){.reference .internal}\]]{#id2}
>
> </div>

Atomicity violations are related to data races, but they are not the same. A data race occurs when two or more threads have conflicting accesses to a shared variable without any synchronization, but in some cases this may be the programmer's intent (not a bug). For example, we used a flag variable in [[Listing 25.22]{.std .std-numref}](locks.html#listing-sync-check-spinlock-fairness){.reference .internal} to force the child threads to wait until the parent had finished creating all the threads. An atomicity violation occurs when some section of code needs to be atomic for correctness, but there is no synchronzation to ensure atomicity. In [[Fig. 26.1]{.std .std-numref}](#fig-sync-bugs-mysql-atomicity-violation){.reference .internal} we show a real-world example of an atomicity violation bug found in one version of MySQL. Here, the atomicity violation bug is also a data race, since the conflicting accesses to `thd->proc_info`{.docutils .literal .notranslate} are not separated by any synchronization. Programmers often mistakenly believe that short code sequences can't be interrupted or interleaved, leading to atomicity violation bugs like the MySQL example. The solution is simple: introduce a lock to protect the `proc_info`{.docutils .literal .notranslate} and ensure the lock is acquired prior to checking if `thd->proc_info`{.docutils .literal .notranslate} is NULL, and released only after Thread 1 is done using `thd->proc_info`{.docutils .literal .notranslate}. (Thread 2 should also hold the lock when setting `thd->proc_info`{.docutils .literal .notranslate} to NULL.)

![[Fig. 26.1 ]{.caption-number}[Example of an atomicity violation bug from MySQL.]{.caption-text}[\#](#fig-sync-bugs-mysql-atomicity-violation "Link to this image"){.headerlink}](../_images/mysql_atomicity_violation.drawio.png){style="width: 75%;"}

We can also find atomicity violation bugs in data-race-free programs. For example, consider the attempt to add locking to the bank account deposit example from [[Listing 25.2]{.std .std-numref}](sharing.html#listing-sync-bank){.reference .internal}, as shown in [[Fig. 26.2]{.std .std-numref}](#fig-sync-bugs-bank-deposit-atomicity-violation){.reference .internal}(a). Here, the programmer has ensured that all accesses to the shared data in the bank account are protected by a lock variable, however, they have not enforced the required atomicity. Because the lock is released after reading the old balance from the account, and re-acquired before writing the new balance, two threads can still interleave in a way that causes one of the deposits to be lost.

![[Fig. 26.2 ]{.caption-number}[Atomicity violation bug and its fix in a data-race-free implementation of the bank deposit function.]{.caption-text}[\#](#fig-sync-bugs-bank-deposit-atomicity-violation "Link to this image"){.headerlink}](../_images/bank_deposit_atomicity_violation.drawio.png){style="width: 75%;"}

When writing concurrent code, always think adversarially. Is your code guaranteed to execute correctly even if the scheduler switches between threads at the worst possible moment? Consider what operations *must* execute without interference---these sequences of instructions must have mutual exclusion enforced.
:::

::: {#order-violations .section}

## [26.2. ] {.section-number}Order Violations[\#](#order-violations "Link to this heading") {.headerlink}

> <div>
>
> The desired order between two (groups of) memory accesses is flipped (i.e., A should always be executed before B, but the order is not enforced during execution).[\[[LPSZ08](../misc/bib.html#id10 "Shan Lu, Soyeon Park, Eunsoo Seo, and Yuanyuan Zhou. Learning from mistakes: a comprehensive study on real world concurrency bug characteristics. In Proceedings of the 13th International Conference on Architectural Support for Programming Languages and Operating Systems, ASPLOS XIII, 329–339. New York, NY, USA, 2008. Association for Computing Machinery. URL: https://doi.org/10.1145/1346281.1346323, doi:10.1145/1346281.1346323."){.reference .internal}\]]{#id3}
>
> </div>

The producer / consumer bounded buffer problem demonstrated the need to enforce ordering between operations in different threads. However, programmers sometimes assume that operations in different threads must be ordered in some way without actually enforcing that order. This may occur because of assumptions about the relative speed at which threads are executing (e.g., if T1 has to perform a more complex calculation than T2, a programmer might assume that T2 will finish first). These assumptions are unsafe because a thread's progress depends on many external factors, including how much time the scheduler gives it to run on a CPU and how many cache misses or page faults occur while it is running.

![[Fig. 26.3 ]{.caption-number}[Ordering violation bug in Mozilla.]{.caption-text}[\#](#fig-sync-bugs-mozilla-ordering-violation "Link to this image"){.headerlink}](../_images/mozilla_ordering_violation.drawio.png){style="width: 75%;"}

A real-world example of an order violation bug comes from Mozilla, and is illustrated in [[Fig. 26.3]{.std .std-numref}](#fig-sync-bugs-mozilla-ordering-violation){.reference .internal}. In this example, Thread 1 is responsible for initialization and creation of other threads. Thread 2 is one of the threads created by Thread 1, and the programmers assumed that Thread 2 would have to run after Thread 1. Unfortunately, Thread 2 becomes runnable as soon as it is created, and may execute before Thread 1 assigns a value to the variable `mThread`{.docutils .literal .notranslate}. In the best case scenario, `mThread`{.docutils .literal .notranslate} will be NULL prior to the assignment in Thread 1, and Thread 2 will crash when it attempts to dereference `mThread->mState`{.docutils .literal .notranslate}. Why is this the best case? Because if `mThread`{.docutils .literal .notranslate} is non-NULL but not correctly initialized yet, then Thread 2 will set its `mState`{.docutils .literal .notranslate} from a random memory location and could continue to execute in unexpected ways for a long time without actually crashing. Crash failures are *much* easier to detect and debug than arbitrary incorrect behavior.

The fix for this bug is simply to enforce some ordering, so that Thread 2 has to wait until the initialization is complete. A semaphore with initial value 0 would work well for this purpose. Thread 2 issues a `sem_wait()`{.docutils .literal .notranslate} prior to accessing `mThread`{.docutils .literal .notranslate}, and Thread 1 issues a `sem_post()`{.docutils .literal .notranslate} when it is safe to use `mThread`{.docutils .literal .notranslate}.
:::

::: {#deadlocks .section}

## [26.3. ] {.section-number}Deadlocks[\#](#deadlocks "Link to this heading") {.headerlink}

> <div>
>
> A situation, typically one involving opposing parties, in which no progress can be made. (Oxford Languages definition)
>
> </div>

> <div>
>
> A state in which each actor in a system is waiting on another actor to take action. (Computer systems definition)
>
> </div>

An informal notion of *deadlock* is likely already familiar to you. Examples outside of computer systems include this amazing law passed by the Kansas State Legislature in the early 20th century:

> <div>
>
> When two trains approach each other at a crossing, both shall come to a full stop and neither shall start upon again until the other has gone.
>
> </div>

![[Fig. 26.4 ]{.caption-number}[Two trains approaching each other at a crossing.]{.caption-text}[\#](#fig-sync-bugs-train-deadlock "Link to this image"){.headerlink}](../_images/trains-from-slides.png){style="width: 50%;"}

Another real-world example of deadlock comes from the [Massachusetts Driver's Manual, Chapter 4, Rules of the Road](https://www.mass.gov/doc/drivers-manual/download){.reference .external}:

> <div>
>
> **Four-Way Stop**
>
> At an intersection with stop signs in all directions, you must yield the right-of-way to...
>
> - Another vehicle that has already come to a full stop
> - A vehicle directly to your right that has stopped at the same time as you
>
> </div>

![[Fig. 26.5 ]{.caption-number}[Deadlock at a four-way stop caused by strictly following the rules of the road.]{.caption-text}[\#](#fig-sync-bugs-four-way-stop "Link to this image"){.headerlink}](../_images/four-way-stop.drawio.png){style="width: 25%;"}

As illustrated in [[Fig. 26.5]{.std .std-numref}](#fig-sync-bugs-four-way-stop){.reference .internal}, strictly following the rules of the road would result in a deadlock if four cars arrived at a four-way stop at exactly the same time. Each driver is required to yield to the vehicle on their right, so no driver is actually permitted to proceed through the intersection.

Since this is an operating systems book, our focus is on deadlocks that arise in the concurrent execution of computer programs. We will use the term `thread`{.docutils .literal .notranslate} to refer to the concurrent execution contexts, although the same issues arise when processes share resources.

::: {#what-is-a-resource .section}

### [26.3.1. ] {.section-number}What is a resource?[\#](#what-is-a-resource "Link to this heading") {.headerlink}

In discussing deadlocks, we often talk about *resources* that are shared by multiple threads or processes in a computer system. In general, a resource is any object that is needed by a thread to do its work. Some resources may be physical objects, like a printer or a network card, while others are logical objects, like a counter variable, a scheduler queue, or a data structure representing a bank account record in a database. In fact, even the physical resources will be represented and managed by the computer system using some data structure. And, when we have a shared data object, we usually need to associate a lock with it to protect against unwanted interference. So, when we talk about resource deadlocks, we are often talking about the lock that protects that resource from concurrent access. When we say that a thread (or process) has been allocated (equivalently, assigned or granted) a resource, we often mean that the thread has acquired the lock protecting that resource, and is now permitted to use the resource.

We often find situations where threads need to acquire multiple resources protected by different locks. For example, consider the problem of transferring funds from one bank account to another. We want the entire transfer to happen atomically---either the funds are in the source account, meaning the transfer hasn't happened yet, or the funds are in the destination account, meaning the transfer has been completed. If we had a single lock for the entire bank database, then all we need to do is acquire that lock, debit the source account and credit the destination account before releasing the lock. But since most operations access a single account (e.g., deposit, withdraw, read balance, etc.), this would give terrible performance to the bank customers. We really want to have a lock associated with each account, so that independent operations on different accounts can happen concurrently. Now the transfer operation needs to acquire locks for both the source and destination accounts and hold them until the balances of both accounts have been updated. Sample code for this setup is shown in [[Listing 26.1]{.std .std-numref}](#listing-sync-bugs-transfer){.reference .internal}: we have a structure for each account which includes the account balance and a lock, and the transfer function must acquire the locks on both accounts before it updates the balances. As we will see, situations like this can easily lead to deadlocks.

::: {#listing-sync-bugs-transfer .literal-block-wrapper .docutils .container}
::: code-block-caption
[Listing 26.1 ]{.caption-number}[Simple bank transfer, requiring locks on two accounts]{.caption-text}[\#](#listing-sync-bugs-transfer "Link to this code"){.headerlink}
:::

::: {.highlight-c .notranslate}
::: highlight
1typedef struct account_s {
2    int acct_num;
3    money_t balance;
4    pthread_mutex_lock acct_lock;
5} account_t;
6
7void transfer(account_t *src_acct, account_t *dest_acct, money_t amount)
8{
9    pthread_mutex_lock(&src_acct->acct_lock);
10    pthread_mutex_lock(&dest_acct->acct_lock);
11
12    src_acct->balance -= amount;
13    dest_acct->balance += amount;
14
15    pthread_mutex_unlock(&dest_acct->acct_lock);
16    pthread_mutex_unlock(&src_acct->acct_lock);
17}
:::
:::
:::
:::

::: {#visualizing-and-modeling-deadlocks .section}

### [26.3.2. ] {.section-number}Visualizing and Modeling Deadlocks[\#](#visualizing-and-modeling-deadlocks "Link to this heading") {.headerlink}

To visualize resource deadlocks, we adopt the directed bipartite graph model introduced by Holt [\[[Hol72](../misc/bib.html#id12 "Richard C. Holt. Some deadlock properties of computer systems. ACM Comput. Surv., 4(3):179–196, sep 1972. URL: https://doi.org/10.1145/356603.356607, doi:10.1145/356603.356607."){.reference .internal}\]]{#id4}, in which threads and resources are represented by nodes, resource allocations are represented by a directed edge from the resource node to the thread node that has been granted exclusive use of that resource, and resource requests are represented by a directed edge from a thread node to the resource node that it is requesting. (We will only deal with the case where there is a single instance of each type of resource.) When drawing such a resource graph, we depict thread nodes using circles, and resource nodes using squares.

[[Fig. 26.6]{.std .std-numref}](#fig-sync-bugs-resource-graph){.reference .internal} shows an example resource allocation graph with two threads and two resources. Resource R1 has been allocated to thread T1, and resource R2 has been allocated to thread T2. Thread T1 has made a request for R2 (which cannot be granted until T2 releases it), and T2 has made a request for R1 (which cannot be granted until T1 releases it). These threads are deadlocked.

![[Fig. 26.6 ]{.caption-number}[Example of a resource allocation graph with a cycle, showing two threads and two resources; the threads are deadlocked.]{.caption-text}[\#](#fig-sync-bugs-resource-graph "Link to this image"){.headerlink}](../_images/resource_graph.drawio.png){style="width: 25%;"}

Returning to our bank transfer example, the situation in [[Fig. 26.6]{.std .std-numref}](#fig-sync-bugs-resource-graph){.reference .internal} could arise if R1 and R2 are accounts, and T1 is running `transfer(R1, R2, amt1)`{.docutils .literal .notranslate} while T2 is running `transfer(R2, R1, amt2)`{.docutils .literal .notranslate}. In the `transfer()`{.docutils .literal .notranslate} function code, each thread first acquires the lock on the source account, so T1 locks R1 and T2 locks R2. Then, each thread attempts to acquire the lock on the destination account, so T1 blocks waiting for T2 to release R2, and T2 blocks waiting for T1 to release R1.
:::

::: {#the-four-conditions-for-deadlock .section}

### [26.3.3. ] {.section-number}The Four Conditions for Deadlock[\#](#the-four-conditions-for-deadlock "Link to this heading") {.headerlink}

Deadlocks in concurrent software systems were described by Djikstra [\[[Dij65](../misc/bib.html#id5){.reference .internal}\]]{#id5}, who called them "the deadly embrace". A few years later, Coffman et al. laid out the formal conditions for deadlock to occur [\[[CES71](../misc/bib.html#id11 "E. G. Coffman, M. Elphick, and A. Shoshani. System deadlocks. ACM Comput. Surv., 3(2):67–78, jun 1971. URL: https://doi.org/10.1145/356586.356588, doi:10.1145/356586.356588."){.reference .internal}\]]{#id6}:

Mutual exclusion

:   Threads are granted exclusive access to the resources they need; a resource that has been allocated to one thread cannot be used by any other thread.

Hold and wait

:   A thread holding resources can request additional ones; if the additional resources are not available, the thread will wait for them while continuing to hold onto the resources it has already been granted.

No preemption

:   Previously granted resources cannot be forcibly taken away from a thread; threads must voluntarily release resources when they are done using them.

Circular wait

:   There exists a circular chain of threads, each of which is waiting for a resource held by the next member of the chain.

These conditions, taken together, are necessary and sufficient for deadlock. If we break one of the four conditions, then deadlock cannot occur. Let's try attacking each condition in turn.
:::

::: {#breaking-mutual-exclusion .section}
[]{#cont-sync-concurrency-bugs-break-mutex}

### [26.3.4. ] {.section-number}Breaking Mutual Exclusion[\#](#breaking-mutual-exclusion "Link to this heading") {.headerlink}

Recall that we introduced mutual exclusion as one of the requirements for a solution to the critical section problem. Herlihy, however, showed that we can devise *non-blocking* algorithms to operate on concurrent data structures without enforcing mutual exclusion, given atomic hardware instructions such as `compare-and-swap`{.docutils .literal .notranslate} (`CAS`{.docutils .literal .notranslate}) [\[[Her93](../misc/bib.html#id14 "Maurice Herlihy. A methodology for implementing highly concurrent data objects. ACM Trans. Program. Lang. Syst., 15(5):745–770, nov 1993. URL: https://doi.org/10.1145/161468.161469, doi:10.1145/161468.161469."){.reference .internal}\]]{#id7} [\[[Her90](../misc/bib.html#id13 "M. Herlihy. A methodology for implementing highly concurrent data structures. In Proceedings of the Second ACM SIGPLAN Symposium on Principles & Practice of Parallel Programming, PPOPP '90, 197–206. New York, NY, USA, 1990. Association for Computing Machinery. URL: https://doi.org/10.1145/99163.99185, doi:10.1145/99163.99185."){.reference .internal}\]]{#id8}. These algorithms and data structures are called *lock-free* if they guarantee that *some* thread will complete an operation in a finite number of steps taken by itself or other threads, and *wait-free* if they guarantee that *each* thread will complete an operation in a finite number of steps.

The basic idea behind lock-free synchronization is to attempt to make a change optimistically, assuming there will be no interference from other threads. If any interference happens there must be a way to detect and recover from it, usually by retrying the operation. The `CAS(location, expected, new)`{.docutils .literal .notranslate} atomic instruction (see [[Listing 25.14]{.std .std-numref}](locks.html#listing-sync-cas){.reference .internal}) has this flavor---if the specified memory location still contains the expected value, then there has been no interference, the memory location can be updated with the new value, and the `CAS`{.docutils .literal .notranslate} succeeds. If the `CAS`{.docutils .literal .notranslate} fails, then the operation must be retried.

For example, suppose we needed to implement an `AtomicAdd()`{.docutils .literal .notranslate} function. We saw earlier ([[Listing 25.5]{.std .std-numref}](sharing.html#listing-sync-counter-assembly){.reference .internal}) that incrementing or decrementing a variable involves multiple steps, and so we used a lock to make those steps atomic.

::: {.highlight-c .notranslate}
::: highlight
pthread_mutex_t L = PTHREAD_MUTEX_INITIALIZER;

```
void AtomicAdd(int *val, int a) 
{
    pthread_mutex_lock(&L);
    *val += a;
    pthread_mutex_unlock(&L);
}
```

:::
:::

The overhead of acquiring and releasing the lock, however, far exceeds the work of the actual integer addition, making this a very inefficient solution. Using `CAS`{.docutils .literal .notranslate} we can avoid locking. The solution is shown below:

::: {.highlight-c .notranslate}
::: highlight
1void AtomicAdd(int *val, int a)
2{
3    do {
4        int old = *val;
5        int new = old + a;
6    } while (CAS(val, old, new) == false);
7}
:::
:::

A thread first reads the current value of the variable from the memory location, then adds the requested amount to obtain the new value. The `CAS`{.docutils .literal .notranslate} will succeed if the value stored in the memory location still matches the old value that was read. If another thread has managed to complete its own `AtomicAdd`{.docutils .literal .notranslate} on the same location between the read of the old value at line 4 and the `CAS`{.docutils .literal .notranslate} on line 6, then the memory location will no longer contain the `old`{.docutils .literal .notranslate} value, the `CAS`{.docutils .literal .notranslate} will fail (returning `false`{.docutils .literal .notranslate}) and the thread will return to line 4 for another attempt. We can see that the `AtomicAdd()`{.docutils .literal .notranslate} is lock-free, because some thread's `CAS`{.docutils .literal .notranslate} must succeed. It is not wait-free, however, because an unlucky thread could retry an arbitrary number of times without completing its operation.

The `CAS`{.docutils .literal .notranslate} primitive suffers from what is called the `ABA`{.docutils .literal .notranslate} problem. Briefly, a `CAS`{.docutils .literal .notranslate} succeeds when the memory location contains the expected value, however, this does not mean that nothing has changed. It is possible for thread T1 to read a value `A`{.docutils .literal .notranslate}, thread T2 to change the value to `B`{.docutils .literal .notranslate}, and thread T3 to change the value back to `A`{.docutils .literal .notranslate} again before T1 attempts a `CAS`{.docutils .literal .notranslate}. T1's `CAS`{.docutils .literal .notranslate} would succeed, even though the execution of other threads had been interleaved with its own accesses to the memory location. In the case of the `AtomicAdd()`{.docutils .literal .notranslate} shown above, this interleaving is harmless---so long as the current value matches what the thread read previously, the new value will be correct. In implementations of more complex data structures such as a non-blocking stack, however, more care is needed to correctly handle the `ABA`{.docutils .literal .notranslate} problem.

While non-blocking algorithms can prevent deadlocks by eliminating the mutual exclusion requirement, they are complex and hard to design. Efficient non-blocking algorithms exist for a handful of important data structures (e.g., stacks, queues, and linked lists) but there are many situations where they cannot be applied. Consider the bank account `transfer()`{.docutils .literal .notranslate} function, for example: we can easily update either account using our lock-free `AtomicAdd()`{.docutils .literal .notranslate}, but this doesn't help us to atomically update *both* accounts. We are often stuck with the mutual exclusion requirement for correctness, so we must look elsewhere for a solution to deadlock.

We will discuss *Read-Copy-Update* (RCU), a widely used primitive that provides lock-free synchronization for readers of a data structure, later.
:::

::: {#breaking-hold-and-wait .section}
[]{#cont-sync-concurrency-bugs-deadlock-holdandwait}

### [26.3.5. ] {.section-number}Breaking Hold-and-Wait[\#](#breaking-hold-and-wait "Link to this heading") {.headerlink}

If threads acquire all the resources they need before starting execution, then a thread will never have to wait for additional resources while holding onto resources it has already been granted. Once a thread is able to start running, it will have everything it needs to finish, making the resources available again for other threads. No deadlock! Unfortunately, there are several significant problems with this approach:

- A thread with 'large' resource needs (e.g., many different locks) may have to wait for a long time for all resources to be available at the same time. Additional effort is needed to ensure these threads do not starve.
- The system concurrency is limited because threads must acquire all resources before starting, rather than acquiring them when they needed. Consequently, resources are tied up for a longer time, even when they could be safely used by other threads.
- A thread may not know all the resources that it will need before it even starts running. Particularly for interactive tasks, input from the user can heavily influence what resources are needed next.

As a general strategy, acquiring all resources before starting execution is not very promising, although it may be used in some specialized systems such as batch processing. Another way to break the hold-and-wait condition requires a thread to release all the resources it already holds before it can request an additional resource. The thread must then submit a batch request for all the resources it needs (the ones it just gave up, and the new resource). The thread will be blocked until the complete set of resources can be allocated to it, but it will not be holding any resources while it waits. This strategy does not prevent starvation of a thread that needs a large number of resources simultaneously, and it requires care on the part of the programmer to ensure that data structures are not left in an inconsistent state when the resources are released.

There is a lot of overhead in giving up existing resources (e.g., releasing all the locks already acquired) and then immediately asking for them back again, particularly when the additional resource was already available. To help with this situation, some thread libraries offer a `trylock()`{.docutils .literal .notranslate} function:

- `pthread_mutex_trylock(pthread_mutex_t *mutex)`{.docutils .literal .notranslate}: Acquire the lock referenced by `mutex`{.docutils .literal .notranslate} if it is available and return 0; if `mutex`{.docutils .literal .notranslate} is currently locked, the call will return immediately with an error code.

A thread holding one or more locks already will first try to acquire an additional lock with a `trylock()`{.docutils .literal .notranslate} operation. If it succeeds, then there is no need to release the locks it already held. If the `trylock()`{.docutils .literal .notranslate} fails, however, the thread must release all of the other locks and try again to acquire the full set of locks. For example:

::: {#listing-sync-bugs-transfer-trylock .literal-block-wrapper .docutils .container}
::: code-block-caption
[Listing 26.2 ]{.caption-number}[Simple bank transfer, using trylock to break the hold-and-wait condition]{.caption-text}[\#](#listing-sync-bugs-transfer-trylock "Link to this code"){.headerlink}
:::

::: {.highlight-c .notranslate}
::: highlight
1void transfer(account_t *src_acct, account_t *dest_acct, money_t amount)
2{
3    pthread_mutex_lock(&src_acct->acct_lock);
4    while (pthread_mutex_trylock(&dest_acct->acct_lock) == EBUSY) {
5        pthread_mutex_unlock(&src_acct->acct_lock);
6        pthread_mutex_lock(&src_acct->acct_lock);
7    }
8
9    src_acct->balance -= amount;
10    dest_acct->balance += amount;
11
12    pthread_mutex_unlock(&dest_acct->acct_lock);
13    pthread_mutex_unlock(&src_acct->acct_lock);
14}
:::
:::
:::

By releasing the source account lock on line 5 when the destination account is already locked by another thread, we prevent deadlock from occurring. There is, however, a new possibility of *livelock* in which our two threads performing conflicting transfers, T1 and T2, continually lock one account, find the second account locked by another thread, release their first lock and try again. Inserting some random delay between the release on line 5 and the re-acquisition on line 6 can reduce the likelihood that threads will repeatedly conflict in this way.

**Two-Phase Locking**

Breaking the hold-and-wait condition is related to *two-phase locking*, which is a common strategy in database systems. In two-phase locking, an operation that requires multiple locks executes first in a *growing* phase, and then in a *shrinking phase*. In Phase One (growing), the thread tries to acquire all the locks it needs, one at a time. If any lock is unavailable, then it releases all the locks and starts over. Once Phase One succeeds, the thread has all the locks it needs, and can start performing updates, after which it can release the locks. This version of two-phase locking prevents deadlocks by not allowing the hold-and-wait condition. (Note that in the database literature, two-phase locking is often described with hold-and-wait in Phase One. Deadlocks are thus possible, and the database system needs a strategy for detecting them and aborting one of the transactions that is involved in the deadlock cycle.)
:::

::: {#allowing-preemption-breaking-the-no-preemption-condition .section}

### [26.3.6. ] {.section-number}Allowing Preemption (breaking the no preemption condition)[\#](#allowing-preemption-breaking-the-no-preemption-condition "Link to this heading") {.headerlink}

For certain physical resources, we can prevent deadlock by forcibly preempting the resource from one thread and allocating it to another. In particular, this works for resources that we can *virtualize* so that each thread has the illusion of its own private copy of the resource. For example, a physical CPU can be allocated to one thread for a timeslice, then forcibly preempted and allocated to another thread. Similarly, a page of physical memory can be allocated to the use of one address space, then preempted and reallocated to the use of another address space. In both cases, this is feasible because we can save the state of the resource (in the thread struct for the CPU, or in the swap file for memory) when it is preempted from a thread, and restore the state when it is returned to the thread.

However, when we are dealing with shared data structures, breaking 'no preemption' is not a very appealing option. We don't generally know the state of the data structure if we preempt a lock from a thread in the middle of a critical section, so we have no way of ensuring that the data is consistent before allowing another thread to access it. We also can't guarantee that it is safe for the original thread to resume from the point at which it was preempted, and we have no way of rolling back or aborting the operation that the thread was in the middle of performing. In contrast, database systems include transactional logging mechanisms that make it possible to abort a transaction, preempting the locks that the transaction held and restoring the database to its pre-transaction state.
:::

::: {#breaking-circular-wait .section}

### [26.3.7. ] {.section-number}Breaking Circular Wait[\#](#breaking-circular-wait "Link to this heading") {.headerlink}

The final condition we have to consider is the circular wait. It is quite appealing to allow the first three conditions, since they all serve to make it easier to write correct concurrent code, while ensuring that we never find ourselves in a situation with a circular chain of threads holding some resources and waiting for a resource held by the next thread in the chain.

One idea that we can immediately reject is to prevent circular wait by only allowing a thread to request or hold one resource at a time. There are simply too many scenarios where a thread needs to use multiple resources together to accomplish the desired task, such as transferring between two bank accounts. The only feasible way to implement this idea is to have a 'big giant lock' that protects all the resources in the system that could possibly be used together. Then, threads would only need a single resource, namely the big giant lock. In our bank scenario, this would mean a single lock for all the bank accounts, but the resulting loss of concurrency would be unacceptable.

The other option is to provide a global ordering of resources, and require all threads to acquire resources according to this ordering. That is, a thread holding resource [\\(j\\)]{.math .notranslate .nohighlight} cannot make a request for resource [\\(i\\)]{.math .notranslate .nohighlight} where [\\(i\\)]{.math .notranslate .nohighlight} \< [\\(j\\)]{.math .notranslate .nohighlight} in the global ordering. The resulting resource allocation graph is guaranteed to contain no cycles, and circular wait is impossible. There are several challenges with this idea in practice. The first is that it may be difficult to come up with a global ordering for a system when there are a large number of different resources. The second is that it relies on programmers to know and respect the global ordering when they write code. Nonetheless, it is a very widely used and effective strategy in practice.

Returning again to our bank transfer function, we can use the account numbers to define a global lock ordering: lower-numbered accounts precede higher-numbered accounts in the lock ordering. An example of this strategy is shown in [[Listing 26.3]{.std .std-numref}](#listing-sync-bugs-transfer-ordering){.reference .internal}.

::: {#listing-sync-bugs-transfer-ordering .literal-block-wrapper .docutils .container}
::: code-block-caption
[Listing 26.3 ]{.caption-number}[Simple bank transfer, using lock ordering to break the circular wait condition]{.caption-text}[\#](#listing-sync-bugs-transfer-ordering "Link to this code"){.headerlink}
:::

::: {.highlight-c .notranslate}
::: highlight
1void transfer(account_t *src_acct, account_t *dest_acct, money_t amount)
2{
3    if (src_acct->acct_num < dest_acct->acct_num) {
4        pthread_mutex_lock(&src_acct->acct_lock);
5        pthread_mutex_lock(&dest_acct->acct_lock);
6    } else {
7        pthread_mutex_lock(&dest_acct->acct_lock);
8        pthread_mutex_lock(&src_acct->acct_lock);
9    }
10
11    src_acct->balance -= amount;
12    dest_acct->balance += amount;
13
14    pthread_mutex_unlock(&dest_acct->acct_lock);
15    pthread_mutex_unlock(&src_acct->acct_lock);
16}
:::
:::
:::

Now, if T1 is running `transfer(R1, R2, amt1)`{.docutils .literal .notranslate} while T2 is running `transfer(R2, R1, amt2)`{.docutils .literal .notranslate}, the two threads must lock the accounts in the same order. Suppose R2 has a lower account number than R1. Then, T1 will execute lines 7-8, locking R2 first followed by R1, and T2 will execute lines 4-5, also locking R2 followed by R1. Whichever thread succeeds in locking R2 first will proceed to lock R1 and complete its transfer, releasing both the locks and allowing the other thread to proceed. Deadlock is prevented.
:::

::: {#reality-check .section}

### [26.3.8. ] {.section-number}Reality Check[\#](#reality-check "Link to this heading") {.headerlink}

No single strategy for dealing with deadlock is appropriate for all resources in all situations. Moreover, all strategies are costly in terms of computation overhead, or restricting the use of resources. Consequently, many systems make some use of what Tanenbaum refers to as "the ostrich algorithm": ignore the problem and hope it doesn't happen too often [\[[TB14](../misc/bib.html#id15 "Andrew S. Tanenbaum and Herbert Bos. Modern Operating Systems. Prentice Hall Press, USA, 4th edition, 2014. ISBN 013359162X."){.reference .internal}\]]{#id9}. This isn't really as shocking as it might sound at first. For personal computers, which are rebooted frequently, the rare inconvenience of manually resolving a deadlock (by forcibly killing some tasks, or rebooting the machine) is likely to be preferable to the constant overhead of ensuring deadlocks don't occur. On the other hand, deadlocks are unacceptable in safety critical systems and ensuring they don't occur is worth some loss in performance. Modern operating systems like Linux employ a mix of strategies for deadlock, including using lock-free algorithms when possible, defining a well-documented lock hierarchy that kernel programmers are expected to follow, and providing runtime lock validators that check for deadlocks or incorrect lock usage. Because of the high runtime cost, such validators are generally used during development but not in deployment.
:::
:::

::: {#livelock-starvation-and-other-bugs .section}

## [26.4. ] {.section-number}Livelock, Starvation and Other Bugs[\#](#livelock-starvation-and-other-bugs "Link to this heading") {.headerlink}

While atomicity violations, order violations, and deadlocks collectively made up over 98% of the concurrency bugs in Lu et al.'s study [\[[LPSZ08](../misc/bib.html#id10 "Shan Lu, Soyeon Park, Eunsoo Seo, and Yuanyuan Zhou. Learning from mistakes: a comprehensive study on real world concurrency bug characteristics. In Proceedings of the 13th International Conference on Architectural Support for Programming Languages and Operating Systems, ASPLOS XIII, 329–339. New York, NY, USA, 2008. Association for Computing Machinery. URL: https://doi.org/10.1145/1346281.1346323, doi:10.1145/1346281.1346323."){.reference .internal}\]]{#id10}, there are other subtle concurrency issues that can occur.

In [[Section 26.3.5]{.std .std-numref}](#cont-sync-concurrency-bugs-deadlock-holdandwait){.reference .internal}, we briefly mentioned *livelock*, which occurs when threads are running and changing state, but are not making progress towards completing an operation. The common example of a real-world livelock is when two people meet in a narrow corridor and each repeatedly steps aside in the same direction to let the other person pass. The `trylock`{.docutils .literal .notranslate} scenario is one way that livelock can occur in a computer system. More generally, livelocks can happen whenever threads continually retry a failed operation. For example, there is usually some limit on the number of files that a process can have open. Suppose this limit is set to 10 and we have a multithreaded process with 16 threads, each of which needs to open 2 files (say, to read its input and write its output). If a thread's attempt to open a file fails because there are too many open files already (e.g., `open()`{.docutils .literal .notranslate} returns -1 with `errno == EMFILE`{.docutils .literal .notranslate} "Too many open files"), then the thread will simply try to open the file again, in the hopes that some other thread will finish, close its files, and allow this thread to proceed. Code for this is depicted in [[Listing 26.4]{.std .std-numref}](#listing-sync-bugs-livelock-files){.reference .internal}. Now, if all available open files are used by threads that have opened their input files, no thread will be able to open an output file and complete its work. This scenario looks extremely similar to deadlock: we have a limited set of resources (slots in the open file table), all of the resources have been allocated to threads, and all of the threads are holding their resources while waiting for an additional resource that is held by another thread. The difference is that the threads are not blocked---they are repeatedly issuing an `open()`{.docutils .literal .notranslate} system call and getting a response, so work is being done, but the threads are not making any progress.

::: {#listing-sync-bugs-livelock-files .literal-block-wrapper .docutils .container}
::: code-block-caption
[Listing 26.4 ]{.caption-number}[thread function from livelock.c - Example of livelock due to open file limit.]{.caption-text}[\#](#listing-sync-bugs-livelock-files "Link to this code"){.headerlink}
:::

::: {.highlight-default .notranslate}
::: highlight
1void *threadfunc(void *arg)
2{
3    struct args_s *my_args = (struct args_s *)arg;
4
5    int fd_in;
6    int fd_out;
7
8    /* Open input file, retrying if there are too many files already open */
9    for ( ; ; ) {
10        fd_in = open(my_args->infile, O_RDONLY);
11        if (fd_in > 0) {
12            break;
13        }
14        if (errno != EMFILE) {
15            return NULL;
16        }
17    }
18
19    fprintf(stderr,"Thread %d has input file %s open now.\n",
20            my_args->id, my_args->infile);
21
22    /* Open output file, retrying if there are too many files already open */
23    for ( ; ; ) {
24        fd_out = open(my_args->outfile, O_RDWR);
25        if (fd_out > 0) {
26            break;
27        }
28        if (errno != EMFILE)  {
29            close(fd_in);
30            return NULL;
31        }
32    }
33    fprintf(stderr,"Thread %d has output file %s open now.\n",
34            my_args->id, my_args->outfile);
35
36    /* Sleep for a while to simulate time reading input and producing output */
37    sleep(1);
38
39    close(fd_in);
40    close(fd_out);
41
42    return NULL;
43}
:::
:::
:::

Another study of bugs in open source code [\[[AASEH17](../misc/bib.html#id16 "Abbaspour Asadollah, S., Sundmark, D., Eldh, S., and Hans Hansson. Concurrency bugs in open source software: a case study. Journal of Internet Services and Applications, 8(4):1-15, apr 2017. URL: https://doi.org/10.1186/s13174-017-0055-2, doi:10.1186/s13174-017-0055-2."){.reference .internal}\]]{#id11} found that livelock bug reports were extremely rare (only 2 out of 351 concurrency-related bug reports). This may be because of the difficulty in diagnosing and reproducing livelocks, or because programmers were aware of the potential for livelock and took care to avoid it (for example, by setting a limit on the number of retries).

**Starvation** is distinct from deadlock and livelock, although, again, some thread (or threads) never receive the resources they need. The difference is that the resource(s) a thread is waiting for will repeatedly become free, but is always allocated to a different thread. We saw this in shortest-job-first scheduling, where an infinite sequence of short threads are always granted the CPU ahead of a long-running thread. Starvation may also occur if a thread has to give up all the resources (locks) it already holds before it is allowed to request more resources. Starvation related to synchronization can also occur with reader/writer locks, where threads that only need to read a data object can execute concurrently using a shared lock but threads that need to write the data object must obtain an exclusive lock, waiting for all readers to finish. Finally, starvation can occur due to characteristics of modern hardware that give some threads an advantage when competing for a lock, such as NUMA memory systems and caching.

Finally, there are concurrency bugs that are difficult to classify. Lu et al. provide one example from MySQL, where the developers included a *watchdog* thread to monitor other threads for potential deadlock. The monitor was designed to crash the server, forcing a restart, if it detected that some thread had waited for more than `fatal_timeout`{.docutils .literal .notranslate} to acquire a lock. A simplified version of this scenario is depicted in [[Fig. 26.7]{.std .std-numref}](#fig-sync-bugs-timing){.reference .internal}. Unfortunately, when the workload was high, there could be a very large number of worker threads and the lock wait time frequently exceeded the allowed timeout. The developers had not considered how to adjust the fatal timeout value based on the workload.

![[Fig. 26.7 ]{.caption-number}[Example of a concurrency-related bug from MySQL.]{.caption-text}[\#](#fig-sync-bugs-timing "Link to this image"){.headerlink}](../_images/timing_bug.drawio.png){style="width: 90%;"}
:::
:::

::: prev-next-area
[](ordering.html "previous page"){.left-prev}

::: prev-next-info
previous

[25.4. ]{.section-number}Ordering Thread Events
:::

[](advanced.html "next page"){.right-next}

::: prev-next-info
next

[27. ]{.section-number}Advanced Synchronization
:::
:::
:::

::: {.bd-sidebar-secondary .bd-toc}
::: {.sidebar-secondary-items .sidebar-secondary__inner}
::: sidebar-secondary-item
::: {.page-toc .tocsection .onthispage}
Contents
:::

- [26.1. Atomicity Violations](#atomicity-violations){.reference .internal .nav-link}
- [26.2. Order Violations](#order-violations){.reference .internal .nav-link}
- [26.3. Deadlocks](#deadlocks){.reference .internal .nav-link}
  - [26.3.1. What is a resource?](#what-is-a-resource){.reference .internal .nav-link}
  - [26.3.2. Visualizing and Modeling Deadlocks](#visualizing-and-modeling-deadlocks){.reference .internal .nav-link}
  - [26.3.3. The Four Conditions for Deadlock](#the-four-conditions-for-deadlock){.reference .internal .nav-link}
  - [26.3.4. Breaking Mutual Exclusion](#breaking-mutual-exclusion){.reference .internal .nav-link}
  - [26.3.5. Breaking Hold-and-Wait](#breaking-hold-and-wait){.reference .internal .nav-link}
  - [26.3.6. Allowing Preemption (breaking the no preemption condition)](#allowing-preemption-breaking-the-no-preemption-condition){.reference .internal .nav-link}
  - [26.3.7. Breaking Circular Wait](#breaking-circular-wait){.reference .internal .nav-link}
  - [26.3.8. Reality Check](#reality-check){.reference .internal .nav-link}
- [26.4. Livelock, Starvation and Other Bugs](#livelock-starvation-and-other-bugs){.reference .internal .nav-link}
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
