---
docsearch:language: en
lang: en
title: 34.1. Examples --- Introduction to Operating Systems
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
  - [34.1. Examples](#){.current .reference .internal}
  - [34.2. Contributors](credit.html){.reference .internal}
  - [34.3. Contributing](Contributing.html){.reference .internal}
  - [34.6. Resources to look at](resources.html){.reference .internal}
  - [34.7. Out of date](fix.html){.reference .internal}
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

- [[ ![JupyterHub logo](../_static/images/logo_jupyterhub.svg) ]{.btn__icon-container} [JupyterHub]{.btn__text-container}](https://jupyterhub-opf-jupyterhub.apps.smaug.na.operate-first.cloud/hub/user-redirect/git-pull?repo=https%3A//github.com/OpenOSOrg/openos&urlpath=lab/tree/openos/content/contributing/examples.ipynb&branch=main "Launch on JupyterHub"){.btn .btn-sm .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
  :::

::: {.dropdown .dropdown-source-buttons}

- [[ ]{.btn__icon-container} [Repository]{.btn__text-container}](https://github.com/OpenOSOrg/openos "Source repository"){.btn .btn-sm .btn-source-repository-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
- [[ ]{.btn__icon-container} [Suggest edit]{.btn__text-container}](https://github.com/OpenOSOrg/openos/edit/main/content/contributing/examples.ipynb "Suggest edit"){.btn .btn-sm .btn-source-edit-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
- [[ ]{.btn__icon-container} [Open issue]{.btn__text-container}](https://github.com/OpenOSOrg/openos/issues/new?title=Issue%20on%20page%20%2Fcontributing/examples.html&body=Your%20issue%20content%20here. "Open an issue"){.btn .btn-sm .btn-source-issues-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
  :::

::: {.dropdown .dropdown-download-buttons}

- [[ ]{.btn__icon-container} [.ipynb]{.btn__text-container}](../_sources/contributing/examples.ipynb "Download source file"){.btn .btn-sm .btn-download-source-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}

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

# Examples

::: {#print-main-content}
::: {#jb-print-toc}

<div>

## Contents

</div>

- [34.1.1. Notes and warnings](#notes-and-warnings){.reference .internal .nav-link}
- [34.1.2. Figures](#figures){.reference .internal .nav-link}
- [34.1.3. Table](#table){.reference .internal .nav-link}
- [34.1.4. Authoring content](#authoring-content){.reference .internal .nav-link}
  - [34.1.4.1. Using jupyterlab](#using-jupyterlab){.reference .internal .nav-link}
  - [34.1.4.2. Adding figures](#adding-figures){.reference .internal .nav-link}
    :::
    :::
    :::

::: {#searchbox}
:::

::: {#examples .section .tex2jax_ignore .mathjax_ignore}

# [34.1. ] {.section-number}Examples[\#](#examples "Link to this heading") {.headerlink}

Starting to re-organize this, to just past in simple examples so there is one place to find them

::: {#notes-and-warnings .section}

## [34.1.1. ] {.section-number}Notes and warnings[\#](#notes-and-warnings "Link to this heading") {.headerlink}

::: {.admonition .note}
Note

We recommend you look at this notebook as the best example of generating content, and we will make a valiant attempt to keep it up to date as we gain more experience. Having said that, the file system chapter today probably has a better set of examples

::: {.admonition .warning}
Warning

It is really easy to waste months with all the degrees of freedom with this authoring model, and we will try to be prescriptive on how we use the tools, so we recommend you jump straight to the [[tutorial]{.std .std-ref}](fix.html#cont-contr-tutorial){.reference .internal} directions on [[authoring]{.std .std-ref}](#cont-contr-authoring){.reference .internal} material.

::: {.admonition .note}
Note

This is an example of a note, in a warning, in a note.
:::
:::
:::

::: {.highlight-default .notranslate}
::: highlight
:::
:::
:::

::: {#figures .section}

## [34.1.2. ] {.section-number}Figures[\#](#figures "Link to this heading") {.headerlink}

As shown in figure [[Fig. 34.1]{.std .std-numref}](#contrib-fig-examp){.reference .internal}, most operating systems today have ...

![[Fig. 34.1 ]{.caption-number}[A caption for figure]{.caption-text}[\#](#contrib-fig-examp "Link to this image"){.headerlink}](../_images/osstructure-1.dio.png){style="width: 50%;"}

For more on figures look at this [reference](https://myst-parser.readthedocs.io/en/latest/syntax/roles-and-directives.html#images-and-figures){.reference .external}.
:::

::: {#table .section}

## [34.1.3. ] {.section-number}Table[\#](#table "Link to this heading") {.headerlink}

::: pst-scrollable-table-container
Value                                                        Binary Prefix   Abbreviation

---

[\\(1024 = 2\^{10}\\)]{.math .notranslate .nohighlight}      kilo            K
[\\(1024\^2 = 2\^{20}\\)]{.math .notranslate .nohighlight}   mega            M
[\\(1024\^3 = 2\^{30}\\)]{.math .notranslate .nohighlight}   giga            G
[\\(1024\^4 = 2\^{40}\\)]{.math .notranslate .nohighlight}   tera            T
[\\(1024\^5 = 2\^{50}\\)]{.math .notranslate .nohighlight}   peta            P
:::

As shown in `ex:table_ref`{.xref .std .std-numref .docutils .literal .notranslate}

::: pst-scrollable-table-container
Function   Reference      Brief Description

---

mmap()     man 2 mmap     Allocates a page of virtual memory
munmap()   man 2 munmap   Deallocates a page of virtual memory
:::

Could use Pandas from [this style guild](https://pandas.pydata.org/docs/user_guide/style.html){.reference .external}

::: {.cell .docutils .container}
::: {.cell_input .docutils .container}
::: {.highlight-ipython3 .notranslate}
::: highlight
import pandas as pd
import numpy as np
import matplotlib as mpl

```
df = pd.DataFrame({
    "strings": ["Adam", "Mike"],
    "ints": [1, 3],
    "floats": [1.123, 1000.23]
})
df.style \
  .format(precision=3, thousands=".", decimal=",") \
  .format_index(str.upper, axis=1) \
  .relabel_index(["row 1", "row 2"], axis=0)
```

:::
:::
:::

::: {.cell_output .docutils .container}
::: {.output .text_html}
        STRINGS   INTS   FLOATS

---

row 1   Adam      1      1,123
row 2   Mike      3      1.000,230
:::
:::
:::

At the end of this section we have links to various [[reference]{.xref .myst}](#cont:contr:ref){.reference .internal} materials, for example, sections of Jonathan's textbook that we plan to steal materials from.
:::

::: {#authoring-content .section}
[]{#cont-contr-authoring}

## [34.1.4. ] {.section-number}Authoring content[\#](#authoring-content "Link to this heading") {.headerlink}

::: {#using-jupyterlab .section}

### [34.1.4.1. ] {.section-number}Using jupyterlab[\#](#using-jupyterlab "Link to this heading") {.headerlink}

Will put various hints here on what we find works, although for the most part like any editor, you will gradually experience what works best for you.

- there seems to be just one file browser, I tend to open multiple links to the textbook:

  1. for the place I am actually authoring
  2. for a browser to move around, look at examples
  3. for the rendered book/result
- we might want to build some simple vidios/todos
  :::

::: {#adding-figures .section}

### [34.1.4.2. ] {.section-number}Adding figures[\#](#adding-figures "Link to this heading") {.headerlink}

Use [draw.io](http://draw.io){.reference .external} for open source software, I download the desktop version from [here](https://www.diagrams.net/%7D){.reference .external} since it seems more reliable. You can just download the image to your desktop, edit it there, and upload it again. You can Please use png as the source type of the file, rather than the default drawio; in this case it will create a XXX.drawio.png file, where the diagram is embedded in the png, so you can both dispay it, and edit it. This means you can not only continue to edit the file directly, but can also include exactly the same file in a figure.

Tricks I have found in using this:

1. with the desktop version you can directly copy images browser see this [vidio](https://www.youtube.com/watch?v=pYROq5Aphoc){.reference .external}
2. I tend to use layers, for animation, then upload it and generate multiple png files form the same image
3. You very much want to export the picture as high-resolution, by using a large zoom, see Figure [[Fig. 34.4]{.std .std-numref}](#contrib-fig-dioex2){.reference .internal}

![[Fig. 34.2 ]{.caption-number}[Making images high resolution.]{.caption-text}[\#](#contrib-fig-dioex3 "Link to this image"){.headerlink}](../_images/draw-io-control-resolution.png){style="width: 60%;"}

If you use the drawio embedded in the notebook environment, to generate a png rather than using the file export from the figure, use the command palette from jupyter "view" menue as shown in figures [[Fig. 34.3]{.std .std-numref}](#contrib-fig-dioex1){.reference .internal} and [[Fig. 34.4]{.std .std-numref}](#contrib-fig-dioex2){.reference .internal}.

![[Fig. 34.3 ]{.caption-number}[Activate Command Palette to export drawio figure as png.]{.caption-text}[\#](#contrib-fig-dioex1 "Link to this image"){.headerlink}](../_images/drawio-export-1.png){style="width: 60%;"}

![[Fig. 34.4 ]{.caption-number}[Export drawio figure as png.]{.caption-text}[\#](#contrib-fig-dioex2 "Link to this image"){.headerlink}](../_images/drawio-export-2.png){style="width: 60%;"}

Note, this is strongly discouraged, since I don't see any way to fix the resolution so that the images don't suck. I end up exporting from [draw.io](http://draw.io){.reference .external} at 500% to get pictures to look reasonable.

We use the figure directive in myst, so the following:

::: {.highlight-default .notranslate}
::: highlight

| ```{figure} ../images/osstructure-1.drawio.png |
| ---------------------------------------------- |
| width: 50%                                     |
| name: fcontrib:fig:examp                       |
| align: right                                   |
| ---                                            |
| A caption for figure                           |
| ```                                            |
| :::                                            |
| :::                                            |

Results in this:
:::
:::
:::

::: prev-next-area
[](intro.html "previous page"){.left-prev}

::: prev-next-info
previous

[34. ]{.section-number}Contributing
:::

[](credit.html "next page"){.right-next}

::: prev-next-info
next

[34.2. ]{.section-number}Contributors
:::
:::
:::

::: {.bd-sidebar-secondary .bd-toc}
::: {.sidebar-secondary-items .sidebar-secondary__inner}
::: sidebar-secondary-item
::: {.page-toc .tocsection .onthispage}
Contents
:::

- [34.1.1. Notes and warnings](#notes-and-warnings){.reference .internal .nav-link}
- [34.1.2. Figures](#figures){.reference .internal .nav-link}
- [34.1.3. Table](#table){.reference .internal .nav-link}
- [34.1.4. Authoring content](#authoring-content){.reference .internal .nav-link}
  - [34.1.4.1. Using jupyterlab](#using-jupyterlab){.reference .internal .nav-link}
  - [34.1.4.2. Adding figures](#adding-figures){.reference .internal .nav-link}
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
