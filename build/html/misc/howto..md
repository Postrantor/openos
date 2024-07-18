---
docsearch:language: en
lang: en
title: 33. How to read this book --- Introduction to Operating Systems
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

- [33. How to read this book](#){.current .reference .internal}
- [34. Contributing](../contributing/intro.html){.reference .internal}
  []{.toctree-toggle role="presentation"}
  - [34.1. Examples](../contributing/examples.html){.reference .internal}
  - [34.2. Contributors](../contributing/credit.html){.reference .internal}
  - [34.3. Contributing](../contributing/Contributing.html){.reference .internal}
  - [34.6. Resources to look at](../contributing/resources.html){.reference .internal}
  - [34.7. Out of date](../contributing/fix.html){.reference .internal}
- [35. Bibliography](bib.html){.reference .internal}
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

- [[ ![JupyterHub logo](../_static/images/logo_jupyterhub.svg) ]{.btn__icon-container} [JupyterHub]{.btn__text-container}](https://jupyterhub-opf-jupyterhub.apps.smaug.na.operate-first.cloud/hub/user-redirect/git-pull?repo=https%3A//github.com/OpenOSOrg/openos&urlpath=lab/tree/openos/content/misc/howto.ipynb&branch=main "Launch on JupyterHub"){.btn .btn-sm .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
  :::

::: {.dropdown .dropdown-source-buttons}

- [[ ]{.btn__icon-container} [Repository]{.btn__text-container}](https://github.com/OpenOSOrg/openos "Source repository"){.btn .btn-sm .btn-source-repository-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
- [[ ]{.btn__icon-container} [Suggest edit]{.btn__text-container}](https://github.com/OpenOSOrg/openos/edit/main/content/misc/howto.ipynb "Suggest edit"){.btn .btn-sm .btn-source-edit-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
- [[ ]{.btn__icon-container} [Open issue]{.btn__text-container}](https://github.com/OpenOSOrg/openos/issues/new?title=Issue%20on%20page%20%2Fmisc/howto.html&body=Your%20issue%20content%20here. "Open an issue"){.btn .btn-sm .btn-source-issues-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
  :::

::: {.dropdown .dropdown-download-buttons}

- [[ ]{.btn__icon-container} [.ipynb]{.btn__text-container}](../_sources/misc/howto.ipynb "Download source file"){.btn .btn-sm .btn-download-source-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}

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

# How to read this book

::: {#print-main-content}
::: {#jb-print-toc}

<div>

## Contents

</div>

- [33.1. Browser compatibility](#browser-compatibility){.reference .internal .nav-link}
- [33.2. Opening an issue](#opening-an-issue){.reference .internal .nav-link}
- [33.3. WARNING -- DANGER](#warning-danger){.reference .internal .nav-link}
- [33.4. Step 0: Start your server](#step-0-start-your-server){.reference .internal .nav-link}
  - [33.4.1. BU Server startup](#bu-server-startup){.reference .internal .nav-link}
  - [33.4.2. Booting your server](#booting-your-server){.reference .internal .nav-link}
- [33.5. UNIX Terminal Environment](#unix-terminal-environment){.reference .internal .nav-link}
  - [33.5.1. Creating Terminals](#creating-terminals){.reference .internal .nav-link}
  - [33.5.2. Closing Terminals](#closing-terminals){.reference .internal .nav-link}
- [33.6. UNIX Terminal Environment "Lifetime"](#unix-terminal-environment-lifetime){.reference .internal .nav-link}
  - [33.6.1. WARNING](#warning){.reference .internal .nav-link}
- [33.7. Shutting Down Your Server](#shutting-down-your-server){.reference .internal .nav-link}
  - [33.7.1. Hub Control Panel](#hub-control-panel){.reference .internal .nav-link}
  - [33.7.2. Shutdown](#shutdown){.reference .internal .nav-link}
    :::
    :::
    :::

::: {#searchbox}
:::

::: {#how-to-read-this-book .section .tex2jax_ignore .mathjax_ignore}
[]{#misc-howto}

# [33. ] {.section-number}How to read this book[\#](#how-to-read-this-book "Link to this heading") {.headerlink}

This book has been designed so that you can actively engage with the material. We have constructed an online environment that you can login to from your browser. Once you have logged in you can then start a "server" that you can then access in your browser. This server is identical to the server that was used to author the content of the book and has all the software required for the examples and more.

In general we recommend that you read the book at a computer with a mouse and keyboard so that you can follow along with the examples. Below we will walk you though a typical session of work with the book.[[\[]{.fn-bracket}1[\]]{.fn-bracket}](#credja){#id1 .footnote-reference .brackets role="doc-noteref"}

::: {#browser-compatibility .section}

## [33.1. ] {.section-number}Browser compatibility[\#](#browser-compatibility "Link to this heading") {.headerlink}

The author recommends using the [Google Chrome](https://www.google.com/chrome/){.reference .external} browser but most of the content should work with most browsers. If you run into issues please open an issue and the try switching browsers to see if this solves your problem.
:::

::: {#opening-an-issue .section}
[]{#misc-howto-issue}

## [33.2. ] {.section-number}Opening an issue[\#](#opening-an-issue "Link to this heading") {.headerlink}

Towards the top at the top right hand side of the page you will see a few icons. Putting your mouse over the git icon will reveal a dropdown. Select "open issue" and follow the instructions. Be sure to state what browser you were using and what the problem was. If possible include a screenshot.

Thanks!
:::

::: {#warning-danger .section}

## [33.3. ] {.section-number}WARNING -- DANGER[\#](#warning-danger "Link to this heading") {.headerlink}

> <div>
>
> **The files you create within your Linux server are NOT PERMANENT!** In other words you cannot rely on the files to be there if the server crashes for some reason, it gets shutdown due to inactivity, or you purposefully shut it down. Every time you make a change to your code you are expected to save your work to your github repo.
>
> </div>

:::

::: {#step-0-start-your-server .section}

## [33.4. ] {.section-number}Step 0: Start your server[\#](#step-0-start-your-server "Link to this heading") {.headerlink}

If you are in a BU class that is using this book, follow this link:

- [https://rhods-dashboard-redhat-ods-applications.apps.prod2023.zkf1.p1.openshiftapps. com/notebookController/spawner](https://rhods-dashboard-redhat-ods-applications.apps.prod2023.zkf1.p1.openshiftapps.com/notebookController/spawner){target="_blank" rel="noopener noreferrerhttps"}

::: {#bu-server-startup .section}

### [33.4.1. ] {.section-number}BU Server startup[\#](#bu-server-startup "Link to this heading") {.headerlink}

Clicking on the above link should take you to the following page:

![](../images/howto/howto0.png)

Clicking \"Login with OpenShift\". This will take you to the page displayed below.

![](../images/howto/howto0.1.png)

Click \"GoogleBU\". This will take you to the following login page.

![](../images/howto/howto0.2.png)

Enter your BU username and password and then click \"Continue\". This may then redirect you to BU\'s two factor authentication service as shown below

![](../images/howto/howto0.3.png)

Select your choice of authentication mechanism. If you are not able to login try again using an [\"incognito\" browser window\"](https://support.google.com/chrome/answer/95464?hl=en&co=GENIE.Platform%3DDesktop). If you still cannot login and you are sure you are in a class that is using the book please contact the teaching staff and they will add your BU user to the service.
:::

::: {#booting-your-server .section}

### [33.4.2. ] {.section-number}Booting your server[\#](#booting-your-server "Link to this heading") {.headerlink}

After login you should be presented with the following panel. You will need to:

1. Select the right "Notebook Image" ("UCSLS UNIX Environment" or "Under the Covers: The Secret Life of Software"),
2. Select "Start server in current tab", and then
3. click on the "Start Server" button.

![](../images/howto/howto1.png)

You then should observe the following sequence progress as your server starts up

+------------------------------------------------------------------------------+------------------------------------------------------------------------------+------------------------------------------------------------------------------+
| ::: {style="padding: 0; margin: 0 0 0 0;"}                                   | ::: {style="padding: 0; margin: 0 0 0 0;"}                                   | ::: {style="padding: 0; margin: 0 0 0 0;"}                                   |
| ![](../images/howto/howto2.png){width="100%" style="padding: 0; margin: 0;"} | ![](../images/howto/howto3.png){width="100%" style="padding: 0; margin: 0;"} | ![](../images/howto/howto4.png){width="100%" style="padding: 0; margin: 0;"} |
| :::                                                                          | :::                                                                          | :::                                                                          |
+------------------------------------------------------------------------------+------------------------------------------------------------------------------+------------------------------------------------------------------------------+

At this point you may be presented again with the following login page on which you should again select "GoogleBU".

![](../images/howto/howto4.1.png)
:::
:::

::: {#unix-terminal-environment .section}

## [33.5. ] {.section-number}UNIX Terminal Environment[\#](#unix-terminal-environment "Link to this heading") {.headerlink}

After the boot process you should be presented with the UNIX terminal environment that we will be using as illustrated below.

![](../images/howto/howto5.png)

\>

::: {#creating-terminals .section}

### [33.5.1. ] {.section-number}Creating Terminals[\#](#creating-terminals "Link to this heading") {.headerlink}

![](../images/howto/howto6.png)

Use the "File" menu to select "New" then "Terminal". This should start a Terminal as shown below:

![](../images/howto/howto7.png)

Using the "File-\>New-\>Terminal" menu option again lets you create more terminals. Each terminal will have its own tab as shown below.

![](../images/howto/howto7.1.png)

You can create and organize as many terminals as you like. Dragging the "Terminal" tab title bar around will allow you to adjust the layout. For example, below we have started three terminals and organized them in two rows -- two on the first row and one on the second.

![](../images/howto/howto8.png)
:::

::: {#closing-terminals .section}

### [33.5.2. ] {.section-number}Closing Terminals[\#](#closing-terminals "Link to this heading") {.headerlink}

To close a terminal simply click the "x" in the terminal's tab title bar.
:::
:::

::: {#unix-terminal-environment-lifetime .section}

## [33.6. ] {.section-number}UNIX Terminal Environment "Lifetime"[\#](#unix-terminal-environment-lifetime "Link to this heading") {.headerlink}

Your UNIX terminal environment is temporary. It will automatically be destroyed. This will happen:

1. After a period of inactivity
2. 12 hours after you started it

Rather than letting the system destroy your environment arbitrarily it is best for you to shut it down yourself when you are done your work, see below.

::: {#warning .section}

### [33.6.1. ] {.section-number}WARNING[\#](#warning "Link to this heading") {.headerlink}

Given the temporary nature of the environment you should be aware that **ANY FILES YOU HAVE WITHIN IT WILL BE DESTROYED** when it shuts down. When you start a new one it will reset to a fresh clean state.

This is intentional; you are expected to commit your work frequently back to github classroom along with a message explaining your commit. **Your history of commits is something you are expected to be able to explain when reviewing your homework assignment.**
:::
:::

::: {#shutting-down-your-server .section}

## [33.7. ] {.section-number}Shutting Down Your Server[\#](#shutting-down-your-server "Link to this heading") {.headerlink}

**When you have finished your session of working it is important that you shutdown your server.** To shutdown the server select the "Hub Control" feature from the "File" menu as illustrated below

![](../images/howto/howto10.png)

::: {#hub-control-panel .section}

### [33.7.1. ] {.section-number}Hub Control Panel[\#](#hub-control-panel "Link to this heading") {.headerlink}

This will open a new tab or window with following page:

![](../images/howto/howto11.png)

This may present you with a confirmation panel. Click "Stop server" to confirm.

![](../images/howto/howto11.1.png)
:::

::: {#shutdown .section}

### [33.7.2. ] {.section-number}Shutdown[\#](#shutdown "Link to this heading") {.headerlink}

At this point the browser tab or window that you used for your work session will no longer be valid, see below, and you can safely close it.

![](../images/howto/howto13.png)

---

[[\[]{.fn-bracket}[1](#id1){role="doc-backlink"}[\]]{.fn-bracket}]{.label}

This material comes from jonathan's systems book [here](https://jappavoo.github.io/UndertheCovers/textbook/howto.html#how-to-read-this-book){.reference .external}, but we expect minor tweaks to creep in as we gain experience with the OS class and eventually we will be pointing to different images, etc...
:::
:::
:::

::: prev-next-area
[](../sec/sec.html "previous page"){.left-prev}

::: prev-next-info
previous

[32. ]{.section-number}Security
:::

[](../contributing/intro.html "next page"){.right-next}

::: prev-next-info
next

[34. ]{.section-number}Contributing
:::
:::
:::

::: {.bd-sidebar-secondary .bd-toc}
::: {.sidebar-secondary-items .sidebar-secondary__inner}
::: sidebar-secondary-item
::: {.page-toc .tocsection .onthispage}
Contents
:::

- [33.1. Browser compatibility](#browser-compatibility){.reference .internal .nav-link}
- [33.2. Opening an issue](#opening-an-issue){.reference .internal .nav-link}
- [33.3. WARNING -- DANGER](#warning-danger){.reference .internal .nav-link}
- [33.4. Step 0: Start your server](#step-0-start-your-server){.reference .internal .nav-link}
  - [33.4.1. BU Server startup](#bu-server-startup){.reference .internal .nav-link}
  - [33.4.2. Booting your server](#booting-your-server){.reference .internal .nav-link}
- [33.5. UNIX Terminal Environment](#unix-terminal-environment){.reference .internal .nav-link}
  - [33.5.1. Creating Terminals](#creating-terminals){.reference .internal .nav-link}
  - [33.5.2. Closing Terminals](#closing-terminals){.reference .internal .nav-link}
- [33.6. UNIX Terminal Environment "Lifetime"](#unix-terminal-environment-lifetime){.reference .internal .nav-link}
  - [33.6.1. WARNING](#warning){.reference .internal .nav-link}
- [33.7. Shutting Down Your Server](#shutting-down-your-server){.reference .internal .nav-link}
  - [33.7.1. Hub Control Panel](#hub-control-panel){.reference .internal .nav-link}
  - [33.7.2. Shutdown](#shutdown){.reference .internal .nav-link}
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
