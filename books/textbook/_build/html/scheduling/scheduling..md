---
tip: translate by baidu@2024-07-18 12:55:29
docsearch:language: en
lang: en
title: 10. Scheduling --- Introduction to Operating Systems
viewport:
  - width=device-width, initial-scale=1.0
  - width=device-width, initial-scale=1
  - width=device-width, initial-scale=1
---

# Scheduling

Scheduling is the policy the operating system uses to time multiplexes the CPU between different tasks. A large number of scheduling policies have been developed over the years. Some of these are specialized for particular types of computing systems, while others aim to support more general-purpose systems. We first discuss why scheduling is complicated and the goals scheduling policies are designed to meet, and then review a number of these policies.

> 调度是操作系统用于在不同任务之间对 CPU 进行时间复用的策略。多年来，已经制定了大量的调度策略。其中一些专门用于特定类型的计算系统，而另一些则旨在支持更通用的系统。我们首先讨论了为什么调度很复杂，以及调度策略旨在满足的目标，然后回顾了其中一些策略。

::: {.admonition .note}
Note

**Space and time multiplexing:** In reality today all computers have many physical CPUs, and the kernel does both space and time multiplexing. Given the existence of caches and NUMA memory, the decision of not only when to run a task but also where (i.e. on which CPU) to run it has profound performance implications. However, we will largly focus on introducing the problem of scheduling from he perspective of a single CPU.

> **空间和时间复用：**事实上，今天所有的计算机都有许多物理 CPU，内核同时进行空间和时间的复用。考虑到缓存和 NUMA 内存的存在，不仅要决定何时运行任务，还要决定在哪里（即在哪个 CPU 上）运行任务，这对性能有着深远的影响。然而，我们将主要从单个 CPU 的角度介绍调度问题。
> :::
