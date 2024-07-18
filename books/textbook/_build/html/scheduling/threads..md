---
tip: translate by baidu@2024-07-18 13:09:39
docsearch:language: en
lang: en
title: "9. The Thread: A Virtual CPU --- Introduction to Operating Systems"
viewport:
  - width=device-width, initial-scale=1.0
  - width=device-width, initial-scale=1
  - width=device-width, initial-scale=1
---

# The Thread: A Virtual CPU

## Contents

# [9. ] {.section-number}The Thread: A Virtual CPU[\#](#the-thread-a-virtual-cpu "Link to this heading") {.headerlink}

If a process is a _virtual computer_, a **thread** is a _virtual CPU_. Modern computers have many CPUs, and many applications are written to exploit multiple _virtual CPU_ either to enable progress to be made while some threads are blocked, or to enable the program to exploit multiple physical CPUs. We call such applications multi-threaded applications. All the **threads** are part of the same process, sharing memory, open files, etc... they only differ in the set of registers run on the CPU. Of course, one of those registers is the stack pointer, so each thread by default has its own stack.

> 如果一个进程是一个虚拟计算机，那么一个线程就是一个虚拟 CPU。现代计算机有许多 CPU，许多应用程序都是为了利用多个虚拟 CPU 而编写的，要么是为了在某些线程被阻塞时取得进展，要么是使程序能够利用多个物理 CPU。我们称这种应用程序为多线程应用程序。所有**线程**都是同一进程的一部分，共享内存、打开文件等……它们只在 CPU 上运行的寄存器集上有所不同。当然，其中一个寄存器是堆栈指针，因此默认情况下每个线程都有自己的堆栈。

One special case of a multi-threaded program is the kernel itself. While many applications may run on a single CPU, the kernel has to run on all the CPUs. The major challenge to write multi-threaded programs, of which the kernel is probably the most extreme example, is how to ensure that the threads that are running at the same time **synchronize** so that they don't modify the same memory in incompatible ways at the same time. This is one of the most complex topics in operating systems, and we defer it to later (see [[synchronization]{.xref .myst}](#cont:conc:intro){.reference .internal}) after we have finished discussing memory management and file systems.

> 多线程程序的一个特例是内核本身。虽然许多应用程序可以在单个 CPU 上运行，但内核必须在所有 CPU 上运行。编写多线程程序的主要挑战（内核可能是其中最极端的例子）是如何确保同时运行的线程**同步**，这样它们就不会同时以不兼容的方式修改同一内存。这是操作系统中最复杂的主题之一，我们将在讨论完内存管理和文件系统后再讨论（请参阅[synchronize]{.xref.myst}]（#cont:conc:intro）{.reference.internal}）。

