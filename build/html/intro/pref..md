---
docsearch:language: en
lang: en
title: Preface --- Introduction to Operating Systems
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
[![Introduction to Operating Systems - Home](../_static/logo.png){.logo__image .only-light}](#){.navbar-brand .logo}
:::

::: sidebar-primary-item
:::

::: sidebar-primary-item
::: {.bd-toc-item .navbar-nav .active}

- [Preface](#){.reference .internal}

[Getting started]{.caption-text}

- [1. Introduction](intro.html){.reference .internal}
- [2. Purpose of operating systems](purpose.html){.reference .internal}
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

- [[ ![JupyterHub logo](../_static/images/logo_jupyterhub.svg) ]{.btn__icon-container} [JupyterHub]{.btn__text-container}](https://jupyterhub-opf-jupyterhub.apps.smaug.na.operate-first.cloud/hub/user-redirect/git-pull?repo=https%3A//github.com/OpenOSOrg/openos&urlpath=lab/tree/openos/content/intro/pref.ipynb&branch=main "Launch on JupyterHub"){.btn .btn-sm .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
  :::

::: {.dropdown .dropdown-source-buttons}

- [[ ]{.btn__icon-container} [Repository]{.btn__text-container}](https://github.com/OpenOSOrg/openos "Source repository"){.btn .btn-sm .btn-source-repository-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
- [[ ]{.btn__icon-container} [Suggest edit]{.btn__text-container}](https://github.com/OpenOSOrg/openos/edit/main/content/intro/pref.ipynb "Suggest edit"){.btn .btn-sm .btn-source-edit-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
- [[ ]{.btn__icon-container} [Open issue]{.btn__text-container}](https://github.com/OpenOSOrg/openos/issues/new?title=Issue%20on%20page%20%2Fintro/pref.html&body=Your%20issue%20content%20here. "Open an issue"){.btn .btn-sm .btn-source-issues-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
  :::

::: {.dropdown .dropdown-download-buttons}

- [[ ]{.btn__icon-container} [.ipynb]{.btn__text-container}](../_sources/intro/pref.ipynb "Download source file"){.btn .btn-sm .btn-download-source-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}

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

# Preface

::: {#print-main-content}
::: {#jb-print-toc}

<div>

## Contents

</div>

- [Our motivation](#our-motivation){.reference .internal .nav-link}
- [Book Overview](#book-overview){.reference .internal .nav-link}
  :::
  :::
  :::

::: {#searchbox}
:::

::: {#preface .section .tex2jax_ignore .mathjax_ignore}
[]{#cont-pref}

# Preface[\#](#preface "Link to this heading") {.headerlink}

In late 2021 Jonathan Appavoo started discussing with us his vision of creating open source interactive educational materials. You can see an early talk on this [here](https://research.redhat.com/events/steps-toward-open-source-education/){.reference .external}. Somehow, we found ourselves committing to writing an operating system textbook, and here we are. You will eventually find in the repository three kinds of information:

1. This textbook which will largely be static content.
2. Lab materials which will include significant amounts of interactive content.
3. Lecture slides

Right now, we are focused only on the textbook portion of this materials. It can be largely read statically; and you can even download a PDF (see download symbol top right). However, we strongly recommend using it online going back and forth between different materials via the provided links. We provide a companion container (an OS concept we will [[discuss]{.std .std-ref}](../virt/virt.html#virt-containers){.reference .internal} which we strongly recommend you keep open alongside the material and use to run exercises. The lab materials are intended to execute in the container. Moreover, the container has the curated set of tools that we expect you to use for the course, and provides the same environment as the assignments; you are likely to run into problems if you work on the assignments outside of the container environment and don't expect TAs to help you if you do that.

Please see [[here]{.std .std-ref}](../contributing/credit.html#cont-contr-contributors){.reference .internal} for the list of contributors. This text was originally developed for the Boston University course EC440 Introduction to Operating Systems. You can [view this text online](https://okrieg.github.io/openos/textbook/intro_tb.html){.reference .external} or [view the source](https://github.com/okrieg/openos){.reference .external}.

::: {#our-motivation .section}
[]{#cont-pref-mot}

## Our motivation[\#](#our-motivation "Link to this heading") {.headerlink}

Our motivation to write this book is three fold. First, our students pay way too much money for textbooks. At one point, students could buy used textbooks, although even then publishers would constantly churn editions to get students to buy new versions. Increasingly, textbooks contain interactive materials, that force students to buy the most recent edition; again its about the money. Free online books (FOB) provide us the opportunity to address this cost issue, while also enabling frequent revisions and extensive linking between different materials. The motivation for FOB for operating systems is described in the excellent [blog](http://from-a-to-remzi.blogspot.com/2014/01/the-case-for-free-online-books-fobs.html){.reference .external} by Remzi Arpaci-Dusseau. Moreover, the excellent operating system FOB titled "[Operating Systems: Three Easy Pieces](https://pages.cs.wisc.edu/~remzi/OSTEP/){.reference .external}" [\[[ADAD18](../misc/bib.html#id2 "Remzi H Arpaci-Dusseau and Andrea C Arpaci-Dusseau. Operating systems: Three easy pieces. Arpaci-Dusseau Books LLC Boston, 2018. URL: https://pages.cs.wisc.edu/~remzi/OSTEP/."){.reference .internal}\]]{#id1}, is enormously better than our effort today. So why are we developing another FOB? That leads to our next two reasons.

Second, we have found students think in many different ways and repetition at multiple different levels of detail is incredibly important to understand operating systems. The Three Easy pieces FOB does a great job of interlinking materials, enabling students to approach the material in multiple ways. However, with jupyter book and containers we can go much further; enabling dynamic content that is deeply connected to the book. Our own experience as OS developers and researchers is that we don't understand anything until we have played with code; we hope that the model we are developing based on Jonathans OPE will enable us to give students more of that experience. In fact, as Jonathan articulates so well in the talk referenced above, students today have grown up with so many levels of software complexity obscuring the systems they are using that this interactive experience is critical to enable systems to be approached.

Third, as operating system researchers and developers that have experienced the entire growth of open source, we believe that open source can be an enormously powerful tool for educational materials. Textbooks get out of date soon after they are written; and this is especially the case in operating systems which are one of the most rapidly evolving technical areas. We believe that only an open source community will be able to create educational materials that evolve as fast as the topics they cover. While we respect Remzi's perspective from [\[[ADAD18](../misc/bib.html#id2 "Remzi H Arpaci-Dusseau and Andrea C Arpaci-Dusseau. Operating systems: Three easy pieces. Arpaci-Dusseau Books LLC Boston, 2018. URL: https://pages.cs.wisc.edu/~remzi/OSTEP/."){.reference .internal}\]]{#id2} that "a book should have a single voice", our own frustration of teaching from materials developed by others has led us to want to enable instructors to be able to modify any part of our content to teach operating systems in a way that reflects their background, their community of students, and their own biases. Feel free to fork our book at make it your own. We do hope that people will be motivated to offer their changes back to us; and they can do so using the same mechanisms used by community projects like Linux. Hopefully, we can do a good job and create standards and a community such that the material has a coherent single voice; if not, perhaps someone that is better at it will fork our book and create such a community.
:::

::: {#book-overview .section}
[]{#cont-pref-how}

## Book Overview[\#](#book-overview "Link to this heading") {.headerlink}

For detailed instructions on how to read this book and launch the container associated with it, please refer [[here]{.std .std-ref}](../misc/howto.html#misc-howto){.reference .internal}. The book is divided into multiple sections, each with small chapters that should hopefully be relatively fast reads. The first part, [[Getting Started]{.std .std-ref}](intro.html#cont-gs-intro){.reference .internal}, gives an overview of the entire book and the tools operating system developers like you will need to know. The next three parts describe three of the core services of operating systems, namely [[Scheduling]{.std .std-ref}](../scheduling/intro.html#cont-vp){.reference .internal}, [[Memory Management]{.std .std-ref}](../mm/intro.html#cont-mm-intro){.reference .internal}, and [[file systems]{.std .std-ref}](../fs/intro.html#cont-fs-intro){.reference .internal}. The next part, [[concurrency]{.xref .myst}](#cont:conc:intro){.reference .internal}, introduces some of the most complicated aspects of operating systems to deal with the parallelism of todays platforms, namely threads, synchronization, and deadlock. We have lumped a bunch of important topics that are typically only covered briefly in an introductory OS book, including security, virtualization, a bit on the history of operating systems and alternative OS structures. Finally the appendices have chapters on how to read and contribute to this book.

::: {.admonition .warning}
Warning

This book is a work in progress, most parts are today just scaffolding, and a [[community]{.std .std-ref}](../contributing/credit.html#cont-contr-contributors){.reference .internal} is working hard to try to get materials in place as we are actively reading it. We hope you will consider contributing to this effort by reporting [[issues]{.std .std-ref}](../misc/howto.html#misc-howto-issue){.reference .internal} you find.
:::
:::

::: {.toctree-wrapper .compound}
:::

::: {.toctree-wrapper .compound}
:::

::: {.toctree-wrapper .compound}
:::

::: {.toctree-wrapper .compound}
:::

::: {.toctree-wrapper .compound}
:::

::: {.toctree-wrapper .compound}
:::

::: {.toctree-wrapper .compound}
:::
:::

::: prev-next-area
[](intro.html "next page"){.right-next}

::: prev-next-info
next

[1. ]{.section-number}Introduction
:::
:::
:::

::: {.bd-sidebar-secondary .bd-toc}
::: {.sidebar-secondary-items .sidebar-secondary__inner}
::: sidebar-secondary-item
::: {.page-toc .tocsection .onthispage}
Contents
:::

- [Our motivation](#our-motivation){.reference .internal .nav-link}
- [Book Overview](#book-overview){.reference .internal .nav-link}
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
