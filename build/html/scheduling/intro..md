---
tip: translate by baidu@2024-07-18 13:03:43
docsearch:language: en
lang: en
title: 6. Introduction --- Introduction to Operating Systems
viewport:
  - width=device-width, initial-scale=1.0
  - width=device-width, initial-scale=1
  - width=device-width, initial-scale=1
---

# Introduction

# [6. ] {.section-number}Introduction[\#](#introduction "Link to this heading") {.headerlink}

We [[already]{.std .std-ref}](../intro/structure.html#cont-gs-structure-struc){.reference .internal} described the idea of a process, as a virtual computer that isolates running applications from each other, and discussed a bit how the [[OS]{.std .std-ref}](../intro/abstractions.html#cont-gs-abstractions-process){.reference .internal} implements that abstraction. We first [[review]{.std .std-ref}](process.html#cont-vp-process){.reference .internal} the abstraction of a process in more detail and [[then]{.std .std-ref}](virtual.html#cont-vp-virt){.reference .internal} how the operating system allows multiple processes to execute on a computer while giving each the illusion it has the entire computer to itself. We then discuss the abstraction of [[threads]{.std .std-ref}](threads.html#cont-vp-threads){.reference .internal}, which implements the abstraction of a virtual processor. The processor needs to be multiplexed between different applications, we then describe the goals of [[scheduling]{.std .std-ref}](scheduling.html#cont-vp-scheduling){.reference .internal} and a variety of scheduling algorithms.

> 我们[[已经]{.std.std-ref}]（../intro/structure.html#cont gs structure struc）{.reference.internal}描述了进程的概念，即一个将正在运行的应用程序彼此隔离的虚拟计算机，并讨论了[[OS]{.std.std-ref}]（…/intro/stabstractions.html#cont-gs abstractions process）{.rereference.internal]如何实现该抽象。我们首先[[回顾]{.std.std-ref}]（process.html#cont-vp-process）{.reference.internal}更详细地描述了进程的抽象，然后[[然后]{.sdt.std-ref}]（virtual.html#cont-vp-virt）{.review.internal]操作系统如何允许多个进程在计算机上执行，同时给每个进程一种它拥有整个计算机的错觉。然后，我们讨论[[threads]{.std.std-ref}]（threades.html#cont-vp-threads）{.reference.internal}的抽象，它实现了虚拟处理器的抽象。处理器需要在不同的应用程序之间进行复用，然后我们描述了[[调度]{.std.std-ref}]（调度.html#cont-vp 调度）{.reference.internal}和各种调度算法的目标。
> :::
