---
docsearch:language: en
lang: en
title: 34.7. Out of date --- Introduction to Operating Systems
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

- [29. Input and Output](../devices/devices.html){.reference .internal}
- [30. More on Disks](../devices/disk2.html){.reference .internal}
- [31. Virtualization](../virt/virt.html){.reference .internal}
- [32. Security](../sec/sec.html){.reference .internal}

[Appendices]{.caption-text}

- [33. How to read this book](../misc/howto.html){.reference .internal}
- [34. Contributing](intro.html){.reference .internal}
  []{.toctree-toggle role="presentation"}
  - [34.1. Examples](examples.html){.reference .internal}
  - [34.2. Contributors](credit.html){.reference .internal}
  - [34.3. Contributing](Contributing.html){.reference .internal}
  - [34.6. Resources to look at](resources.html){.reference .internal}
  - [34.7. Out of date](#){.current .reference .internal}
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

- [[ ![JupyterHub logo](../_static/images/logo_jupyterhub.svg) ]{.btn__icon-container} [JupyterHub]{.btn__text-container}](https://jupyterhub-opf-jupyterhub.apps.smaug.na.operate-first.cloud/hub/user-redirect/git-pull?repo=https%3A//github.com/OpenOSOrg/openos&urlpath=lab/tree/openos/content/contributing/fix.ipynb&branch=main "Launch on JupyterHub"){.btn .btn-sm .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
  :::

::: {.dropdown .dropdown-source-buttons}

- [[ ]{.btn__icon-container} [Repository]{.btn__text-container}](https://github.com/OpenOSOrg/openos "Source repository"){.btn .btn-sm .btn-source-repository-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
- [[ ]{.btn__icon-container} [Suggest edit]{.btn__text-container}](https://github.com/OpenOSOrg/openos/edit/main/content/contributing/fix.ipynb "Suggest edit"){.btn .btn-sm .btn-source-edit-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
- [[ ]{.btn__icon-container} [Open issue]{.btn__text-container}](https://github.com/OpenOSOrg/openos/issues/new?title=Issue%20on%20page%20%2Fcontributing/fix.html&body=Your%20issue%20content%20here. "Open an issue"){.btn .btn-sm .btn-source-issues-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
  :::

::: {.dropdown .dropdown-download-buttons}

- [[ ]{.btn__icon-container} [.ipynb]{.btn__text-container}](../_sources/contributing/fix.ipynb "Download source file"){.btn .btn-sm .btn-download-source-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}

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

# Out of date

::: {#print-main-content}
::: {#jb-print-toc}

<div>

## Contents

</div>

- [34.7.1. Set Up](#set-up){.reference .internal .nav-link}
- [34.7.2. Set Up](#cont-contr-tutorial){.reference .internal .nav-link}
- [34.7.3. Create Your Image](#create-your-image){.reference .internal .nav-link}
- [34.7.4. Build Your Book](#build-your-book){.reference .internal .nav-link}
- [34.7.5. Design choices](#design-choices){.reference .internal .nav-link}
  - [34.7.5.1. RISE presentations.](#rise-presentations){.reference .internal .nav-link}
    - [34.7.5.1.1. Developing one](#developing-one){.reference .internal .nav-link}
    - [34.7.5.1.2. Coverting google slide presentation](#coverting-google-slide-presentation){.reference .internal .nav-link}
    - [34.7.5.1.3. Running one](#running-one){.reference .internal .nav-link}
      :::
      :::
      :::

::: {#searchbox}
:::

::: {#out-of-date .section .tex2jax_ignore .mathjax_ignore}

# [34.7. ] {.section-number}Out of date[\#](#out-of-date "Link to this heading") {.headerlink}

::: {.admonition .warning}
Warning

Everything in this chapter is very out of date... FIXME
:::

::: {#set-up .section}

## [34.7.1. ] {.section-number}Set Up[\#](#set-up "Link to this heading") {.headerlink}

You will want to create your own forked repository from the [openos repository](https://github.com/OpenOSOrg/openos){.reference .external} . If you already have your own container/environment used to build and publish the book, then you can clone your forked repository there and skip the image creation section. Otherwise, clone it locally.

::: {.admonition .note}
Note

There are three important folders that you will use: /containers, /content, /books. The containers folder will hold all of the configuration and the Dockerfile for your docker image. The content folder will hold all of the .ipynb files plus additiional files used to structure your book. The books folder contains the makefile to build and publish your book from the content folder.
:::
:::

::: {#cont-contr-tutorial .section}
[]{#id1}

## [34.7.2. ] {.section-number}Set Up[\#](#cont-contr-tutorial "Link to this heading") {.headerlink}

You will want to create your own forked repository from the [openos repository](https://github.com/OpenOSOrg/openos){.reference .external} . If you already have your own container/environment used to build and publish the book, then you can clone your forked repository there and skip the image creation section. Otherwise, clone it locally.

::: {.admonition .note}
Note

There are three important folders that you will use: /containers, /content, /books. The containers folder will hold all of the configuration and the Dockerfile for your docker image. The content folder will hold all of the .ipynb files plus additiional files used to structure your book. The books folder contains the makefile to build and publish your book from the content folder.
:::
:::

::: {#create-your-image .section}

## [34.7.3. ] {.section-number}Create Your Image[\#](#create-your-image "Link to this heading") {.headerlink}

Navigate to the /containers/container/base folder. This is where you can make any modifications to your image. Navigate back to /containers/container and type "make build" to build your image. This will take around 10-15 minutes, so make sure you have no syntax errors. Type "make publish" to publish to your image registry.

::: {.admonition .warning}
Warning

You will need to have the Docker daemon running in the background to build your image.
:::
:::

::: {#build-your-book .section}

## [34.7.4. ] {.section-number}Build Your Book[\#](#build-your-book "Link to this heading") {.headerlink}

Navigate to the /content folder. Here is where all of your book content will be stored. Please visit the [Jupyter Book website](https://jupyterbook.org/en/stable/intro.html){.reference .external} to see a more detailed description of book format and markup syntax.

Once your book is ready, In your container environment, navigate to /books/textbook and type "make build" to build the textbook. It will create a \_build folder in the same directory containing all of the static assets needed for the website. Type "make pub" to publish to your GitHub Pages site.

Note that you are publishing the book to your forked repository's GitHub Pages site. If you are happy with your changes, commit them and submit a pull request to add your changes to the original repository.
:::

::: {#design-choices .section}
[]{#cont-contr-design}

## [34.7.5. ] {.section-number}Design choices[\#](#design-choices "Link to this heading") {.headerlink}

- All real content is in the "content" directory

  - textbook_toc.yml - the table of contents for the book
- The images (png, jpg, etc) should all be in their respective section folder in the images directory
- The quizzes should all be in the quizzes directory
- The source code being shown/ran should all be in the src directory
- We are creating one subdirectory for each chapter that will contain:

  - book materials; for now, its a single file for book; likely will eventually break into sections
  - all corresponding lectures, referred to as lecture notes
  - all corresponding lab materials

::: {#rise-presentations .section}

### [34.7.5.1. ] {.section-number}RISE presentations.[\#](#rise-presentations "Link to this heading") {.headerlink}

::: {#developing-one .section}

#### [34.7.5.1.1. ] {.section-number}Developing one[\#](#developing-one "Link to this heading") {.headerlink}

- you can find an example with templates for slides in the "content/contributing" directory under L01-example notebook.
- you should create a symbolic link to the lecture note css file (content/css/ln.css) with the name of your slide (e.g., L01-example), and commit it to the repo
- to determin which cells are slides, versus notes, versus subslides... edit the tags
  :::

::: {#coverting-google-slide-presentation .section}

#### [34.7.5.1.2. ] {.section-number}Coverting google slide presentation[\#](#coverting-google-slide-presentation "Link to this heading") {.headerlink}

- download google slidedeck as a powerpoint
- open powerpoint in keynote
- export to images,

  - set to do an image for each stage of animations
  - make sure png and transpartent backgrounds
  - upload to book directory "content/from-google-slides"

    - create new subdirectory (e.g., MM01)
    - upload all images generated into that directory
    - in directory, e.g., mm, type `{code-block} ../python/mkln MM-L1 ../from-google-slides/MM01 `{.docutils .literal .notranslate}
    - you should now have a rise presentation titled MM-L1, where each image is a seperate slide
      :::

::: {#running-one .section}

#### [34.7.5.1.3. ] {.section-number}Running one[\#](#running-one "Link to this heading") {.headerlink}

- press lower case "t", in screen show for speaker notes; my experience is that only works if you start the note before going to full screen on the slide
  :::
  :::
  :::
  :::

::: prev-next-area
[](resources.html "previous page"){.left-prev}

::: prev-next-info
previous

[34.6. ]{.section-number}Resources to look at
:::

[](../misc/bib.html "next page"){.right-next}

::: prev-next-info
next

[35. ]{.section-number}Bibliography
:::
:::
:::

::: {.bd-sidebar-secondary .bd-toc}
::: {.sidebar-secondary-items .sidebar-secondary__inner}
::: sidebar-secondary-item
::: {.page-toc .tocsection .onthispage}
Contents
:::

- [34.7.1. Set Up](#set-up){.reference .internal .nav-link}
- [34.7.2. Set Up](#cont-contr-tutorial){.reference .internal .nav-link}
- [34.7.3. Create Your Image](#create-your-image){.reference .internal .nav-link}
- [34.7.4. Build Your Book](#build-your-book){.reference .internal .nav-link}
- [34.7.5. Design choices](#design-choices){.reference .internal .nav-link}
  - [34.7.5.1. RISE presentations.](#rise-presentations){.reference .internal .nav-link}
    - [34.7.5.1.1. Developing one](#developing-one){.reference .internal .nav-link}
    - [34.7.5.1.2. Coverting google slide presentation](#coverting-google-slide-presentation){.reference .internal .nav-link}
    - [34.7.5.1.3. Running one](#running-one){.reference .internal .nav-link}
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
