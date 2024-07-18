---
docsearch:language: en
lang: en
title: 5.5. Testing --- Introduction to Operating Systems
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
    -   [5.3. Editors](tools-editors.html){.reference .internal}
    -   [5.4. Make](tools-make.html){.reference .internal}
    -   [5.5. Testing](#){.current .reference .internal}
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

-   [[ ![JupyterHub logo](../_static/images/logo_jupyterhub.svg) ]{.btn__icon-container} [JupyterHub]{.btn__text-container}](https://jupyterhub-opf-jupyterhub.apps.smaug.na.operate-first.cloud/hub/user-redirect/git-pull?repo=https%3A//github.com/OpenOSOrg/openos&urlpath=lab/tree/openos/content/intro/tools-testing.ipynb&branch=main "Launch on JupyterHub"){.btn .btn-sm .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
:::

::: {.dropdown .dropdown-source-buttons}

-   [[ ]{.btn__icon-container} [Repository]{.btn__text-container}](https://github.com/OpenOSOrg/openos "Source repository"){.btn .btn-sm .btn-source-repository-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
-   [[ ]{.btn__icon-container} [Suggest edit]{.btn__text-container}](https://github.com/OpenOSOrg/openos/edit/main/content/intro/tools-testing.ipynb "Suggest edit"){.btn .btn-sm .btn-source-edit-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
-   [[ ]{.btn__icon-container} [Open issue]{.btn__text-container}](https://github.com/OpenOSOrg/openos/issues/new?title=Issue%20on%20page%20%2Fintro/tools-testing.html&body=Your%20issue%20content%20here. "Open an issue"){.btn .btn-sm .btn-source-issues-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
:::

::: {.dropdown .dropdown-download-buttons}

-   [[ ]{.btn__icon-container} [.ipynb]{.btn__text-container}](../_sources/intro/tools-testing.ipynb "Download source file"){.btn .btn-sm .btn-download-source-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
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
# Testing

::: {#print-main-content}
::: {#jb-print-toc}
<div>

## Contents

</div>

-   [5.5.1. Unit Tests](#unit-tests){.reference .internal .nav-link}
-   [5.5.2. Integration Tests](#integration-tests){.reference .internal .nav-link}
:::
:::
:::

::: {#searchbox}
:::

::: {.cell .tag_remove-input .docutils .container}
:::

::: {#testing .section .tex2jax_ignore .mathjax_ignore}
[]{#cont-gs-tools-testing}

# [5.5. ]{.section-number}Testing[\#](#testing "Link to this heading"){.headerlink}

Most students try to solve the complicated programs for this course by implementing them, and then manually testing their program. This is, possible...., but incredibly challenging. Proper unit and integration tests will, on the other hand, save you an enormous number of hours in this course.

::: {#unit-tests .section}
## [5.5.1. ]{.section-number}Unit Tests[\#](#unit-tests "Link to this heading"){.headerlink}

As you develop your program, you are going to write many individual functions. For each, think about how to write simple tests to see if the function does what you expect it to. For example, one of the assignments we often hand out is a user level thread scheduler. To get it to work, you need to set up the stack of the thread properly so that when the thread completes it calls a routine to exit. If you write a simple test at the beginning to test what happens after a thread completes, it will take a few minutes to identify and fix any bugs. Many students, instead, spend hours trying to identify the problem manually when they have a running scheduler, with timer interrupts causing threads to switch between themselves.

Lets see some simple examples, we have already shown a script that runs a set of test programs ([[Listing 5.1]{.std .std-numref}](tools-shell.html#run-tests){.reference .internal}), and a makefile ([[Listing 5.2]{.std .std-numref}](tools-make.html#make-parser){.reference .internal})to invoke that script on a parser. The first step on developing a parser is to define its interface, and a set of tests against that interface. To do this, we define the data structures and functions that the parser will expose to its clients in a header file shown in [[Listing 5.3]{.std .std-numref}](#myshell-parser-h){.reference .internal}.

::: {#myshell-parser-h .literal-block-wrapper .docutils .container}
::: code-block-caption
[Listing 5.3 ]{.caption-number}[Header file for parser for shell]{.caption-text}[\#](#myshell-parser-h "Link to this code"){.headerlink}
:::

::: {.highlight-default .notranslate}
::: highlight
     1#ifndef MYSHELL_PARSER_H
     2#define MYSHELL_PARSER_H
     3#include <stdbool.h>
     4
     5#define MAX_LINE_LENGTH 512
     6#define MAX_ARGV_LENGTH (MAX_LINE_LENGTH / 2 + 1)
     7
     8struct pipeline_command {
     9  char *command_args[MAX_ARGV_LENGTH]; // arg[0] is command, rest are arguments
    10  char *redirect_in_path;  // NULL or Name of file to redirect in from 
    11  char *redirect_out_path; // NULL or Name of a file to redirect out to
    12  struct pipeline_command *next; // next command in the pipeline. NULL if done 
    13};
    14
    15struct pipeline {
    16  struct pipeline_command *commands; // first command
    17  bool is_background; // TRUE if should execue in background
    18};
    19
    20void pipeline_free(struct pipeline *pipeline);
    21
    22struct pipeline *pipeline_build(const char *command_line);
    23
    24#endif /* MYSHELL_PARSER_H */
:::
:::
:::

In this header file, we define everything that test programs, and eventually the shell will need to use to call the parser we will develop. The routines `pipeline_build`{.docutils .literal .notranslate} returns a `pipeline`{.docutils .literal .notranslate} struct with a flag that indicates if the whole pipleline is in the background, and points to a linked list of `pipeline_commands`{.docutils .literal .notranslate}. Each `pipeline_command`{.docutils .literal .notranslate} contains a boolean indicates if the command is in the background, and an array where the first element is the command and the other elements are arguments to that command. Our first implementation of `myshell_parser.c`{.docutils .literal .notranslate} (see [[Listing 5.4]{.std .std-numref}](#myshell-parser-c){.reference .internal}) simply returns error messages.

::: {#myshell-parser-c .literal-block-wrapper .docutils .container}
::: code-block-caption
[Listing 5.4 ]{.caption-number}[Initial implementation of]{.caption-text}[\#](#myshell-parser-c "Link to this code"){.headerlink}
:::

::: {.highlight-default .notranslate}
::: highlight
     1#include "myshell_parser.h"
     2#include "stddef.h"
     3
     4struct pipeline *pipeline_build(const char *command_line)
     5{
     6 // TODO: Implement this function
     7 return NULL;
     8}
     9
    10void pipeline_free(struct pipeline *pipeline)
    11{
    12 // TODO: Implement this function
    13}
:::
:::
:::

Before implementing any functionality we write tests on what we expect a correct implementation to do. For example, [[Listing 5.5]{.std .std-numref}](#test-simple-input-c){.reference .internal} shows a test that calls the parser `pipeline_build`{.docutils .literal .notranslate} with a single command `ls`{.docutils .literal .notranslate}, asserts what it expects the state of a correct execution of the parser is.

::: {#test-simple-input-c .literal-block-wrapper .docutils .container}
::: code-block-caption
[Listing 5.5 ]{.caption-number}[Test of a simple]{.caption-text}[\#](#test-simple-input-c "Link to this code"){.headerlink}
:::

::: {.highlight-c .notranslate}
::: highlight
     1#include "myshell_parser.h"
     2#include <stdio.h>
     3#include <stdlib.h>
     4#include <string.h>
     5#include <assert.h>
     6
     7int
     8main(void)
     9{
    10  struct pipeline* my_pipeline = pipeline_build("ls\n");
    11  
    12  // Test that a pipeline was returned
    13  assert(my_pipeline != NULL);
    14  assert(!my_pipeline->is_background);
    15  assert(my_pipeline->commands != NULL);
    16  
    17  // Test the parsed args
    18  assert(strcmp("ls", my_pipeline->commands->command_args[0]) == 0);
    19  assert(my_pipeline->commands->command_args[1] == NULL);
    20  
    21  // Test the redirect state
    22  assert(my_pipeline->commands->redirect_in_path == NULL);
    23  assert(my_pipeline->commands->redirect_out_path == NULL);
    24  
    25  // Test that there is only one parsed command in the pipeline
    26  assert(my_pipeline->commands->next == NULL);
    27  
    28  pipeline_free(my_pipeline);
    29}
:::
:::
:::

As another example, [[Listing 5.6]{.std .std-numref}](#test-simple-pipe-c){.reference .internal} runs a simple example of two commands with a pipe between them.

::: {#test-simple-pipe-c .literal-block-wrapper .docutils .container}
::: code-block-caption
[Listing 5.6 ]{.caption-number}[Test of a simple pipe]{.caption-text}[\#](#test-simple-pipe-c "Link to this code"){.headerlink}
:::

::: {.highlight-c .notranslate}
::: highlight
     1#include "myshell_parser.h"
     2#include <stdio.h>
     3#include <stdlib.h>
     4#include <string.h>
     5#include <assert.h>
     6
     7int
     8main(void)
     9{
    10  struct pipeline* my_pipeline = pipeline_build("ls | cat\n");
    11  
    12  // Test that a pipeline was returned
    13  assert(my_pipeline != NULL);
    14  assert(!my_pipeline->is_background);
    15  assert(my_pipeline->commands != NULL);
    16  
    17  // Test the parsed args
    18  assert(strcmp("ls", my_pipeline->commands->command_args[0]) == 0);
    19  assert(my_pipeline->commands->command_args[1] == NULL);
    20  
    21  // Test the redirect state
    22  assert(my_pipeline->commands->redirect_in_path == NULL);
    23  assert(my_pipeline->commands->redirect_out_path == NULL);
    24  
    25  // Test that there are multiple parsed command in the pipeline
    26  assert(my_pipeline->commands->next != NULL);
    27  
    28  // keep going... what should we be testign next?
    29  pipeline_free(my_pipeline);
    30}
:::
:::
:::

We have already provided examples of how you can invoke the unit test programs from a shell scripts ([[Listing 5.1]{.std .std-numref}](tools-shell.html#run-tests){.reference .internal}), and shown how that can in turn by automatically invoked by make ([[Listing 5.2]{.std .std-numref}](tools-make.html#make-parser){.reference .internal}) so that every time you make a change the makefile will automatically re-run all the tests. Now, given the above test files, if we type make with that makefile, the `all`{.docutils .literal .notranslate} rule will run the `check`{.docutils .literal .notranslate} rule which will recompile any required software and then invoke the shell script to run all the tests. In our case, both test programs assert because the pipeline returned is `NULL`{.docutils .literal .notranslate}.

::: {.cell .tag_remove-input .docutils .container}
::: {.cell_output .docutils .container}
:::
:::

Unit tests are specific to the particular interfaces of the functions you write. We expect students to write their own unit tests, since the internal functions of their application are up to them to design. For the parser, we have defined the functions that we want you to implement, so that we can give you some example of unit tests. However, we would recommend that a good parser implementation should start by implementing a lexer, that converts each syntactical element of the input into a set of tokens. If you do that, you should add the new interface to the `.h`{.docutils .literal .notranslate} file and new tests to make sure that your lexing functionality works.

You should never delete your tests. For example, the parser will eventually become the first shell assignment for many courses based on this book. You will keep adding new functionality, and as you do, you will find that you will find bugs in your parser. If your makefile doesn't keep running all the old tests, you are very likely to be introducing bugs...
:::

::: {#integration-tests .section}
## [5.5.2. ]{.section-number}Integration Tests[\#](#integration-tests "Link to this heading"){.headerlink}

Integration tests use the public interfaces end-to-end. For example, the tests we run with gradescope to automatically test if your programs are correct are all integration tests. We hope you will share your integration tests with the class, and in the BU version of the course, we will often add tests provided by students to the test suite we use in gradescope; the best way you can have tests you know you will pass is to contribute tests to us. In many cases, you can write integration tests in the same we described above, but calling the public interfaces of libraries. If the task is to develop a program, you can use, for example, shell scripts, with the output redirected to a file, to run tests, compare the result to an expect result, and raise an error if the results do not agree with the expected ones.
:::
:::

::: prev-next-area
[](tools-make.html "previous page"){.left-prev}

::: prev-next-info
previous

[5.4. ]{.section-number}Make
:::

[](tools-git.html "next page"){.right-next}

::: prev-next-info
next

[5.6. ]{.section-number}Git Basics
:::
:::
:::

::: {.bd-sidebar-secondary .bd-toc}
::: {.sidebar-secondary-items .sidebar-secondary__inner}
::: sidebar-secondary-item
::: {.page-toc .tocsection .onthispage}
Contents
:::

-   [5.5.1. Unit Tests](#unit-tests){.reference .internal .nav-link}
-   [5.5.2. Integration Tests](#integration-tests){.reference .internal .nav-link}
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