::: {#interface .section}

## [9.1. ] {.section-number}Interface[\#](#interface "Link to this heading") {.headerlink}

The standard interface for threads is posix threads. Like always, use `man`{.docutils .literal .notranslate} to find out more information about any of these calls. This interface is implemented in Linux using the pthread library on top of the system calls we have previously described. Core functions are:

> 线程的标准接口是 posix 线程。像往常一样，使用`man`{.docutils.literal.notranslate}来了解有关这些调用的更多信息。这个接口是在 Linux 中使用 pthread 库在我们之前描述的系统调用之上实现的。核心功能是：

- `err =  pthread_create(&id, attr, start_routine)`{.docutils .literal .notranslate}: creates a thread that will start executing at start_routine, returning status and the thread id

> -`err=pthread_create（&id，attr，start_routine）`{.docutils.literal.notranslate}：创建一个将在 start_routime 开始执行的线程，返回状态和线程 id

- `pthread_exit(retval)`{.docutils .literal .notranslate}: exit the current thread, returning to the parent the return value

> -`pthread_exit（retval）`{.docutils.literal.notranslate}：退出当前线程，将返回值返回给父线程

- `id = pthread_self()`{.docutils .literal .notranslate}: returns the id of the thread that called it

> -`id=pthread_self（）`{.docutils.literal.notranslate}：返回调用它的线程的 id

- `err = pthread_join(id, &retval)`{.docutils .literal .notranslate}: wait for thread specified by id to complete, and return its status.

> -`err=pthread_join（id，&retval）`{.docutils.literal.notranslate}：等待 id 指定的线程完成，并返回其状态。

In addition, there are a set of synchronization operations that we will discuss later.

> 此外，我们稍后将讨论一组同步操作。
> :::

::: {#implementation .section}

## [9.2. ] {.section-number}Implementation[\#](#implementation "Link to this heading") {.headerlink}

If you want to exploit multiple CPUs the easiest way is to have the abstraction of threads implemented by the kernel, just like processes. You may have wondered why in [[Fig. 4.2]{.std .std-numref}](../intro/abstractions.html#img-intro-proc){.reference .internal} and [[Listing 8.1]{.std .std-numref}](virtual.html#simple-task-struct){.reference .internal} Linux refers to the internal data structures as _tasks_ rather than processes. The implementation of the thread abstraction in the Linux kernel is that each thread is its own task, with its own thread state, and all the threads in a process point to the same MM and file struct data structures. With such a design, everything we have talked about context switching and scheduling in the previous chapter directly applies to threads, and the fact that multiple of these threads are part of a single process is irrelevant.

> 如果你想利用多个 CPU，最简单的方法是让内核实现线程的抽象，就像进程一样。你可能想知道为什么在[[图 4.2]{.std.std-numref}]（../intro/nabstracts.html#img-intro-proc）{.reference.internal}和[[清单 8.1]{.sdt.std-numaref}]。Linux 内核中线程抽象的实现是，每个线程都是自己的任务，有自己的线程状态，进程中的所有线程都指向相同的 MM 和文件结构数据结构。通过这样的设计，我们在上一章中讨论的上下文切换和调度都直接适用于线程，而这些线程中的多个是单个进程的一部分这一事实无关紧要。

You can also implement threads at user level. There are advantages to such implementation, where in user space one can quickly context switch between one thread and another without having to transition to the kernel and back. In fact, those of you taking EC440 at BU, you will be implementing your own user level threading system. If you implement threads totally at user level, then if any thread makes a system call, it will block all the other threads from running. Also, user-level threads if implemented on a single kernel level thread have no parallelism, i.e. they cannot exploit multiple CPUs.

> 您还可以在用户级别实现线程。这种实现有很多优点，在用户空间中，可以在一个线程和另一个线程之间快速切换上下文，而无需转换到内核并返回。事实上，你们中在 BU 学习 EC440 的人，将实现自己的用户级线程系统。如果你完全在用户级别实现线程，那么如果任何线程进行系统调用，它将阻止所有其他线程运行。此外，如果在单个内核级线程上实现，则用户级线程没有并行性，即它们不能利用多个 CPU。

There is also literature of research that multiplexes some number of user level threads on top of some number of kernel thread, with perhaps the best known work, Scheduler Activations [\[[ABLL91](../misc/bib.html#id19 "Thomas E. Anderson, Brian N. Bershad, Edward D. Lazowska, and Henry M. Levy. Scheduler activations: effective kernel support for the user-level management of parallelism. In Proceedings of the Thirteenth ACM Symposium on Operating Systems Principles, SOSP '91, 95–109. New York, NY, USA, 1991. Association for Computing Machinery. URL: https://doi.org/10.1145/121132.121151, doi:10.1145/121132.121151."){.reference .internal}\]]{#id1}, proposing specific support in a kernel to enable efficient design of user level threads.

> 还有研究文献表明，在一定数量的内核线程之上复用一定数量的用户级线程，其中最著名的工作可能是调度器激活[\[[ABL91]（../misc/bib.html#id19”Thomas E.Anderson、Brian N.Bershad、Edward D.Lazowska 和 Henry M.Levy。调度器激活：对并行性用户级管理的有效内核支持。载于第十三届 ACM 操作系统原理研讨会论文集，SOSP'91，95-109。美国纽约州纽约市，1991 年。国际计算机学会网址：https://doi.org/10.1145/121132.121151，doi:10.1145/121132.121151.“）{.reference.internal}\]]{#id1}，建议在内核中提供特定支持，以实现用户级线程的高效设计。
