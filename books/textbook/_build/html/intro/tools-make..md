---
docsearch:language: en
lang: en
title: 5.4. Make --- Introduction to Operating Systems
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
    -   [5.4. Make](#){.current .reference .internal}
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

-   [[ ![JupyterHub logo](../_static/images/logo_jupyterhub.svg) ]{.btn__icon-container} [JupyterHub]{.btn__text-container}](https://jupyterhub-opf-jupyterhub.apps.smaug.na.operate-first.cloud/hub/user-redirect/git-pull?repo=https%3A//github.com/OpenOSOrg/openos&urlpath=lab/tree/openos/content/intro/tools-make.ipynb&branch=main "Launch on JupyterHub"){.btn .btn-sm .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
:::

::: {.dropdown .dropdown-source-buttons}

-   [[ ]{.btn__icon-container} [Repository]{.btn__text-container}](https://github.com/OpenOSOrg/openos "Source repository"){.btn .btn-sm .btn-source-repository-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
-   [[ ]{.btn__icon-container} [Suggest edit]{.btn__text-container}](https://github.com/OpenOSOrg/openos/edit/main/content/intro/tools-make.ipynb "Suggest edit"){.btn .btn-sm .btn-source-edit-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
-   [[ ]{.btn__icon-container} [Open issue]{.btn__text-container}](https://github.com/OpenOSOrg/openos/issues/new?title=Issue%20on%20page%20%2Fintro/tools-make.html&body=Your%20issue%20content%20here. "Open an issue"){.btn .btn-sm .btn-source-issues-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
:::

::: {.dropdown .dropdown-download-buttons}

-   [[ ]{.btn__icon-container} [.ipynb]{.btn__text-container}](../_sources/intro/tools-make.ipynb "Download source file"){.btn .btn-sm .btn-download-source-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
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
# Make

::: {#print-main-content}
::: {#jb-print-toc}
<div>

## Contents

</div>

-   [5.4.1. Motivation](#motivation){.reference .internal .nav-link}
-   [5.4.2. A simple example](#a-simple-example){.reference .internal .nav-link}
-   [5.4.3. Summary](#summary){.reference .internal .nav-link}
:::
:::
:::

::: {#searchbox}
:::

::: {.cell .tag_remove-input .docutils .container}
:::

::: {#make .section .tex2jax_ignore .mathjax_ignore}
[]{#cont-gs-tools-make}

# [5.4. ]{.section-number}Make[\#](#make "Link to this heading"){.headerlink}

Make is a critical tool to let developers automate compiling complicated programs. After motivating why you want to do master it, we provide an example makefile and demonstrate a bit of the power of this tool.

::: {#motivation .section}
## [5.4.1. ]{.section-number}Motivation[\#](#motivation "Link to this heading"){.headerlink}

For very simple programs, you can use [[emacs]{.std .std-ref}](tools-editors.html#cont-gs-tools-editors){.reference .internal} to write them in a single file and can compile them into executables to be run using, for example, the GNU C compiler gcc:

`gcc filename.c -o filename`{.docutils .literal .notranslate}

That's fine for little programs, although even there, there are lots of flags that you will want to use to compile a program that are not the default with gcc. For example, we would recommend that you always use the following flags:

-   `-Wall`{.docutils .literal .notranslate}: turns on many compiler warning flags; about 90% of the simple bugs that students make are caught by gcc at compile time which emits warnings to ask you if you **really** want to shoot yourself in the foot. Please believe us, if there is a warning, it is much faster to fix it instead of finding the bug at run time later.

-   `-Werror`{.docutils .literal .notranslate}: turns warnings into compilation errors. This is super valuable so that you don't miss the warning; again don't come to a TF for help unless your program compiles with -Wall and -Werror.

-   `-std=gnu99`{.docutils .literal .notranslate}: this isn't super critical, but gcc supports a variety of standard variants of the c programming language, so you might as well use a standard that will ensure that your program is compilable by other compielrs.

-   `-O0`{.docutils .literal .notranslate}: sets optimization level to 0. The compiler supports a wide set of [optimizations](https://gcc.gnu.org/onlinedocs/gcc/Optimize-Options.html){.reference .external} for size, for performance... and for the final program, you might want to specify something different. However, optimizations re-arrange the code, copying functions into other functions. If you want to debug the program you wrote, use `-O0`{.docutils .literal .notranslate}, if you want to debug a program that is logically the same, but doesn't really look like the software you wrote, use something else.

-   `-g`{.docutils .literal .notranslate}: adds debugging symbols to executable. Without this, you are pretty much out of luck if you want to use a [[debugger]{.std .std-ref}](tools-gdb.html#cont-gs-tools-gdb){.reference .internal}, and if you are not using a debugger, then you might as well give up on the projects associated with this course.

-   `-I.`{.docutils .literal .notranslate}: specifies directory where header files can be found (in this example, the working directory `.`{.docutils .literal .notranslate}). You should always seperate key information that describe the interfaces of your program and constants that you might want to change into header files. This flag tells the compiler where those header files are.

Okay, so now, to compiler your simple program, you will type:

`gcc -Wall -Werror -std=gnu99 -O0 -g -I. filename.c -o filename`{.docutils .literal .notranslate}

That's a bit of a pain. How do you know if you remembered to do all that? How do you know how you compiled the program if you come back a day later, or prove to the TF of the course that you used the right flags. More importantly, what happens when you have more than a toy program that can be written in a single file? You won't write any programs for this course that could be written in a single file. How do you remember which files you modified that need to be re-compiled? If you have a header file which 10 `.c`{.docutils .literal .notranslate} files depend on, how to you make sure that all 10 `.c`{.docutils .literal .notranslate} files are re-compiled?

Make and Tab; a sad story:

Make was originally written by [Stuart Feldman](https://en.wikipedia.org/wiki/Stuart_Feldman){.reference .external}, a researcher at bell labs who worked with the team that developed the first version of Unix. One of the painful features of Make is that it uses before each line that specifies an action; a constant source of error since in a text editor it is hard to see the difference between a `<TAB>`{.docutils .literal .notranslate} and a set of spaces. From personal conversation, the reason for this is that Stu hacked together the first version over a weekend and had problems getting other patterns to work with [`lex`{.docutils .literal .notranslate}](https://en.wikipedia.org/wiki/Lex_(software)){.reference .external} which was new at the time. Make was so useful that within a few weeks Stu had 12 users, and even though he knew that `<tab>`{.docutils .literal .notranslate} in column 1 was a bad idea, he didn't want to disrupt his user base. Stu formally apologized when he was honored by ACM as the author of Make for the tens of millions of developers this decision has caused pain to over the years.

That's where make comes in. You create a `makefile`{.docutils .literal .notranslate} that describes the relationships between the files in your program and provides commands for updating each file. Usually for c programs, the executable file is updated from object files (`.o`{.docutils .literal .notranslate} files), which are in turn made by compiling source files (`.c`{.docutils .literal .notranslate} files). Once you have written your makefile, you can just run the shell command `make`{.docutils .literal .notranslate} and it will perform all necessary recompilations. `make`{.docutils .literal .notranslate} knows which files need to be updated based on the last-modification times of the files. You can also provide command line arguments to make to specify which files should be recompiled and how.

We expect you to have at least a basic understanding of how Make works. The version of make provided in the container image for this course is GNU Make. It has many rich features and default rules; for example, it understands that if you want to generate a `.o`{.docutils .literal .notranslate} file from a `.c`{.docutils .literal .notranslate} file, it should use the compiler. You can find extensive details [here](https://www.gnu.org/software/make/manual/html_node/Rules.html){.reference .external} to write makefile rules.
:::

::: {#a-simple-example .section}
## [5.4.2. ]{.section-number}A simple example[\#](#a-simple-example "Link to this heading"){.headerlink}

Here is a simple example that you should understand that is used for a parser that will for many of you be the first assignment of this course.

::: {#make-parser .literal-block-wrapper .docutils .container}
::: code-block-caption
[Listing 5.2 ]{.caption-number}[A Makefile to build a parser]{.caption-text}[\#](#make-parser "Link to this code"){.headerlink}
:::

::: {.highlight-make .notranslate}
::: highlight
     1override CFLAGS := -std=gnu99 -O0 -Wall -Werror -g  -fsanitize=undefined $(CFLAGS) -I.
     2override LDFLAGS := -fsanitize=undefined -fsanitize=leak $(LDLAGS)  
     3CC = gcc
     4
     5# I generally make the first rule run all the tests
     6all: check
     7
     8# rule for making the parser.o  that is needed by all the test programs
     9myshell_parser.o: myshell_parser.c myshell_parser.h
    10
    11
    12# each of the test files depend on their own .c and myshell_parser.h
    13test_simple_input.o: test_simple_input.c myshell_parser.h
    14test_simple_pipe.o: test_simple_pipe.c myshell_parser.h
    15
    16# each of the test programs executables are generated by combining the generated .o with the parser.o
    17test_simple_input : test_simple_input.o myshell_parser.o
    18test_simple_pipe : test_simple_pipe.o myshell_parser.o
    19
    20# Add any additional tests here
    21test_files=./test_simple_input ./test_simple_pipe
    22
    23.PHONY: clean check checkprogs all
    24
    25# Build all of the test program
    26checkprogs: $(test_files)
    27
    28check: checkprogs
    29 /bin/bash run_tests.sh $(test_files)
    30
    31clean:
    32 rm -f *~ *.o $(test_files) $(test_o_files)
:::
:::
:::

This makefile is used to generate and run a set of [[unit tests]{.std .std-ref}](tools-testing.html#cont-gs-tools-testing){.reference .internal} against a parser who's implementation is in `myshell_parser.c`{.docutils .literal .notranslate} where functions implemented by that parser are defined in `myshell_parser.h`{.docutils .literal .notranslate}.

Let's break down each line and rule. In the first line, we specify the flags we want to use to compile C files by assigning a value to CFLAGS (more on implicit variables like CFLAGS [here](https://www.gnu.org/software/make/manual/html_node/Implicit-Variables.html){.reference .external}). The `override`{.docutils .literal .notranslate} directive just makes sure you use the assignments in the makefile even if the variable has previously been set with a command argument. The argument `-fsanitize=undefined`{.docutils .literal .notranslate} to the compiler (CFLAGS) and linker (LDFLAGS) tells gcc to add additional sanitizer run time checks for undefined behavior.

The third line tells Make to use `gcc`{.docutils .literal .notranslate} as the compiler. The first rule `all`{.docutils .literal .notranslate} in this case is run by default. Here we are telling Make to run the rule `check`{.docutils .literal .notranslate} whenever make is run without any arguments. If, on the other hand, you type `make clean`{.docutils .literal .notranslate} it will run the rule on line 30 that will remove all the generated files.

Line 9 defines the rule to create the `myshell_parser.o`{.docutils .literal .notranslate} file that will be linked into all the test programs. It tells make that it should regenerate `myshell_parser.o`{.docutils .literal .notranslate} if either the corresponding `.c`{.docutils .literal .notranslate} file or `.h`{.docutils .literal .notranslate} file changes. Make has a set of implicit rules, where if no recipe is specified, Make understands that it needs to run a compiler to create a `.o`{.docutils .literal .notranslate} file from a `.c`{.docutils .literal .notranslate} file. There are many of these implicit rules as described [here](https://www.gnu.org/software/make/manual/html_node/Catalogue-of-Rules.html#Catalogue-of-Rules){.reference .external}.

Lines 13 and 14 similarly indicates that the test programs depend not only on the corresponding `.c`{.docutils .literal .notranslate} file, but also on `myshell_parser.h`{.docutils .literal .notranslate}. That way, if you edit `myshell_parser.h`{.docutils .literal .notranslate} all the test programs that depend on a prototype you define in that header file will be recompiled. Lines 16 and 17 tell make that the test file depend on both the corresponding `.c`{.docutils .literal .notranslate} file and `myshell_parser.o`{.docutils .literal .notranslate}, and Make knows that it needs to link both `.o`{.docutils .literal .notranslate} files together to create an executable.

Line 20 specifies the list of test programs you are generated, which is used in line 24 that defines the rule checkprogs to generate those test programs, and Line 26 that defines the rule to run the run_tests script we showed before ([[Listing 5.1]{.std .std-numref}](tools-shell.html#run-tests){.reference .internal}) to run all the tests. Line 22, which is not strictly necessary, tells Make that it is really not creating files called clean, check, checkprogs and all.

Note, this makefile could be greatly simplified by using a set of built-in variables Make supports (see [here](https://www.gnu.org/software/make/manual/html_node/Automatic-Variables.html){.reference .external}). For example:

-   `$+`{.docutils .literal .notranslate} inserts all dependencies of the rule

-   `$@`{.docutils .literal .notranslate} inserts the rule's target

You normally don't use make clean, but its useful when you want to, for example, commit your changes to the repository to make sure that new files you have recently created are not hiding among a whole bunch of generated files. Its also useful here to illustrate what is happening from a clean directory. So, if you type `make clean`{.docutils .literal .notranslate} and then `make checkprogs`{.docutils .literal .notranslate} {numref}\`make_parser is:

::: {.cell .tag_remove-input .docutils .container}
::: {.cell_output .docutils .container}
:::
:::

If you type `make checkprogs`{.docutils .literal .notranslate} again, since nothing changed, make will not re-compile anything. While this may not seem like a big deal for your small programs, if you are compiling a complex program like an OS kernel, it can save you hours to only compile the programs you really need to. On our case, the second time we type `make checkprogs`{.docutils .literal .notranslate} we get:

::: {.cell .tag_remove-input .docutils .container}
::: {.cell_output .docutils .container}
:::
:::

If you modify `test_simple_input.c`{.docutils .literal .notranslate} make will only re-compile that file and link the corresponding executable. In this case, we can simulate modifying the file by using the unix command `touch`{.docutils .literal .notranslate} to change the modification time:

::: {.cell .tag_remove-input .docutils .container}
::: {.cell_output .docutils .container}
:::
:::

If on the other hand we modify `myshell_parser.c`{.docutils .literal .notranslate} Make understands it needs to re-compile that file and all the executables that link to it.

::: {.cell .tag_remove-input .docutils .container}
::: {.cell_output .docutils .container}
:::
:::

And if `myshell_parser.h`{.docutils .literal .notranslate} is modified, everything that relies on it needs to be re-generated.

::: {.cell .tag_remove-input .docutils .container}
::: {.cell_output .docutils .container}
:::
:::
:::

::: {#summary .section}
## [5.4.3. ]{.section-number}Summary[\#](#summary "Link to this heading"){.headerlink}

If you are writing complicated programs, composed of many files, you need to master make. The example we showed above showed how this one tool enables you to ensure that you always specify the right flags, and ensure that if a file has changed, everything that relies on it will automatically be regenerated. Finally, we have shown how you can automatically run a set of tests everytime you change anything; something we will talk more about [[here]{.std .std-ref}](tools-testing.html#cont-gs-tools-testing){.reference .internal}. For more info on `make`{.docutils .literal .notranslate}, see the [GNU make manual](https://www.gnu.org/software/make/manual/make.html){.reference .external}.
:::
:::

::: prev-next-area
[](tools-editors.html "previous page"){.left-prev}

::: prev-next-info
previous

[5.3. ]{.section-number}Editors
:::

[](tools-testing.html "next page"){.right-next}

::: prev-next-info
next

[5.5. ]{.section-number}Testing
:::
:::
:::

::: {.bd-sidebar-secondary .bd-toc}
::: {.sidebar-secondary-items .sidebar-secondary__inner}
::: sidebar-secondary-item
::: {.page-toc .tocsection .onthispage}
Contents
:::

-   [5.4.1. Motivation](#motivation){.reference .internal .nav-link}
-   [5.4.2. A simple example](#a-simple-example){.reference .internal .nav-link}
-   [5.4.3. Summary](#summary){.reference .internal .nav-link}
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
