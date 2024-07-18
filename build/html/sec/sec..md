---
docsearch:language: en
lang: en
title: 32. Security --- Introduction to Operating Systems
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
- [32. Security](#){.current .reference .internal}

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

- [[ ![JupyterHub logo](../_static/images/logo_jupyterhub.svg) ]{.btn__icon-container} [JupyterHub]{.btn__text-container}](https://jupyterhub-opf-jupyterhub.apps.smaug.na.operate-first.cloud/hub/user-redirect/git-pull?repo=https%3A//github.com/OpenOSOrg/openos&urlpath=lab/tree/openos/content/sec/sec.ipynb&branch=main "Launch on JupyterHub"){.btn .btn-sm .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
  :::

::: {.dropdown .dropdown-source-buttons}

- [[ ]{.btn__icon-container} [Repository]{.btn__text-container}](https://github.com/OpenOSOrg/openos "Source repository"){.btn .btn-sm .btn-source-repository-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
- [[ ]{.btn__icon-container} [Suggest edit]{.btn__text-container}](https://github.com/OpenOSOrg/openos/edit/main/content/sec/sec.ipynb "Suggest edit"){.btn .btn-sm .btn-source-edit-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
- [[ ]{.btn__icon-container} [Open issue]{.btn__text-container}](https://github.com/OpenOSOrg/openos/issues/new?title=Issue%20on%20page%20%2Fsec/sec.html&body=Your%20issue%20content%20here. "Open an issue"){.btn .btn-sm .btn-source-issues-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}
  :::

::: {.dropdown .dropdown-download-buttons}

- [[ ]{.btn__icon-container} [.ipynb]{.btn__text-container}](../_sources/sec/sec.ipynb "Download source file"){.btn .btn-sm .btn-download-source-button .dropdown-item target="_blank" bs-placement="left" bs-toggle="tooltip"}

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

# Security

::: {#print-main-content}
::: {#jb-print-toc}

<div>

## Contents

</div>

- [32.1. Protection](#protection){.reference .internal .nav-link}
  - [32.1.1. Identity and Authentication](#identity-and-authentication){.reference .internal .nav-link}
  - [32.1.2. Checking passwords](#checking-passwords){.reference .internal .nav-link}
  - [32.1.3. Centralized authentication - LDAP and Kerberos](#centralized-authentication-ldap-and-kerberos){.reference .internal .nav-link}
- [32.2. Unix Access Control](#unix-access-control){.reference .internal .nav-link}
  - [32.2.1. Limitations of Unix permissions](#limitations-of-unix-permissions){.reference .internal .nav-link}
  - [32.2.2. Access Control Lists](#access-control-lists){.reference .internal .nav-link}
  - [32.2.3. Access Control List Examples](#access-control-list-examples){.reference .internal .nav-link}
  - [32.2.4. Other Privileged Operations](#other-privileged-operations){.reference .internal .nav-link}
- [32.3. SELinux](#selinux){.reference .internal .nav-link}
  - [32.3.1. Control of Information Flow](#control-of-information-flow){.reference .internal .nav-link}
    - [32.3.1.1. Review Questions](#review-questions){.reference .internal .nav-link}
- [32.4. Attacks --- Stack Overflow](#attacks-stack-overflow){.reference .internal .nav-link}
  - [32.4.1. Security - SQL Injection](#security-sql-injection){.reference .internal .nav-link}
  - [32.4.2. SSL and Connection Security](#ssl-and-connection-security){.reference .internal .nav-link}
    :::
    :::
    :::

::: {#searchbox}
:::

::: {#security .section .tex2jax_ignore .mathjax_ignore}

# [32. ] {.section-number}Security[\#](#security "Link to this heading") {.headerlink}

The term computer security covers a number of areas and goals. Most of them fall under the following categories:

- Confidentiality of data. As a user of a computer system, this allows you to prevent others from accessing information which you wish to keep private, such as email or passwords.
- Confidentiality of actions. This lets you prevent others from observing what programs you run and what files or external resources you access.
- Integrity of data. Your data will not be modified or deleted without your permission.
- Integrity of operations. Commands should do what they are supposed to do. For example, when you type ls you should get a directory listing, rather than a script that sends your passwords to a secret website in Russia.
- Availability. A system will not stop running when you need it to be operational.

With the rise of the Internet, security has become a much broader field, much of it related to either networking or the behavior of applications such as web browsers. This chapter will cover operating system features which enable computer security, and which reduce the risks from security flaws in application software; the field of computing security is much larger, however[[\[]{.fn-bracket}1[\]]{.fn-bracket}](#id10){#id1 .footnote-reference .brackets role="doc-noteref"}.

::: {#protection .section}

## [32.1. ] {.section-number}Protection[\#](#protection "Link to this heading") {.headerlink}

Much of security involves protection: deciding whether or not to allow an operation based on a series of rules. The purpose of protection is to ensure the security goals described above, by applying these rules to computing operations, allowing some operations and forbiding others. (This is not sufficient for full security, as seen in the discussion below of software vulnerabilities, but it helps.) These rules are typically based on a simple model, of actors, objects, and actions:

- Actors. These perform the actions. At the lowest level these are almost always processes, but they are typically identified by a text or numeric user ID, which is typically associated with either an actual person or a system service.
- Objects. These are the things which are being protected: usually files or directories, but sometimes processes, special devices, configurations, or other aspects of the system which can be modified.
- Actions. These are performed on objects. The most common actions are read and write, but others can include creating and deleting files, killing a process, or rebooting the system.

The goal of the operating system's protection or *access control* mechanisms is to express and enforce policies which determine whether a particular combination of an actor performing an action on an object is to be allowed or denied.

::: {#identity-and-authentication .section}

### [32.1.1. ] {.section-number}Identity and Authentication[\#](#identity-and-authentication "Link to this heading") {.headerlink}

In a Unix-like operating system, the actual actors are processes, which perform actions by issuing system calls. However specifying rules based on the processes themselves---e.g. process 10 may access file `"/home/pjd"`{.docutils .literal .notranslate}---will not work, because processes are created dynamically: rules could only be made for processes in existence at that time, and not for ones created in the future.

The solution used in almost all operating systems today is the concept of *user identity*: every process is associated with a user identity (e.g. a user name and ID in Unix) and rules are specified in terms of these identities. In its simplest form each of these identities is a login name associated with an individual person, and rules for that identity are used to permit or restrict access by that person[[\[]{.fn-bracket}2[\]]{.fn-bracket}](#id11){#id2 .footnote-reference .brackets role="doc-noteref"}. User identity is inherited through the `fork`{.docutils .literal .notranslate} system call, so that actions taken by a process either directly or indirectly (through children of that process) are bound by the same rules. Access rules specify actors in terms of these identities, and every process is associated with one of these identities, allowing a fixed mapping from identities to permissions.

These authentication mechanisms are frequently called *factors*; hence the term *multi-factor authentication*, where more than one factor (e.g. password, text message) are used. The Wikipedia entry on "Multi-factor authentication" is a good introduction.

In practice this requires a login process, or *authentication*, in which an external user proves that she has the right to take on a certain identity. Thus, the person Jane Smith may be given the right to use the operating system identity named `smith.j`{.docutils .literal .notranslate}, after *authenticating* that identity to the system by providing the correct password. Authentication is an important part of operating system security, as it forms the link between the higher-level goals of system administration (e.g. Jane is allowed to access *file.txt*, but Joe isn't) and the operating system-level features which implement this control.

Most authentication mechanisms can be classified as one of three types, based on the type of verification provided by the user:

1. *Something you know*: e.g. a password. This is the most common form of authentication, due to ease of implementation.
2. *Something you have*: like a key to a lock, an RSA SecurID token, etc. More complicated to administer, but more difficult for an adversary to obtain.
3. *Something you are*: often biometric data, such as a fingerprint.

You have undoubtedly used many password-authenticated processes; in addition you may have used other methods such as a SecureID token or fingerprint scanner. There are advantages and disadvantages to each type of authentication; however this class focuses on passwords as they are the most widely used.
:::

::: {#checking-passwords .section}

### [32.1.2. ] {.section-number}Checking passwords[\#](#checking-passwords "Link to this heading") {.headerlink}

Securely storing and checking passwords is difficult, and various methods have been used over the years. The primary alternatives are as follows.

**Unencrypted file**: Passwords are stored In an unencrypted file, only accessible to the operating system or a privileged user, and a simple string compare is used to verify a user-entered password. Although in principle this should be secure, the result of any error or failure is catastrophic. (This issue is particularly problematic since people typically re-use passwords across systems.)

**Hashed password file**: Passwords are put through a one-way cryptographic hash function[[\[]{.fn-bracket}3[\]]{.fn-bracket}](#id12){#id3 .footnote-reference .brackets role="doc-noteref"} before being stored. User-entered passwords are hashed by the same algorithm and compared with the stored password hash; if the two match, then the password is correct. Early UNIX systems used this mechanism, and made the password file publicly-readable, as the same file held other information (e.g. mapping between numeric user ID and text username) used by many unprivileged programs. (e.g. the **ls -l** command would need this mapping to show file ownership.) This was considered fairly secure on slow (and especially non-networked) machines, due to the length of time required to crack an individual password by *brute force*---i.e. trying all possible combinations until the correct password was found. However the discovery of *dictionary attacks* changed this, however.

A dictionary attack is based on the idea that in most cases breaking into *any* account is almost as good as breaking a particular account, and takes advantage of the fact that on shared machines (e.g. **[login.ccs.neu.edu](http://login.ccs.neu.edu){.reference .external}**) there are a large number of user accounts, increasing the chance of breaking into one of them. The attack consists of calculating the hash for every word in a dictionary[[\[]{.fn-bracket}4[\]]{.fn-bracket}](#id13){#id4 .footnote-reference .brackets role="doc-noteref"}, and then comparing this list with the hashes in the password file; if *any* of the accounts has a password in this list, the attack succeeds. (a more sophisticated attack, using pre-computed *rainbow tables*[[\[]{.fn-bracket}5[\]]{.fn-bracket}](#id14){#id5 .footnote-reference .brackets role="doc-noteref"} is able to crack individual hashed passwords very quickly, as well.)

**Password "salt"**: This is a variation on hashed passwords---when a password is stored, a random string S is chosen (for unknown reasons called the *salt*) and appended to the password before hashing ; the stored value is then \[S, hash(S+password)\]. Verifying a password is straightforward: the salt value is read from the password file and appended to the input password before it is hashed and compared. This protects against attacks which require pre-computed tables (e.g. dictionary and rainbow table attacks), as now tables would be needed for every possible salt value. (in early usage this was 12 bits long; in modern systems it is 32 bits or more.)

As machines (especially GPUs) become faster and faster, even this method has become less secure over time, as it is becoming feasible for attackers to evaluate billions of possible passwords per second. Counter-measures include making the hash function slower (e.g. running the password through the hash function 5000 times), and protecting the password file against public access, just like was done with early plain-text password files. (this is done in Linux--- `/etc/passwd`{.docutils .literal .notranslate} contains username and UID information, and is publicly readable, while `/etc/shadow`{.docutils .literal .notranslate} contains password hashes and is protected.

::: {#shadowpw .literal-block-wrapper .docutils .container}
::: code-block-caption
[Listing 32.1 ]{.caption-number}[Password and shadow password files in Linux]{.caption-text}[\#](#shadowpw "Link to this code"){.headerlink}
:::

::: {.highlight-default .notranslate}
::: highlight
pjd@cs5600-vbox:~$ ls -l /etc/shadow /etc/passwd
-rw-r--r-- 1 root root   1061 Aug 24  2013 /etc/passwd
-rw-r----- 1 root shadow  867 Aug 24  2013 /etc/shadow
pjd@cs5600-vbox:~$ tail -2 /etc/passwd
student:x:1000:1000:A,,,:/home/student:/bin/bash
pjd:x:1001:1001:Peter Desnoyers,,,:/home/pjd:/bin/bash
pjd@cs5600-vbox:~$ sudo tail -2 /etc/shadow
student:$6$JjiTdyS2$cvbtxgVxMwMI5fL0If5Dc90JRuds9yolCKGHc/52ET1tLwksji/
SN05pksqdwACztcvhIyCDRfAt9lrK133WA/:15935:0:99999:7:::
pjd:$6$wz5.BTqz$RXkmlCnbb0aoA7C67zf2zL7FokmdKLoc51MLdn7jcDe/JMHzs7iePBC
NEy7O7ZGbVFIl4wTEbi5a8yhhQALnd1:15941:0:99999:7:::
:::
:::
:::

**Challenge-response**: This is another variation on password checking, although it is typically used over a network rather than for direct login. In this case the server must keep the password in clear text; when a client requests authentication, the server sends a *challenge*---a random string---which the client adds to the password before hashing it and sending the result back to the server. In this way an attacker with access to the network is unable to learn the password, and (if the server never repeats challenges) is unable to replay previous responses.
:::

::: {#centralized-authentication-ldap-and-kerberos .section}

### [32.1.3. ] {.section-number}Centralized authentication - LDAP and Kerberos[\#](#centralized-authentication-ldap-and-kerberos "Link to this heading") {.headerlink}

Modern computer systems frequently use centralized password administration: for instance, when you log in to a CCIS workstation your password is not checked locally, but rather against a central authentication server. The most common used mechanisms are LDAP and Kerberos, frequently used as part of Microsoft's Active Directory service. LDAP (lightweight directory access protocol) is a general-purpose directory protocol that can store information about people, machines, and just about anything else that a computer might want to name; an example entry is shown in [[Listing 32.2]{.std .std-numref}](#fig-ldap){.reference .internal}.

::: {#fig-ldap .literal-block-wrapper .docutils .container}
::: code-block-caption
[Listing 32.2 ]{.caption-number}[Typical CCIS LDAP entry]{.caption-text}[\#](#fig-ldap "Link to this code"){.headerlink}
:::

::: {.highlight-default .notranslate}
::: highlight
# pjd, people, ccs.neu.edu
dn: uid=pjd,ou=people,dc=ccs,dc=neu,dc=edu
displayName: Peter J. Desnoyers
cn: pjd
loginShell: /bin/bash
uidNumber: 11415
gidNumber: 65100
sn: Desnoyers
homeDirectory: /home/pjd
mail: pjd@ccs.neu.edumailto:pjd@ccs.neu.edu
givenName: Peter
...
:::
:::
:::

One of the attributes an LDAP entry can have is a password: a client can log in to the LDAP server by specifying this password, which will be checked by the server. A Linux or other system will use an LDAP server for authentication by attempting to login with the credentials supplied by the user; if this succeeds, then the local login is successful and user information (such as shell and home directory) is retrieved from the server[[\[]{.fn-bracket}6[\]]{.fn-bracket}](#id15){#id6 .footnote-reference .brackets role="doc-noteref"}.

Kerberos is a more general-purpose authentication mechanism that allows a server to supply unforgeable cryptographically-signed tickets. These allow untrusted machines, like personal computers, to securely access network services, such as a file server while only having to authenticate once, to the Kerberos server; after this initial authentication, the Kerberos tickets can be used for authentication without having to request additional passwords from the user.
:::
:::

::: {#unix-access-control .section}

## [32.2. ] {.section-number}Unix Access Control[\#](#unix-access-control "Link to this heading") {.headerlink}

Basic security in an operating system is performed by access control: the process of determining whether each OS action will be allowed, based on the actor (determined by information like a user ID), the specific object (e.g. a file), and object permissions. The desired operation can be described by an access control matrix, such as this one or four users, 3 files and 1 directory:

::: pst-scrollable-table-container
file1        file2        dir1         file3

---

user1                read                      read/write
user2   read         read         read/write   read
user3   read         read
user4   read/write   read/write

: [Table 32.1 ]{.caption-number}[Simple access matrix (again)]{.caption-text}[\#](#fig-sec-simple "Link to this table"){.headerlink}
:::

To be more specific, the Unix security model has the following parts:

**Actors**: Users. User identity (and file ownership) is described by two IDs:

1. User id (`uid`{.docutils .literal .notranslate})
2. Group id (`gid`{.docutils .literal .notranslate})

In addition there are permissions for *world*---i.e. any user.

**Objects**: Files and directories.

**Actions:** On files: *read*, *write*, and *execute* (i.e. run as a program). Directories: *list* (as in `ls`{.docutils .literal .notranslate}), *traverse* - i.e. accessing the file `/a/b/c`{.docutils .literal .notranslate} requires traversing the directories `/a`{.docutils .literal .notranslate} and `/a/b`{.docutils .literal .notranslate}, and *modify* - i.e. creating, deleting, or renaming files (or directories) within that directory. (note that list, traverse, and modify are encoded as read, execute, and write permissions)

Users may belong to more than one group: as an example, user pjd belongs to groups faculty, cs5600 and sssl, as shown here by the id command:

::: {#id19 .literal-block-wrapper .docutils .container}
::: code-block-caption
[Listing 32.3 ]{.caption-number}[Id command output]{.caption-text}[\#](#id19 "Link to this code"){.headerlink}
:::

::: {.highlight-default .notranslate}
::: highlight
pjd@login:~$ id pjd
uid=11415(pjd) gid=65100(faculty) groups=1254(cs5600),1294(sssl),65100(faculty)
:::
:::
:::

Files and directories have an owner and a group, and three sets of permissions: one for the file owner, one for members of its group, and one for world, with the permissions typically encoded in a single string, as shown in [[Fig. 32.1]{.std .std-numref}](#fig-sec-lsdashl){.reference .internal}.

![[Fig. 32.1 ]{.caption-number}[Interpreting file ownership and permissions]{.caption-text}[\#](#fig-sec-lsdashl "Link to this image"){.headerlink}](../_images/security-fig1.png){style="width: 70%;"}

Finally, (a) only the owner of a file may change its permissions, and (b) each user may belong to some number of groups. (typically up to 32)

Permissions are interpreted as follows:

::: {#id20 .literal-block-wrapper .docutils .container}
::: code-block-caption
[Listing 32.4 ]{.caption-number}[File access algorithm]{.caption-text}[\#](#id20 "Link to this code"){.headerlink}
:::

::: {.highlight-default .notranslate}
::: highlight
check(process, action, file):
if process.uid = file.uid:
if action in file.perm.owner
allow
else deny
if process.gid = file.gid:
if action in file.perm.group
allow
else deny
if action in file.perm.world:
allow
else deny
:::
:::
:::

As an example, the access control matrix from earlier:

::: pst-scrollable-table-container
file1        file2        dir1         file3

---

user1   \-           read         \-           read/write
user2   read         read         read/write   read
user3   read         read         \-           \-
user4   read/write   read/write   \-           \-

: [Table 32.2 ]{.caption-number}[Simple access matrix (again)]{.caption-text}[\#](#fig-sec-simple2 "Link to this table"){.headerlink}
:::

can be encoded in the set of permissions shown below.

::: {.highlight-default .notranslate}
::: highlight
group1 = {user2,user3,user4}
file1:  owner = user4, group = group1
permissions = {owner = 'rw-', group = 'r--', other = '---'}
file2:  owner = user4, group = [doesn't matter]
permissions = {owner = 'rw-', group = 'r--', other = 'r--'}
dir1:   owner = user2, group = [doesn't matter]
permissions = {owner = 'rw-', group = '---', other = '---'}
group2 = {user1,user2}
file3:  owner = user1, group = group2
permissions = {owner = 'rw-', group = 'r--', other = '---'}
:::
:::

::: {#limitations-of-unix-permissions .section}

### [32.2.1. ] {.section-number}Limitations of Unix permissions[\#](#limitations-of-unix-permissions "Link to this heading") {.headerlink}

However if we make minor changes to this access control list:

::: {.highlight-none .notranslate}
::: highlight
file1   file2   dir1   file3
:::
:::

---

user1 --- r-- --- rw- user2 r-- r-- rw-- r-- user3 rw- r-- --- rwx user4 rw- rw- --- ---

: Complex access matrix (`ls -l`{.docutils .literal .notranslate} notation used for conciseness)

There are two problems here:

`file1`{.docutils .literal .notranslate}: Here two users have the highest level of privilege. If `user3`{.docutils .literal .notranslate} and `user4`{.docutils .literal .notranslate} are assigned to the same group, and the `file1`{.docutils .literal .notranslate} owner and group permission are both set to `rw-`{.docutils .literal .notranslate}, then the only permission left is "world". If that is set to `—`{.docutils .literal .notranslate} then `user2`{.docutils .literal .notranslate} will not have the read access specified in the access control matrix; however if it is set to `r–`{.docutils .literal .notranslate} then `user1`{.docutils .literal .notranslate} will improperly have access[[\[]{.fn-bracket}7[\]]{.fn-bracket}](#id16){#id7 .footnote-reference .brackets role="doc-noteref"}.

`file3`{.docutils .literal .notranslate}: Here there are 4 distinct combinations of permissions, while Unix permissions for a single file can only hold 3 combinations (owner, group, and world).
:::

::: {#access-control-lists .section}

### [32.2.2. ] {.section-number}Access Control Lists[\#](#access-control-lists "Link to this heading") {.headerlink}

Access Control Lists (ACLs) are explicit rules granting or denying access to users, and are more powerful than simple permissions. The idea is straightforward: an ACL is a list of rules, where each rule specifies a user or group, an action, and whether to allow or deny permissions.

Using the same example, which could not be encoded in standard Unix permissions:

::: {.highlight-none .notranslate}
::: highlight
file1   file2   dir1    file3
user1   ---     r--     ---     rw-
user2   r--     r--     rw-     r--
user3   rw-     r--     ---     rwx
user4   rw-     rw-     ---     ---
:::
:::

the desired access to `file1`{.docutils .literal .notranslate} can be expressed as:

::: {.highlight-default .notranslate}
::: highlight
file1:      owner = user4, group = {user4,user3}
owner: rw-, group: rw-, user2: r--, other: ---
file3:      owner = user3, group = {user3, user1}
owner: rwx, group: rw-, user2: r--, other: ---
:::
:::
:::

::: {#access-control-list-examples .section}

### [32.2.3. ] {.section-number}Access Control List Examples[\#](#access-control-list-examples "Link to this heading") {.headerlink}

This example uses OSX access control lists; however, Linux and Windows have similar mechanisms. We start with three user IDs: `pjd`{.docutils .literal .notranslate}, `guest`{.docutils .literal .notranslate}, and `joe`{.docutils .literal .notranslate}.

First a file is created, made readable by all users, and an ACL rule is added denying access to user joe (using the chmod ---a command).

::: {.highlight-default .notranslate}
::: highlight
pjd$ echo 'file 1 contents' > file.1
pjd$ chmod u=r,g=r,o=r file.1
pjd$ chmod +a 'joe deny read' file.1
pjd$ ls -le file.1
-r--r--r--+ 1 pjd  wheel  16 Aug 28 14:20 file.1
0: user:joe deny read
:::
:::

The file can now be read by both `pjd`{.docutils .literal .notranslate} and `guest`{.docutils .literal .notranslate}, but not `joe`{.docutils .literal .notranslate}:

::: {.highlight-default .notranslate}
::: highlight
pjd$ cat file.1
file 1 contents
joe$ cat file.1
cat: file.1: Permission denied
guest$ cat file.1
file 1 contents
:::
:::

Now we create a second file, set it owner read-only, and a rule is added giving read access to `joe`{.docutils .literal .notranslate} but no other user:

::: {.highlight-default .notranslate}
::: highlight
pjd$ echo 'file 2 contents' > file.2
pjd$ chmod u=r,g=,o= file.2
pjd$ ls -le file.2
-r--------+ 1 pjd  wheel  16 Aug 28 14:20 file.2
0: user:joe allow read
:::
:::

Now the file can be read by `pjd`{.docutils .literal .notranslate} and `joe`{.docutils .literal .notranslate} but not `guest`{.docutils .literal .notranslate}:

::: {.highlight-default .notranslate}
::: highlight
pjd$ cat file.2
file 2 contents
joe$ cat file.2
file 2 contents
guest$ cat file.2
cat: file.2: Permission denied
:::
:::
:::

::: {#other-privileged-operations .section}

### [32.2.4. ] {.section-number}Other Privileged Operations[\#](#other-privileged-operations "Link to this heading") {.headerlink}

Most Linux security checking is handled by a combination of the following rules:

- File system permissions
- Signal permissions

  - A non-root process can only signal processes with the same user ID.
- Super-user

  - User ID 0 (traditionally named "root") may access any file or signal any process; dangerous kernel operations can only be performed if the current user id is 0.
- Set UID

  - This allows users to invoke functions with elevated privileges when appropriate.

Most security checking in Linux / Unix is handled by file system permissions. As an example, system utilities need direct access to the disk (e.g. to format a new file system); normal users are prevented from reformatting the disk by the permissions on the special file representing the disk device (e.g. `/dev/sd0`{.docutils .literal .notranslate})

Unix signals are primarily used to kill a process, and so are only allowed between processes with the same user ID.

User ID number 0 (traditionally given the username "root") is allowed to bypass all user id-based permissions. In addition, certain system calls (e.g. mount a file system, reboot, install a kernel module) may only be performed by the super-user.

Finally, the setuid permission flag on a file tells the kernel that when the file is executed it should take on the identity of the file's owner, not the user who invoked it. This is a simple mechanism which allows programs to make finer distinctions than the kernel does. For instance the `mount`{.docutils .literal .notranslate} program is owned by user "root", and marked *setuid*, as under certain circumstances a normal user may be allowed to mount a filesystem (e.g. when it is a removable drive). When the program is run by a normal user, it checks configuration files to see whether the request is authorized; if so it is able to invoke the mount system call as user ID root.
:::
:::

::: {#selinux .section}

## [32.3. ] {.section-number}SELinux[\#](#selinux "Link to this heading") {.headerlink}

An alternate security mechanism available in Linux is called SELinux, or Security-Enhanced Linux. This is an enhancement to the normal Linux security model, which allows for exceptions to normal Linux rules. As an example, normal file permissions can still deny access to a file, but in cases where permissions allow access, SELinux rules might still forbid it.

SELinux is based on rules about *domains* and *types*. A domain is an execution environment that users run programs in; a set of rules for a domain determine which users can run what programs within that domain. Files have types, and rules determine which domains are able to access which types of files. Finally, users can change domains by running certain programs; when this occurs is again determined by (unsurprisingly) another set of rules.

Rules are loaded into the kernel by a user-space policy process, and file types are determined by an SELinux context associated with the file, stored in file *extended attributes* in the file inode.

As an example, the password file `/etc/passwd`{.docutils .literal .notranslate} contains usernames, groups, home directories, but not the hashed passwords themselves, which are in the shadow file, `/etc/shadow`{.docutils .literal .notranslate}; the shadow file may be modified when users run the `/usr/bin/passwd`{.docutils .literal .notranslate} program:

::: {.highlight-default .notranslate}
::: highlight
[root@localhost ~]# ls -Z /etc/passwd /etc/shadow /usr/bin/passwd
-rw-r--r--  root   root   system_u:object_r:etc_t          /etc/passwd
-r--------  root   root   system_u:object_r:shadow_t      /etc/shadow
-r-s--x--x  root   root   system_u:object_r:passwd_exec_t /usr/bin/passwd
:::
:::

One SELinux policy rule states that a user enters the `passwd_t`{.docutils .literal .notranslate} domain when executing a file of type `passwd_exec_t`{.docutils .literal .notranslate}; another states that processes running in the `passwd_t`{.docutils .literal .notranslate} domain have read and write privileges to files of type `shadow_t`{.docutils .literal .notranslate}. If SELinux is enabled, then even the superuser will only be able to modify `/etc/shadow`{.docutils .literal .notranslate} (and update your password) by executing `/usr/bin/passwd`{.docutils .literal .notranslate} or another executable marked `passwd_exec_t`{.docutils .literal .notranslate}.

Actual SELinux policies are extremely complex, containing hundreds of rules; if you are interested in finding out more there are a number of tutorials on the Internet, including [http://www.centos.org/docs/5/html/Deployment_Guide-en-US/ch-selinux.html](http://www.centos.org/docs/5/html/Deployment_Guide-en-US/ch-selinux.html){.reference .external}

::: {#control-of-information-flow .section}

### [32.3.1. ] {.section-number}Control of Information Flow[\#](#control-of-information-flow "Link to this heading") {.headerlink}

File access control is (somewhat) straightforward for an operating system to provide, as it represents a simple decision. If access is allowed, then the requested operation proceeds without interference; if it is denied, then the request fails completely.

In many cases, however, the desired restrictions are more subtle. Perhaps the earliest published example was a simple computer guessing game; the program would need to access the data to be guessed, while preventing the user from accessing it directly. Simple file permissions would not work, as if the game program were able to access the data file, then other programs (e.g. an editor) would be able to as well, allowing users to cheat.

In general such a problem requires interposing higher-layer software between the user and the protected information. In Unix the *setuid* mechanism allows a user A to run a program as a different user B (e.g. root), by having the executable file owned by user B and setting the *setuid* permission on the file. This can be done in a way that user B has full access to the protected data, allowing the program to access the data on behalf of user A, but only in ways allowed by the program logic.

In modern systems it is more common for such a gatekeeper role to be played by a server with access to the data, which accepts requests from users via messages and makes decisions on what data to reveal. Some examples:

**MySQL**: This database accepts connections over a TCP socket; users log in and then are able to read and modify those tables they have been given permission to access, regardless of which files the data resides in. The MySQL process runs under a separate user ID, which is the only one able to access the underlying data.

**Blackboard**: Connections to Blackboard are web sessions, controlled directly by users, and isolation of the data itself is ensured by preventing user access to the system that Blackboard runs on. The application logic enforces a complex set of rules governing what information each user may access; thus an instructor may see all grades, while a student may only see aggregate information (e.g. averages) about other students' grades.

::: {#review-questions .section}

#### [32.3.1.1. ] {.section-number}Review Questions[\#](#review-questions "Link to this heading") {.headerlink}

:::
:::
:::

::: {#attacks-stack-overflow .section}

## [32.4. ] {.section-number}Attacks --- Stack Overflow[\#](#attacks-stack-overflow "Link to this heading") {.headerlink}

![[Fig. 32.2 ]{.caption-number}[Stack frame and buffer overflow]{.caption-text}[\#](#fig-sec-worm "Link to this image"){.headerlink}](../_images/security-fig2.png){style="width: 70%;"}

In [[Fig. 32.2]{.std .std-numref}](#fig-sec-worm){.reference .internal} you can see a fragment of code that was attacked (among others) by the first piece of Internet malware, the 1988 Morris worm. The target program (`fingerd`{.docutils .literal .notranslate}) was run with a network connection for its standard input, and used the `gets`{.docutils .literal .notranslate} function to read a line of input into a buffer on the stack; it would normally return a simple reply based on that input and then exit. `Gets`{.docutils .literal .notranslate} reads a line from standard input, reading as many bytes as it takes before it finds a newline or reaches end-of-file. The buffer used, located at a lower address on the stack than the return address, was 512 bytes long, but the worm sent a 537-byte single-line message consisting of machine code, ending with a carefully chosen return address pointing at the beginning of the injected code. Since `fingerd`{.docutils .literal .notranslate} was run as the root user, the result was that when the function returned, the malware code had full control of the machine. In the years since, many lessons have been learned about preventing this sort of attack:

- (application writers) Do not use `gets`{.docutils .literal .notranslate} or other functions which can overrun a fixed-length buffer. (e.g. `fgets`{.docutils .literal .notranslate} takes the buffer length as an argument)
- (OS writers) Randomize the location of the stack and libraries each time a program is run, to make it more difficult to guess where an attack should return to.
- (OS writers) Use the NX ("no execute") page table bit on modern processors to prevent code on the stack from being executed.

Unfortunately buffer overflow vulnerabilities are still alive and well, as more sophisticated attacks have been developed to counter these techniques, as long as there is an initial application bug to give access to the stack. [[\[]{.fn-bracket}8[\]]{.fn-bracket}](#id17){#id8 .footnote-reference .brackets role="doc-noteref"}

::: {#security-sql-injection .section}

### [32.4.1. ] {.section-number}Security - SQL Injection[\#](#security-sql-injection "Link to this heading") {.headerlink}

![Image by Randall Munroe, from Xkcd: http://xkcd.com/327/, licensedunder creative commons non-commercial license 2.5](../_images/security-xkcd.png){#fig:security:xkcd width="80%"}

What happened to Bobby's school's student database? Let's assume they used code like this Visual Basic fragment, adapted from an example on an MSDN discussion board. ('&' concatenates strings in VB):

::: {.highlight-default .notranslate}
::: highlight
cmd.commandText = "INSERT INTO Students (Name) VALUES ('" \& studentName \& "');"
cmd.executeNonQuery()
:::
:::

So if studentName="Joey Smith", the following SQL command will be executed:

::: {.highlight-default .notranslate}
::: highlight
``INSERT INTO Students (Name) VALUES('Joey Smith');"
:::
:::

But if studentName="Robert'); DROP TABLE Students;--", we get:

::: {.highlight-default .notranslate}
::: highlight
``INSERT INTO Students (Name) VALUES('Robert'); DROP TABLE Students;--);''
:::
:::

Semicolon (";") is the command separator in SQL, and "" is a comment marker causing the rest of the line to be ignored; after adding 'Robert' to the Students table, the DROP TABLE command will be executed, removing the entire table.
:::

::: {#ssl-and-connection-security .section}

### [32.4.2. ] {.section-number}SSL and Connection Security[\#](#ssl-and-connection-security "Link to this heading") {.headerlink}

Secure Sockets Layer (SSL) allows two systems to establish a connection that cannot be intercepted, even by an adversary who observes every packet sent by both systems. Most importantly, it does not require any shared encryption key to be used by both systems[[\[]{.fn-bracket}9[\]]{.fn-bracket}](#id18){#id9 .footnote-reference .brackets role="doc-noteref"}. SSL relies on a combination of private- and public-key encryption:

- Private-key encryption uses a private key to encrypt a message, which may then be decrypted using the same private key.
- Public-key encryption uses two keys: (a) A public key to encrypt the message, and (b) a separate private key which must be used to decrypt it. In one of today's public-key systems, the public key is the product of two large prime numbers, and the private key is the two numbers themselves. The private key can be derived from the public key by factoring it, but for large numbers this is believed to be prohibitively difficult to actually do.

The simplest use of public-key encryption to provide a private connection would be for the two systems to each have public/private key pairs, send each other their public keys, and then encrypt traffic with the other system's public key. Unfortunately, public-key encryption is very computationally expensive, so instead SSL uses the following steps, sometimes called the SSL handshake:

1. The client connects to the server
2. The server sends its public key to the client
3. The client chooses a random number, encrypts it with the public key, and sends it to the server, which then decrypts it.

Client and server both use this random number as the key to a private-key code --- all outgoing messages are encrypted using this key, and all incoming messages are decrypted with it. There are additional aspects of the SSL protocol to guard against impersonation and "man-in-the-middle" attacks, which are somewhat more complicated and are not covered here.

---

[[\[]{.fn-bracket}[1](#id1){role="doc-backlink"}[\]]{.fn-bracket}]{.label}

E.g. see courses such as CS 5770, Software Vulnerabilities and Security, CS 6750, Cryptography and Communication Security, CS 6740, Network Security, or CS 6760, Privacy, Security and Usability

[[\[]{.fn-bracket}[2](#id2){role="doc-backlink"}[\]]{.fn-bracket}]{.label}

Additional identities are typically used for *system accounts*, like the `httpd`{.docutils .literal .notranslate} user associated with the webserver process on many systems. This allows the same mechanism to be used to grant or restrict access for various system operations.

[[\[]{.fn-bracket}[3](#id3){role="doc-backlink"}[\]]{.fn-bracket}]{.label}

Typically, the password is used as a key to encrypt a known, constant message.

[[\[]{.fn-bracket}[4](#id4){role="doc-backlink"}[\]]{.fn-bracket}]{.label}

Typically common words, plus personal names, plus variations on those words such as appending a digit.

[[\[]{.fn-bracket}[5](#id5){role="doc-backlink"}[\]]{.fn-bracket}]{.label}

see \[[https://engineering.purdue.edu/kak/compsec/NewLectures/](https://engineering.purdue.edu/kak/compsec/NewLectures/){.reference .external} Lecture24.pdf\]([https://engineering.purdue.edu/kak/compsec/NewLectures/](https://engineering.purdue.edu/kak/compsec/NewLectures/){.reference .external} Lecture24.pdf){.uri}

[[\[]{.fn-bracket}[6](#id6){role="doc-backlink"}[\]]{.fn-bracket}]{.label}

In Linux and some other systems this is handled in practice by the PAM (pluggable authentication module) framework, developed at Sun Microsystems, which specifies one or more authentication sources for the system to try for various events such as login.

[[\[]{.fn-bracket}[7](#id7){role="doc-backlink"}[\]]{.fn-bracket}]{.label}

Although it's possible to achieve this matrix with owner=\[`user2 r–`{.docutils .literal .notranslate}\], group=\[`(user2,user3,user4) rw-`{.docutils .literal .notranslate}\], and world=\[`—`{.docutils .literal .notranslate}\], it doesn't really make sense since the owner can gain write access just by changing permissions on the file.

[[\[]{.fn-bracket}[8](#id8){role="doc-backlink"}[\]]{.fn-bracket}]{.label}

If you are interested in learning more about stack overflows, there is a good tutorial at [http://www.tenouk.com/cncplusplusbufferoverflow.html](http://www.tenouk.com/cncplusplusbufferoverflow.html){.reference .external}

[[\[]{.fn-bracket}[9](#id9){role="doc-backlink"}[\]]{.fn-bracket}]{.label}

In most cases using a shared private key doesn't solve the problem: before you use it, you have to figure out how to securely communicate the private key.
:::
:::
:::

::: prev-next-area
[](../virt/virt.html "previous page"){.left-prev}

::: prev-next-info
previous

[31. ]{.section-number}Virtualization
:::

[](../misc/howto.html "next page"){.right-next}

::: prev-next-info
next

[33. ]{.section-number}How to read this book
:::
:::
:::

::: {.bd-sidebar-secondary .bd-toc}
::: {.sidebar-secondary-items .sidebar-secondary__inner}
::: sidebar-secondary-item
::: {.page-toc .tocsection .onthispage}
Contents
:::

- [32.1. Protection](#protection){.reference .internal .nav-link}
  - [32.1.1. Identity and Authentication](#identity-and-authentication){.reference .internal .nav-link}
  - [32.1.2. Checking passwords](#checking-passwords){.reference .internal .nav-link}
  - [32.1.3. Centralized authentication - LDAP and Kerberos](#centralized-authentication-ldap-and-kerberos){.reference .internal .nav-link}
- [32.2. Unix Access Control](#unix-access-control){.reference .internal .nav-link}
  - [32.2.1. Limitations of Unix permissions](#limitations-of-unix-permissions){.reference .internal .nav-link}
  - [32.2.2. Access Control Lists](#access-control-lists){.reference .internal .nav-link}
  - [32.2.3. Access Control List Examples](#access-control-list-examples){.reference .internal .nav-link}
  - [32.2.4. Other Privileged Operations](#other-privileged-operations){.reference .internal .nav-link}
- [32.3. SELinux](#selinux){.reference .internal .nav-link}
  - [32.3.1. Control of Information Flow](#control-of-information-flow){.reference .internal .nav-link}
    - [32.3.1.1. Review Questions](#review-questions){.reference .internal .nav-link}
- [32.4. Attacks --- Stack Overflow](#attacks-stack-overflow){.reference .internal .nav-link}
  - [32.4.1. Security - SQL Injection](#security-sql-injection){.reference .internal .nav-link}
  - [32.4.2. SSL and Connection Security](#ssl-and-connection-security){.reference .internal .nav-link}
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
