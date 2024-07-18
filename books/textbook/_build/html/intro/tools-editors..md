---
docsearch:language: en
lang: en
title: 5.3. Editors --- Introduction to Operating Systems
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
[![Introduction to Operating Systems - Home](../_static/logo.png){.logo__image .only-light}](pref.html){.navbar-brand .logo}
:::

::: sidebar-primary-item
:::

::: sidebar-primary-item
::: {.bd-toc-item .navbar-nav .active}
-   [Preface](pref.html){.reference .internal}

[Getting started]{.caption-text}

-   [1. Introduction](intro.html){.reference .internal}
-   [2. Purpose of operating systems](purpose.html){.reference .internal}
-   [3. Operating System Structure & Unix/Linux](structure.html){.reference .internal}
-   [4. Operating System Abstractions](abstractions.html){.reference .internal}
-   [5. What you should know](tools.html){.reference .internal}
    []{.toctree-toggle role="presentation"}
    -   [5.1. The C Programming Language](tools-c.html){.reference .internal}
    -   [5.2. Shell](tools-shell.html){.reference .internal}
    -   [5.3. Editors](#){.current .reference .internal}
    -   [5.4. Make](tools-make.html){.reference .internal}
    -   [5.5. Testing](tools-testing.html){.reference .internal}
    -   [5.6. Git Basics](tools-git.html){.reference .internal}
    -   [5.7. GDB](tools-gdb.html){.reference .internal}

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

-   [24. Introduction](../sync/sync.html){.reference .internal}
-   [25. Basic Synchronization](../sync/basic.html){.reference .internal}
    []{.toctree-toggle role="presentation"}
    -   [25.1. Cooperating Processes and Inter-process Communication](../sync/sharing.html){.reference .internal}
    -   [25.2. The Critical Section Problem](../sync/criticalsection.html){.reference .internal}
    -   [25.3. Implementing Locks](../sync/locks.html){.reference .internal}
    -   [25.4. Ordering Thread Events](../sync/ordering.html){.reference .internal}
-   [26. Common Concurrency Bugs](../sync/concurrency_bugs.html){.reference .internal}
-   [27. Advanced Synchronization](../sync/advanced.html){.reference .internal}
    []{.toctree-toggle role="presentation"}
    -   [27.1. Read-Dominated Workloads](../sync/readmostly.html){.reference .internal}
    -   [27.2. Challenges of Modern Hardware](../sync/hardware_challenges.html){.reference .internal}
    -   [27.3. Locking in the Linux Kernel](../sync/linux_locking.html){.reference .internal}
-   [28. Review](../sync/review.html){.reference .internal}

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

-   [[ ![JupyterHub logo](../_static/images/logo_jupyterhub.svg) ]{.btn__icon-container} [JupyterHub]{.btn__text-container}](https://jupyterhub-opf-jupyterhub.apps.smaug.na.operate-first.cloud/hub/user-redirect/git-pull?repo=https%3A//github.com/OpenOSOrg/openos&urlpath=lab/tree/openos/content/intro/tools-editors.ipynb&branch=main "Launch on JupyterHub"){.btn .btn-sm .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
:::

::: {.dropdown .dropdown-source-buttons}

-   [[ ]{.btn__icon-container} [Repository]{.btn__text-container}](https://github.com/OpenOSOrg/openos "Source repository"){.btn .btn-sm .btn-source-repository-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
-   [[ ]{.btn__icon-container} [Suggest edit]{.btn__text-container}](https://github.com/OpenOSOrg/openos/edit/main/content/intro/tools-editors.ipynb "Suggest edit"){.btn .btn-sm .btn-source-edit-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
-   [[ ]{.btn__icon-container} [Open issue]{.btn__text-container}](https://github.com/OpenOSOrg/openos/issues/new?title=Issue%20on%20page%20%2Fintro/tools-editors.html&body=Your%20issue%20content%20here. "Open an issue"){.btn .btn-sm .btn-source-issues-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
:::

::: {.dropdown .dropdown-download-buttons}

-   [[ ]{.btn__icon-container} [.ipynb]{.btn__text-container}](../_sources/intro/tools-editors.ipynb "Download source file"){.btn .btn-sm .btn-download-source-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
-   [ ]{.btn__icon-container} [.pdf]{.btn__text-container}
:::

[ ]{.btn__icon-container}
:::
:::
:::
:::
:::

::: {#jb-print-docs-body .onlyprint}
# Editors

::: {#print-main-content}
::: {#jb-print-toc}
:::
:::
:::

::: {#searchbox}
:::

::: {#editors .section .tex2jax_ignore .mathjax_ignore}
[]{#cont-gs-tools-editors}

# [5.3. ]{.section-number}Editors[\#](#editors "Link to this heading"){.headerlink}

The vast majority of OS developers use text based editors, that can be accessed from a terminal, by using ssh to get to a machine, and over a wide variety of connections. The two most popular options are [vim](https://en.wikipedia.org/wiki/Vim_(text_editor)){.reference .external} and [emacs](https://en.wikipedia.org/wiki/Emacs){.reference .external}, which are both available in the container image provided with this book. While the choice of which is better is [the oldest rivalry in computing](https://slate.com/technology/2014/05/oldest-software-rivalry-emacs-and-vi-two-text-editors-used-by-programmers.html){.reference .external}[[\[]{.fn-bracket}1[\]]{.fn-bracket}](#googlesearch){#id1 .footnote-reference .brackets role="doc-noteref"}, the author of this section feels comfortable asserting that it is a self-evident truth that you will be more productive, get a better grade, and probably become a better person if you master emacs (and anyone from the "cult of vi" that touches this chapter puts their soul at risk[[\[]{.fn-bracket}2[\]]{.fn-bracket}](#religion){#id2 .footnote-reference .brackets role="doc-noteref"}).

With vim (the most popular variant of vi today), most users use it to modify a file, and then exit vim when they want to compile, debug or run their programs. To open a file, type `vim <filename>`{.docutils .literal .notranslate}. When you enter vim, you will automatically be in `normal mode`{.docutils .literal .notranslate} where you can navigate using your cursor. To insert text, type `i`{.docutils .literal .notranslate} to enter `insert mode`{.docutils .literal .notranslate}. or 'a' to enter 'append mode'. when you are done changes, press the `esc`{.docutils .literal .notranslate} key to enter normal mode, next press `:`{.docutils .literal .notranslate} to enter `command mode`{.docutils .literal .notranslate}, lastly press `w`{.docutils .literal .notranslate} (for write) and enter to save. To quit, enter command mode and `q`{.docutils .literal .notranslate} (quit). There is also an incredibly arcane command set that enables members of the "cult of vi" to do very complex operations with a few key strokes, but if you spend your time learning that you will probably not have any time left to do OS assignments.

Now that we have discussed everything you ever need to know about vim, lets talk about the better alternative. While you could use emacs to just edit files, power users live in emacs and use to to compile, debug, and run their programs. To open a file in emacs, type `emacs <filename>`{.docutils .literal .notranslate}, or if you are in emacs already (which you should always be) type `<ctrl>-x <ctrl>-f`{.docutils .literal .notranslate} to open a file. Unlike in VIM, you will immediately be able to write in/edit the file. Once you are finished editing, type `<ctrl>-s`{.docutils .literal .notranslate} to save the file. When you want to leave (which you never should) you type `<ctrl>-x`{.docutils .literal .notranslate} followed by `<ctrl>-c`{.docutils .literal .notranslate} to exit. There are many control and escape sequences to do powerful things and a really good reference card is available [here](https://www.gnu.org/software/emacs/refcards/pdf/refcard.pdf){.reference .external}.

Getting help:

You can use `<ctrl>-h`{.docutils .literal .notranslate} to get to get help, where `<ctrl>-h ?`{.docutils .literal .notranslate} gives you all the options, and `<ctrl>-h t`{.docutils .literal .notranslate} starts an emacs tutorial. For example, depending on the type of file you are editing, emacs goes into a file specific *mode* and will have special bindings for that that mode. If you want to understand it, `<ctrl>-h m`{.docutils .literal .notranslate} tells you about the mode and `<ctrl>-h b`{.docutils .literal .notranslate} tells you the key bindings.

A few of the more powerful features that you should take advance of in emacs are:

-   Type `<ctrl>-x <ctrl>-f`{.docutils .literal .notranslate} to open a directory, where emacs will let you move around the filesystem while staying in the editor.

-   Starting up a [shell](https://www.gnu.org/software/emacs/manual/html_node/efaq-w32/Using-shell.html#:~:text=You%20can%20start%20an%20interactive,to%20use%20as%20the%20shell.){.reference .external} which enables you to copy content easily from other buffers in emacs to the shell, and run programs directly there.

-   Running [make within emacs](https://www.gnu.org/software/emacs/manual/html_node/emacs/Compilation.html){.reference .external}. When you do this emacs parses the error messages, and hitting `<ctrl>-x <backquote>`{.docutils .literal .notranslate} will automatically pop you into the right file on the line where the compiler emitted an error.

-   Run [debugger from within emacs](https://www.gnu.org/software/emacs/manual/html_node/emacs/Debuggers.html){.reference .external} (`<esc>-x gdb`{.docutils .literal .notranslate}). When you do this, emacs parses the output of gdb, and automatically pops you into the correct source code file where the code you are debugging lives.

-   Run [grep in emacs](https://www.gnu.org/software/emacs/manual/html_node/emacs/Grep-Searching.html){.reference .external} (`<esc>-x grep`{.docutils .literal .notranslate}) where emacs parses the result, and hitting `<ctrl>-x <backquote>`{.docutils .literal .notranslate} will automatically pop you into the right file on the line where grep returned a result.

These are just a few of the very powerful ways that emacs will improve your life as a software developer (and likely you a a person). While it is a steep learning curve, you will find after a while that your fingers know all the common keystrokes, and you productivity will increase exponentially.

::: {.admonition .warning}
Warning

One danger all real emacs users face eventually is Carpal tunnel syndrome, strongly recommend you rebind the caps locks key to be the control key.
:::

------------------------------------------------------------------------

[[\[]{.fn-bracket}[1](#id1){role="doc-backlink"}[\]]{.fn-bracket}]{.label}

Try doing a google search for `emacs`{.docutils .literal .notranslate} and then do one for `vi`{.docutils .literal .notranslate}.

[[\[]{.fn-bracket}[2](#id2){role="doc-backlink"}[\]]{.fn-bracket}]{.label}

All true believers in the church of emacs consider vi (the predecessor to vim) as the editor of the beast (vi-vi-vi being 666 in roman numerals).
:::

::: prev-next-area
[](tools-shell.html "previous page"){.left-prev}

::: prev-next-info
previous

[5.2. ]{.section-number}Shell
:::

[](tools-make.html "next page"){.right-next}

::: prev-next-info
next

[5.4. ]{.section-number}Make
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
