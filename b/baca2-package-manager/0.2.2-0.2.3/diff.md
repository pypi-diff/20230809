# Comparing `tmp/baca2-package-manager-0.2.2.tar.gz` & `tmp/baca2-package-manager-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baca2-package-manager-0.2.2.tar", last modified: Thu Jul 27 15:11:45 2023, max compression
+gzip compressed data, was "baca2-package-manager-0.2.3.tar", last modified: Wed Aug  9 05:24:30 2023, max compression
```

## Comparing `baca2-package-manager-0.2.2.tar` & `baca2-package-manager-0.2.3.tar`

### file list

```diff
@@ -1,20 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 15:11:45.862127 baca2-package-manager-0.2.2/
--rw-rw-rw-   0        0        0    35823 2023-07-26 17:19:31.000000 baca2-package-manager-0.2.2/LICENSE
--rw-rw-rw-   0        0        0      760 2023-07-27 15:11:45.862127 baca2-package-manager-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0      248 2023-07-26 18:31:13.000000 baca2-package-manager-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-27 15:11:45.797762 baca2-package-manager-0.2.2/baca2PackageManager/
--rw-rw-rw-   0        0        0      748 2023-07-26 18:26:18.000000 baca2-package-manager-0.2.2/baca2PackageManager/__init__.py
--rw-rw-rw-   0        0        0       83 2023-07-26 17:55:56.000000 baca2-package-manager-0.2.2/baca2PackageManager/consts.py
--rw-rw-rw-   0        0        0    24899 2023-07-27 15:10:38.000000 baca2-package-manager-0.2.2/baca2PackageManager/manager.py
--rw-rw-rw-   0        0        0      133 2023-07-26 17:58:18.000000 baca2-package-manager-0.2.2/baca2PackageManager/manager_exceptions.py
--rw-rw-rw-   0        0        0     6069 2023-07-27 15:10:38.000000 baca2-package-manager-0.2.2/baca2PackageManager/validators.py
-drwxrwxrwx   0        0        0        0 2023-07-27 15:11:45.857770 baca2-package-manager-0.2.2/baca2_package_manager.egg-info/
--rw-rw-rw-   0        0        0      760 2023-07-27 15:11:45.000000 baca2-package-manager-0.2.2/baca2_package_manager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      434 2023-07-27 15:11:45.000000 baca2-package-manager-0.2.2/baca2_package_manager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 15:11:45.000000 baca2-package-manager-0.2.2/baca2_package_manager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-27 15:11:45.000000 baca2-package-manager-0.2.2/baca2_package_manager.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-07-27 15:11:45.000000 baca2-package-manager-0.2.2/baca2_package_manager.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-27 15:11:45.863133 baca2-package-manager-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0      722 2023-07-27 15:11:38.000000 baca2-package-manager-0.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-27 15:11:45.860286 baca2-package-manager-0.2.2/tests/
--rw-rw-rw-   0        0        0    24517 2023-07-27 13:54:21.000000 baca2-package-manager-0.2.2/tests/tests.py
+drwxr-xr-x   0 zyndram   (1000) zyndram   (1000)        0 2023-08-09 05:24:30.556209 baca2-package-manager-0.2.3/
+-rw-r--r--   0 zyndram   (1000) zyndram   (1000)    35149 2023-07-31 11:22:11.000000 baca2-package-manager-0.2.3/LICENSE
+-rw-r--r--   0 zyndram   (1000) zyndram   (1000)      741 2023-08-09 05:24:30.556209 baca2-package-manager-0.2.3/PKG-INFO
+-rw-r--r--   0 zyndram   (1000) zyndram   (1000)      243 2023-07-31 11:22:11.000000 baca2-package-manager-0.2.3/README.md
+drwxr-xr-x   0 zyndram   (1000) zyndram   (1000)        0 2023-08-09 05:24:30.556209 baca2-package-manager-0.2.3/baca2PackageManager/
+-rw-r--r--   0 zyndram   (1000) zyndram   (1000)      713 2023-07-31 11:22:11.000000 baca2-package-manager-0.2.3/baca2PackageManager/__init__.py
+-rw-r--r--   0 zyndram   (1000) zyndram   (1000)       80 2023-07-31 11:22:11.000000 baca2-package-manager-0.2.3/baca2PackageManager/consts.py
+-rw-r--r--   0 zyndram   (1000) zyndram   (1000)    24199 2023-08-09 05:22:43.000000 baca2-package-manager-0.2.3/baca2PackageManager/manager.py
+-rw-r--r--   0 zyndram   (1000) zyndram   (1000)      123 2023-07-31 11:22:11.000000 baca2-package-manager-0.2.3/baca2PackageManager/manager_exceptions.py
+-rw-r--r--   0 zyndram   (1000) zyndram   (1000)     5818 2023-07-31 11:22:11.000000 baca2-package-manager-0.2.3/baca2PackageManager/validators.py
+drwxr-xr-x   0 zyndram   (1000) zyndram   (1000)        0 2023-08-09 05:24:30.556209 baca2-package-manager-0.2.3/baca2_package_manager.egg-info/
+-rw-r--r--   0 zyndram   (1000) zyndram   (1000)      741 2023-08-09 05:24:30.000000 baca2-package-manager-0.2.3/baca2_package_manager.egg-info/PKG-INFO
+-rw-r--r--   0 zyndram   (1000) zyndram   (1000)      419 2023-08-09 05:24:30.000000 baca2-package-manager-0.2.3/baca2_package_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 zyndram   (1000) zyndram   (1000)        1 2023-08-09 05:24:30.000000 baca2-package-manager-0.2.3/baca2_package_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 zyndram   (1000) zyndram   (1000)        7 2023-08-09 05:24:30.000000 baca2-package-manager-0.2.3/baca2_package_manager.egg-info/requires.txt
+-rw-r--r--   0 zyndram   (1000) zyndram   (1000)       20 2023-08-09 05:24:30.000000 baca2-package-manager-0.2.3/baca2_package_manager.egg-info/top_level.txt
+-rw-r--r--   0 zyndram   (1000) zyndram   (1000)       38 2023-08-09 05:24:30.556209 baca2-package-manager-0.2.3/setup.cfg
+-rw-r--r--   0 zyndram   (1000) zyndram   (1000)      700 2023-08-09 05:23:58.000000 baca2-package-manager-0.2.3/setup.py
```

### Comparing `baca2-package-manager-0.2.2/LICENSE` & `baca2-package-manager-0.2.3/LICENSE`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,674 +1,674 @@
-                    GNU GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-                            Preamble
-
-  The GNU General Public License is a free, copyleft license for
-software and other kinds of works.
-
-  The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works.  By contrast,
-the GNU General Public License is intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.  We, the Free Software Foundation, use the
-GNU General Public License for most of our software; it applies also to
-any other work released this way by its authors.  You can apply it to
-your programs, too.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-  To protect your rights, we need to prevent others from denying you
-these rights or asking you to surrender the rights.  Therefore, you have
-certain responsibilities if you distribute copies of the software, or if
-you modify it: responsibilities to respect the freedom of others.
-
-  For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must pass on to the recipients the same
-freedoms that you received.  You must make sure that they, too, receive
-or can get the source code.  And you must show them these terms so they
-know their rights.
-
-  Developers that use the GNU GPL protect your rights with two steps:
-(1) assert copyright on the software, and (2) offer you this License
-giving you legal permission to copy, distribute and/or modify it.
-
-  For the developers' and authors' protection, the GPL clearly explains
-that there is no warranty for this free software.  For both users' and
-authors' sake, the GPL requires that modified versions be marked as
-changed, so that their problems will not be attributed erroneously to
-authors of previous versions.
-
-  Some devices are designed to deny users access to install or run
-modified versions of the software inside them, although the manufacturer
-can do so.  This is fundamentally incompatible with the aim of
-protecting users' freedom to change the software.  The systematic
-pattern of such abuse occurs in the area of products for individuals to
-use, which is precisely where it is most unacceptable.  Therefore, we
-have designed this version of the GPL to prohibit the practice for those
-products.  If such problems arise substantially in other domains, we
-stand ready to extend this provision to those domains in future versions
-of the GPL, as needed to protect the freedom of users.
-
-  Finally, every program is threatened constantly by software patents.
-States should not allow patents to restrict development and use of
-software on general-purpose computers, but in those that do, we wish to
-avoid the special danger that patents applied to a free program could
-make it effectively proprietary.  To prevent this, the GPL assures that
-patents cannot be used to render the program non-free.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-                       TERMS AND CONDITIONS
-
-  0. Definitions.
-
-  "This License" refers to version 3 of the GNU General Public License.
-
-  "Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
-
-  "The Program" refers to any copyrightable work licensed under this
-License.  Each licensee is addressed as "you".  "Licensees" and
-"recipients" may be individuals or organizations.
-
-  To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy.  The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
-
-  A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-  To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy.  Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-  To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies.  Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
-
-  An interactive user interface displays "Appropriate Legal Notices"
-to the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License.  If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-  1. Source Code.
-
-  The "source code" for a work means the preferred form of the work
-for making modifications to it.  "Object code" means any non-source
-form of a work.
-
-  A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-  The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form.  A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-  The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities.  However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work.  For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-  The Corresponding Source need not include anything that users
-can regenerate automatically from other parts of the Corresponding
-Source.
-
-  The Corresponding Source for a work in source code form is that
-same work.
-
-  2. Basic Permissions.
-
-  All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met.  This License explicitly affirms your unlimited
-permission to run the unmodified Program.  The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work.  This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-  You may make, run and propagate covered works that you do not
-convey, without conditions so long as your license otherwise remains
-in force.  You may convey covered works to others for the sole purpose
-of having them make modifications exclusively for you, or provide you
-with facilities for running those works, provided that you comply with
-the terms of this License in conveying all material for which you do
-not control copyright.  Those thus making or running the covered works
-for you must do so exclusively on your behalf, under your direction
-and control, on terms that prohibit them from making any copies of
-your copyrighted material outside their relationship with you.
-
-  Conveying under any other circumstances is permitted solely under
-the conditions stated below.  Sublicensing is not allowed; section 10
-makes it unnecessary.
-
-  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-  No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-  When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to
-the covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
-
-  4. Conveying Verbatim Copies.
-
-  You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-  You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-  5. Conveying Modified Source Versions.
-
-  You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified
-    it, and giving a relevant date.
-
-    b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under section
-    7.  This requirement modifies the requirement in section 4 to
-    "keep intact all notices".
-
-    c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy.  This
-    License will therefore apply, along with any applicable section 7
-    additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged.  This License gives no
-    permission to license the work in any other way, but it does not
-    invalidate such permission if you have separately received it.
-
-    d) If the work has interactive user interfaces, each must display
-    Appropriate Legal Notices; however, if the Program has interactive
-    interfaces that do not display Appropriate Legal Notices, your
-    work need not make them do so.
-
-  A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit.  Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-  6. Conveying Non-Source Forms.
-
-  You may convey a covered work in object code form under the terms
-of sections 4 and 5, provided that you also convey the
-machine-readable Corresponding Source under the terms of this License,
-in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by the
-    Corresponding Source fixed on a durable physical medium
-    customarily used for software interchange.
-
-    b) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by a
-    written offer, valid for at least three years and valid for as
-    long as you offer spare parts or customer support for that product
-    model, to give anyone who possesses the object code either (1) a
-    copy of the Corresponding Source for all the software in the
-    product that is covered by this License, on a durable physical
-    medium customarily used for software interchange, for a price no
-    more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the
-    Corresponding Source from a network server at no charge.
-
-    c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source.  This
-    alternative is allowed only occasionally and noncommercially, and
-    only if you received the object code with such an offer, in accord
-    with subsection 6b.
-
-    d) Convey the object code by offering access from a designated
-    place (gratis or for a charge), and offer equivalent access to the
-    Corresponding Source in the same way through the same place at no
-    further charge.  You need not require recipients to copy the
-    Corresponding Source along with the object code.  If the place to
-    copy the object code is a network server, the Corresponding Source
-    may be on a different server (operated by you or a third party)
-    that supports equivalent copying facilities, provided you maintain
-    clear directions next to the object code saying where to find the
-    Corresponding Source.  Regardless of what server hosts the
-    Corresponding Source, you remain obligated to ensure that it is
-    available for as long as needed to satisfy these requirements.
-
-    e) Convey the object code using peer-to-peer transmission, provided
-    you inform other peers where the object code and Corresponding
-    Source of the work are being offered to the general public at no
-    charge under subsection 6d.
-
-  A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-  A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for incorporation
-into a dwelling.  In determining whether a product is a consumer product,
-doubtful cases shall be resolved in favor of coverage.  For a particular
-product received by a particular user, "normally used" refers to a
-typical or common use of that class of product, regardless of the status
-of the particular user or of the way in which the particular user
-actually uses, or expects or is expected to use, the product.  A product
-is a consumer product regardless of whether the product has substantial
-commercial, industrial or non-consumer uses, unless such uses represent
-the only significant mode of use of the product.
-
-  "Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product from
-a modified version of its Corresponding Source.  The information must
-suffice to ensure that the continued functioning of the modified object
-code is in no case prevented or interfered with solely because
-modification has been made.
-
-  If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information.  But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-  The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed.  Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
-
-  Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-  7. Additional Terms.
-
-  "Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law.  If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-  When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it.  (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.)  You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-  Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders of
-that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the
-    terms of sections 15 and 16 of this License; or
-
-    b) Requiring preservation of specified reasonable legal notices or
-    author attributions in that material or in the Appropriate Legal
-    Notices displayed by works containing it; or
-
-    c) Prohibiting misrepresentation of the origin of that material, or
-    requiring that modified versions of such material be marked in
-    reasonable ways as different from the original version; or
-
-    d) Limiting the use for publicity purposes of names of licensors or
-    authors of the material; or
-
-    e) Declining to grant rights under trademark law for use of some
-    trade names, trademarks, or service marks; or
-
-    f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions of
-    it) with contractual assumptions of liability to the recipient, for
-    any liability that these contractual assumptions directly impose on
-    those licensors and authors.
-
-  All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10.  If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term.  If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-  If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-  Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions;
-the above requirements apply either way.
-
-  8. Termination.
-
-  You may not propagate or modify a covered work except as expressly
-provided under this License.  Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-  However, if you cease all violation of this License, then your
-license from a particular copyright holder is reinstated (a)
-provisionally, unless and until the copyright holder explicitly and
-finally terminates your license, and (b) permanently, if the copyright
-holder fails to notify you of the violation by some reasonable means
-prior to 60 days after the cessation.
-
-  Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-  Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License.  If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-  9. Acceptance Not Required for Having Copies.
-
-  You are not required to accept this License in order to receive or
-run a copy of the Program.  Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance.  However,
-nothing other than this License grants you permission to propagate or
-modify any covered work.  These actions infringe copyright if you do
-not accept this License.  Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-  10. Automatic Licensing of Downstream Recipients.
-
-  Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License.  You are not responsible
-for enforcing compliance by third parties with this License.
-
-  An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations.  If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-  You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License.  For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-  11. Patents.
-
-  A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based.  The
-work thus licensed is called the contributor's "contributor version".
-
-  A contributor's "essential patent claims" are all patent claims
-owned or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version.  For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-  Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-  In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement).  To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-  If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients.  "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-  If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-  A patent license is "discriminatory" if it does not include within
-the scope of its coverage, prohibits the exercise of, or is
-conditioned on the non-exercise of one or more of the rights that are
-specifically granted under this License.  You may not convey a covered
-work if you are a party to an arrangement with a third party that is
-in the business of distributing software, under which you make payment
-to the third party based on the extent of your activity of conveying
-the work, and under which the third party grants, to any of the
-parties who would receive the covered work from you, a discriminatory
-patent license (a) in connection with copies of the covered work
-conveyed by you (or copies made from those copies), or (b) primarily
-for and in connection with specific products or compilations that
-contain the covered work, unless you entered into that arrangement,
-or that patent license was granted, prior to 28 March 2007.
-
-  Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-  12. No Surrender of Others' Freedom.
-
-  If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you may
-not convey it at all.  For example, if you agree to terms that obligate you
-to collect a royalty for further conveying from those to whom you convey
-the Program, the only way you could satisfy both those terms and this
-License would be to refrain entirely from conveying the Program.
-
-  13. Use with the GNU Affero General Public License.
-
-  Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU Affero General Public License into a single
-combined work, and to convey the resulting work.  The terms of this
-License will continue to apply to the part which is the covered work,
-but the special requirements of the GNU Affero General Public License,
-section 13, concerning interaction through a network will apply to the
-combination as such.
-
-  14. Revised Versions of this License.
-
-  The Free Software Foundation may publish revised and/or new versions of
-the GNU General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-  Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation.  If the Program does not specify a version number of the
-GNU General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-  If the Program specifies that a proxy can decide which future
-versions of the GNU General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
-
-  Later license versions may give you additional or different
-permissions.  However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-  15. Disclaimer of Warranty.
-
-  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. Limitation of Liability.
-
-  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGES.
-
-  17. Interpretation of Sections 15 and 16.
-
-  If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
-
-                     END OF TERMS AND CONDITIONS
-
-            How to Apply These Terms to Your New Programs
-
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-  If the program does terminal interaction, make it output a short
-notice like this when it starts in an interactive mode:
-
-    <program>  Copyright (C) <year>  <name of author>
-    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, your program's commands
-might be different; for a GUI interface, you would use an "about box".
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<https://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
-<https://www.gnu.org/licenses/why-not-lgpl.html>.
+                    GNU GENERAL PUBLIC LICENSE
+                       Version 3, 29 June 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+                            Preamble
+
+  The GNU General Public License is a free, copyleft license for
+software and other kinds of works.
+
+  The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works.  By contrast,
+the GNU General Public License is intended to guarantee your freedom to
+share and change all versions of a program--to make sure it remains free
+software for all its users.  We, the Free Software Foundation, use the
+GNU General Public License for most of our software; it applies also to
+any other work released this way by its authors.  You can apply it to
+your programs, too.
+
+  When we speak of free software, we are referring to freedom, not
+price.  Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+  To protect your rights, we need to prevent others from denying you
+these rights or asking you to surrender the rights.  Therefore, you have
+certain responsibilities if you distribute copies of the software, or if
+you modify it: responsibilities to respect the freedom of others.
+
+  For example, if you distribute copies of such a program, whether
+gratis or for a fee, you must pass on to the recipients the same
+freedoms that you received.  You must make sure that they, too, receive
+or can get the source code.  And you must show them these terms so they
+know their rights.
+
+  Developers that use the GNU GPL protect your rights with two steps:
+(1) assert copyright on the software, and (2) offer you this License
+giving you legal permission to copy, distribute and/or modify it.
+
+  For the developers' and authors' protection, the GPL clearly explains
+that there is no warranty for this free software.  For both users' and
+authors' sake, the GPL requires that modified versions be marked as
+changed, so that their problems will not be attributed erroneously to
+authors of previous versions.
+
+  Some devices are designed to deny users access to install or run
+modified versions of the software inside them, although the manufacturer
+can do so.  This is fundamentally incompatible with the aim of
+protecting users' freedom to change the software.  The systematic
+pattern of such abuse occurs in the area of products for individuals to
+use, which is precisely where it is most unacceptable.  Therefore, we
+have designed this version of the GPL to prohibit the practice for those
+products.  If such problems arise substantially in other domains, we
+stand ready to extend this provision to those domains in future versions
+of the GPL, as needed to protect the freedom of users.
+
+  Finally, every program is threatened constantly by software patents.
+States should not allow patents to restrict development and use of
+software on general-purpose computers, but in those that do, we wish to
+avoid the special danger that patents applied to a free program could
+make it effectively proprietary.  To prevent this, the GPL assures that
+patents cannot be used to render the program non-free.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.
+
+                       TERMS AND CONDITIONS
+
+  0. Definitions.
+
+  "This License" refers to version 3 of the GNU General Public License.
+
+  "Copyright" also means copyright-like laws that apply to other kinds of
+works, such as semiconductor masks.
+
+  "The Program" refers to any copyrightable work licensed under this
+License.  Each licensee is addressed as "you".  "Licensees" and
+"recipients" may be individuals or organizations.
+
+  To "modify" a work means to copy from or adapt all or part of the work
+in a fashion requiring copyright permission, other than the making of an
+exact copy.  The resulting work is called a "modified version" of the
+earlier work or a work "based on" the earlier work.
+
+  A "covered work" means either the unmodified Program or a work based
+on the Program.
+
+  To "propagate" a work means to do anything with it that, without
+permission, would make you directly or secondarily liable for
+infringement under applicable copyright law, except executing it on a
+computer or modifying a private copy.  Propagation includes copying,
+distribution (with or without modification), making available to the
+public, and in some countries other activities as well.
+
+  To "convey" a work means any kind of propagation that enables other
+parties to make or receive copies.  Mere interaction with a user through
+a computer network, with no transfer of a copy, is not conveying.
+
+  An interactive user interface displays "Appropriate Legal Notices"
+to the extent that it includes a convenient and prominently visible
+feature that (1) displays an appropriate copyright notice, and (2)
+tells the user that there is no warranty for the work (except to the
+extent that warranties are provided), that licensees may convey the
+work under this License, and how to view a copy of this License.  If
+the interface presents a list of user commands or options, such as a
+menu, a prominent item in the list meets this criterion.
+
+  1. Source Code.
+
+  The "source code" for a work means the preferred form of the work
+for making modifications to it.  "Object code" means any non-source
+form of a work.
+
+  A "Standard Interface" means an interface that either is an official
+standard defined by a recognized standards body, or, in the case of
+interfaces specified for a particular programming language, one that
+is widely used among developers working in that language.
+
+  The "System Libraries" of an executable work include anything, other
+than the work as a whole, that (a) is included in the normal form of
+packaging a Major Component, but which is not part of that Major
+Component, and (b) serves only to enable use of the work with that
+Major Component, or to implement a Standard Interface for which an
+implementation is available to the public in source code form.  A
+"Major Component", in this context, means a major essential component
+(kernel, window system, and so on) of the specific operating system
+(if any) on which the executable work runs, or a compiler used to
+produce the work, or an object code interpreter used to run it.
+
+  The "Corresponding Source" for a work in object code form means all
+the source code needed to generate, install, and (for an executable
+work) run the object code and to modify the work, including scripts to
+control those activities.  However, it does not include the work's
+System Libraries, or general-purpose tools or generally available free
+programs which are used unmodified in performing those activities but
+which are not part of the work.  For example, Corresponding Source
+includes interface definition files associated with source files for
+the work, and the source code for shared libraries and dynamically
+linked subprograms that the work is specifically designed to require,
+such as by intimate data communication or control flow between those
+subprograms and other parts of the work.
+
+  The Corresponding Source need not include anything that users
+can regenerate automatically from other parts of the Corresponding
+Source.
+
+  The Corresponding Source for a work in source code form is that
+same work.
+
+  2. Basic Permissions.
+
+  All rights granted under this License are granted for the term of
+copyright on the Program, and are irrevocable provided the stated
+conditions are met.  This License explicitly affirms your unlimited
+permission to run the unmodified Program.  The output from running a
+covered work is covered by this License only if the output, given its
+content, constitutes a covered work.  This License acknowledges your
+rights of fair use or other equivalent, as provided by copyright law.
+
+  You may make, run and propagate covered works that you do not
+convey, without conditions so long as your license otherwise remains
+in force.  You may convey covered works to others for the sole purpose
+of having them make modifications exclusively for you, or provide you
+with facilities for running those works, provided that you comply with
+the terms of this License in conveying all material for which you do
+not control copyright.  Those thus making or running the covered works
+for you must do so exclusively on your behalf, under your direction
+and control, on terms that prohibit them from making any copies of
+your copyrighted material outside their relationship with you.
+
+  Conveying under any other circumstances is permitted solely under
+the conditions stated below.  Sublicensing is not allowed; section 10
+makes it unnecessary.
+
+  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+  No covered work shall be deemed part of an effective technological
+measure under any applicable law fulfilling obligations under article
+11 of the WIPO copyright treaty adopted on 20 December 1996, or
+similar laws prohibiting or restricting circumvention of such
+measures.
+
+  When you convey a covered work, you waive any legal power to forbid
+circumvention of technological measures to the extent such circumvention
+is effected by exercising rights under this License with respect to
+the covered work, and you disclaim any intention to limit operation or
+modification of the work as a means of enforcing, against the work's
+users, your or third parties' legal rights to forbid circumvention of
+technological measures.
+
+  4. Conveying Verbatim Copies.
+
+  You may convey verbatim copies of the Program's source code as you
+receive it, in any medium, provided that you conspicuously and
+appropriately publish on each copy an appropriate copyright notice;
+keep intact all notices stating that this License and any
+non-permissive terms added in accord with section 7 apply to the code;
+keep intact all notices of the absence of any warranty; and give all
+recipients a copy of this License along with the Program.
+
+  You may charge any price or no price for each copy that you convey,
+and you may offer support or warranty protection for a fee.
+
+  5. Conveying Modified Source Versions.
+
+  You may convey a work based on the Program, or the modifications to
+produce it from the Program, in the form of source code under the
+terms of section 4, provided that you also meet all of these conditions:
+
+    a) The work must carry prominent notices stating that you modified
+    it, and giving a relevant date.
+
+    b) The work must carry prominent notices stating that it is
+    released under this License and any conditions added under section
+    7.  This requirement modifies the requirement in section 4 to
+    "keep intact all notices".
+
+    c) You must license the entire work, as a whole, under this
+    License to anyone who comes into possession of a copy.  This
+    License will therefore apply, along with any applicable section 7
+    additional terms, to the whole of the work, and all its parts,
+    regardless of how they are packaged.  This License gives no
+    permission to license the work in any other way, but it does not
+    invalidate such permission if you have separately received it.
+
+    d) If the work has interactive user interfaces, each must display
+    Appropriate Legal Notices; however, if the Program has interactive
+    interfaces that do not display Appropriate Legal Notices, your
+    work need not make them do so.
+
+  A compilation of a covered work with other separate and independent
+works, which are not by their nature extensions of the covered work,
+and which are not combined with it such as to form a larger program,
+in or on a volume of a storage or distribution medium, is called an
+"aggregate" if the compilation and its resulting copyright are not
+used to limit the access or legal rights of the compilation's users
+beyond what the individual works permit.  Inclusion of a covered work
+in an aggregate does not cause this License to apply to the other
+parts of the aggregate.
+
+  6. Conveying Non-Source Forms.
+
+  You may convey a covered work in object code form under the terms
+of sections 4 and 5, provided that you also convey the
+machine-readable Corresponding Source under the terms of this License,
+in one of these ways:
+
+    a) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by the
+    Corresponding Source fixed on a durable physical medium
+    customarily used for software interchange.
+
+    b) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by a
+    written offer, valid for at least three years and valid for as
+    long as you offer spare parts or customer support for that product
+    model, to give anyone who possesses the object code either (1) a
+    copy of the Corresponding Source for all the software in the
+    product that is covered by this License, on a durable physical
+    medium customarily used for software interchange, for a price no
+    more than your reasonable cost of physically performing this
+    conveying of source, or (2) access to copy the
+    Corresponding Source from a network server at no charge.
+
+    c) Convey individual copies of the object code with a copy of the
+    written offer to provide the Corresponding Source.  This
+    alternative is allowed only occasionally and noncommercially, and
+    only if you received the object code with such an offer, in accord
+    with subsection 6b.
+
+    d) Convey the object code by offering access from a designated
+    place (gratis or for a charge), and offer equivalent access to the
+    Corresponding Source in the same way through the same place at no
+    further charge.  You need not require recipients to copy the
+    Corresponding Source along with the object code.  If the place to
+    copy the object code is a network server, the Corresponding Source
+    may be on a different server (operated by you or a third party)
+    that supports equivalent copying facilities, provided you maintain
+    clear directions next to the object code saying where to find the
+    Corresponding Source.  Regardless of what server hosts the
+    Corresponding Source, you remain obligated to ensure that it is
+    available for as long as needed to satisfy these requirements.
+
+    e) Convey the object code using peer-to-peer transmission, provided
+    you inform other peers where the object code and Corresponding
+    Source of the work are being offered to the general public at no
+    charge under subsection 6d.
+
+  A separable portion of the object code, whose source code is excluded
+from the Corresponding Source as a System Library, need not be
+included in conveying the object code work.
+
+  A "User Product" is either (1) a "consumer product", which means any
+tangible personal property which is normally used for personal, family,
+or household purposes, or (2) anything designed or sold for incorporation
+into a dwelling.  In determining whether a product is a consumer product,
+doubtful cases shall be resolved in favor of coverage.  For a particular
+product received by a particular user, "normally used" refers to a
+typical or common use of that class of product, regardless of the status
+of the particular user or of the way in which the particular user
+actually uses, or expects or is expected to use, the product.  A product
+is a consumer product regardless of whether the product has substantial
+commercial, industrial or non-consumer uses, unless such uses represent
+the only significant mode of use of the product.
+
+  "Installation Information" for a User Product means any methods,
+procedures, authorization keys, or other information required to install
+and execute modified versions of a covered work in that User Product from
+a modified version of its Corresponding Source.  The information must
+suffice to ensure that the continued functioning of the modified object
+code is in no case prevented or interfered with solely because
+modification has been made.
+
+  If you convey an object code work under this section in, or with, or
+specifically for use in, a User Product, and the conveying occurs as
+part of a transaction in which the right of possession and use of the
+User Product is transferred to the recipient in perpetuity or for a
+fixed term (regardless of how the transaction is characterized), the
+Corresponding Source conveyed under this section must be accompanied
+by the Installation Information.  But this requirement does not apply
+if neither you nor any third party retains the ability to install
+modified object code on the User Product (for example, the work has
+been installed in ROM).
+
+  The requirement to provide Installation Information does not include a
+requirement to continue to provide support service, warranty, or updates
+for a work that has been modified or installed by the recipient, or for
+the User Product in which it has been modified or installed.  Access to a
+network may be denied when the modification itself materially and
+adversely affects the operation of the network or violates the rules and
+protocols for communication across the network.
+
+  Corresponding Source conveyed, and Installation Information provided,
+in accord with this section must be in a format that is publicly
+documented (and with an implementation available to the public in
+source code form), and must require no special password or key for
+unpacking, reading or copying.
+
+  7. Additional Terms.
+
+  "Additional permissions" are terms that supplement the terms of this
+License by making exceptions from one or more of its conditions.
+Additional permissions that are applicable to the entire Program shall
+be treated as though they were included in this License, to the extent
+that they are valid under applicable law.  If additional permissions
+apply only to part of the Program, that part may be used separately
+under those permissions, but the entire Program remains governed by
+this License without regard to the additional permissions.
+
+  When you convey a copy of a covered work, you may at your option
+remove any additional permissions from that copy, or from any part of
+it.  (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.)  You may place
+additional permissions on material, added by you to a covered work,
+for which you have or can give appropriate copyright permission.
+
+  Notwithstanding any other provision of this License, for material you
+add to a covered work, you may (if authorized by the copyright holders of
+that material) supplement the terms of this License with terms:
+
+    a) Disclaiming warranty or limiting liability differently from the
+    terms of sections 15 and 16 of this License; or
+
+    b) Requiring preservation of specified reasonable legal notices or
+    author attributions in that material or in the Appropriate Legal
+    Notices displayed by works containing it; or
+
+    c) Prohibiting misrepresentation of the origin of that material, or
+    requiring that modified versions of such material be marked in
+    reasonable ways as different from the original version; or
+
+    d) Limiting the use for publicity purposes of names of licensors or
+    authors of the material; or
+
+    e) Declining to grant rights under trademark law for use of some
+    trade names, trademarks, or service marks; or
+
+    f) Requiring indemnification of licensors and authors of that
+    material by anyone who conveys the material (or modified versions of
+    it) with contractual assumptions of liability to the recipient, for
+    any liability that these contractual assumptions directly impose on
+    those licensors and authors.
+
+  All other non-permissive additional terms are considered "further
+restrictions" within the meaning of section 10.  If the Program as you
+received it, or any part of it, contains a notice stating that it is
+governed by this License along with a term that is a further
+restriction, you may remove that term.  If a license document contains
+a further restriction but permits relicensing or conveying under this
+License, you may add to a covered work material governed by the terms
+of that license document, provided that the further restriction does
+not survive such relicensing or conveying.
+
+  If you add terms to a covered work in accord with this section, you
+must place, in the relevant source files, a statement of the
+additional terms that apply to those files, or a notice indicating
+where to find the applicable terms.
+
+  Additional terms, permissive or non-permissive, may be stated in the
+form of a separately written license, or stated as exceptions;
+the above requirements apply either way.
+
+  8. Termination.
+
+  You may not propagate or modify a covered work except as expressly
+provided under this License.  Any attempt otherwise to propagate or
+modify it is void, and will automatically terminate your rights under
+this License (including any patent licenses granted under the third
+paragraph of section 11).
+
+  However, if you cease all violation of this License, then your
+license from a particular copyright holder is reinstated (a)
+provisionally, unless and until the copyright holder explicitly and
+finally terminates your license, and (b) permanently, if the copyright
+holder fails to notify you of the violation by some reasonable means
+prior to 60 days after the cessation.
+
+  Moreover, your license from a particular copyright holder is
+reinstated permanently if the copyright holder notifies you of the
+violation by some reasonable means, this is the first time you have
+received notice of violation of this License (for any work) from that
+copyright holder, and you cure the violation prior to 30 days after
+your receipt of the notice.
+
+  Termination of your rights under this section does not terminate the
+licenses of parties who have received copies or rights from you under
+this License.  If your rights have been terminated and not permanently
+reinstated, you do not qualify to receive new licenses for the same
+material under section 10.
+
+  9. Acceptance Not Required for Having Copies.
+
+  You are not required to accept this License in order to receive or
+run a copy of the Program.  Ancillary propagation of a covered work
+occurring solely as a consequence of using peer-to-peer transmission
+to receive a copy likewise does not require acceptance.  However,
+nothing other than this License grants you permission to propagate or
+modify any covered work.  These actions infringe copyright if you do
+not accept this License.  Therefore, by modifying or propagating a
+covered work, you indicate your acceptance of this License to do so.
+
+  10. Automatic Licensing of Downstream Recipients.
+
+  Each time you convey a covered work, the recipient automatically
+receives a license from the original licensors, to run, modify and
+propagate that work, subject to this License.  You are not responsible
+for enforcing compliance by third parties with this License.
+
+  An "entity transaction" is a transaction transferring control of an
+organization, or substantially all assets of one, or subdividing an
+organization, or merging organizations.  If propagation of a covered
+work results from an entity transaction, each party to that
+transaction who receives a copy of the work also receives whatever
+licenses to the work the party's predecessor in interest had or could
+give under the previous paragraph, plus a right to possession of the
+Corresponding Source of the work from the predecessor in interest, if
+the predecessor has it or can get it with reasonable efforts.
+
+  You may not impose any further restrictions on the exercise of the
+rights granted or affirmed under this License.  For example, you may
+not impose a license fee, royalty, or other charge for exercise of
+rights granted under this License, and you may not initiate litigation
+(including a cross-claim or counterclaim in a lawsuit) alleging that
+any patent claim is infringed by making, using, selling, offering for
+sale, or importing the Program or any portion of it.
+
+  11. Patents.
+
+  A "contributor" is a copyright holder who authorizes use under this
+License of the Program or a work on which the Program is based.  The
+work thus licensed is called the contributor's "contributor version".
+
+  A contributor's "essential patent claims" are all patent claims
+owned or controlled by the contributor, whether already acquired or
+hereafter acquired, that would be infringed by some manner, permitted
+by this License, of making, using, or selling its contributor version,
+but do not include claims that would be infringed only as a
+consequence of further modification of the contributor version.  For
+purposes of this definition, "control" includes the right to grant
+patent sublicenses in a manner consistent with the requirements of
+this License.
+
+  Each contributor grants you a non-exclusive, worldwide, royalty-free
+patent license under the contributor's essential patent claims, to
+make, use, sell, offer for sale, import and otherwise run, modify and
+propagate the contents of its contributor version.
+
+  In the following three paragraphs, a "patent license" is any express
+agreement or commitment, however denominated, not to enforce a patent
+(such as an express permission to practice a patent or covenant not to
+sue for patent infringement).  To "grant" such a patent license to a
+party means to make such an agreement or commitment not to enforce a
+patent against the party.
+
+  If you convey a covered work, knowingly relying on a patent license,
+and the Corresponding Source of the work is not available for anyone
+to copy, free of charge and under the terms of this License, through a
+publicly available network server or other readily accessible means,
+then you must either (1) cause the Corresponding Source to be so
+available, or (2) arrange to deprive yourself of the benefit of the
+patent license for this particular work, or (3) arrange, in a manner
+consistent with the requirements of this License, to extend the patent
+license to downstream recipients.  "Knowingly relying" means you have
+actual knowledge that, but for the patent license, your conveying the
+covered work in a country, or your recipient's use of the covered work
+in a country, would infringe one or more identifiable patents in that
+country that you have reason to believe are valid.
+
+  If, pursuant to or in connection with a single transaction or
+arrangement, you convey, or propagate by procuring conveyance of, a
+covered work, and grant a patent license to some of the parties
+receiving the covered work authorizing them to use, propagate, modify
+or convey a specific copy of the covered work, then the patent license
+you grant is automatically extended to all recipients of the covered
+work and works based on it.
+
+  A patent license is "discriminatory" if it does not include within
+the scope of its coverage, prohibits the exercise of, or is
+conditioned on the non-exercise of one or more of the rights that are
+specifically granted under this License.  You may not convey a covered
+work if you are a party to an arrangement with a third party that is
+in the business of distributing software, under which you make payment
+to the third party based on the extent of your activity of conveying
+the work, and under which the third party grants, to any of the
+parties who would receive the covered work from you, a discriminatory
+patent license (a) in connection with copies of the covered work
+conveyed by you (or copies made from those copies), or (b) primarily
+for and in connection with specific products or compilations that
+contain the covered work, unless you entered into that arrangement,
+or that patent license was granted, prior to 28 March 2007.
+
+  Nothing in this License shall be construed as excluding or limiting
+any implied license or other defenses to infringement that may
+otherwise be available to you under applicable patent law.
+
+  12. No Surrender of Others' Freedom.
+
+  If conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License.  If you cannot convey a
+covered work so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you may
+not convey it at all.  For example, if you agree to terms that obligate you
+to collect a royalty for further conveying from those to whom you convey
+the Program, the only way you could satisfy both those terms and this
+License would be to refrain entirely from conveying the Program.
+
+  13. Use with the GNU Affero General Public License.
+
+  Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU Affero General Public License into a single
+combined work, and to convey the resulting work.  The terms of this
+License will continue to apply to the part which is the covered work,
+but the special requirements of the GNU Affero General Public License,
+section 13, concerning interaction through a network will apply to the
+combination as such.
+
+  14. Revised Versions of this License.
+
+  The Free Software Foundation may publish revised and/or new versions of
+the GNU General Public License from time to time.  Such new versions will
+be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+  Each version is given a distinguishing version number.  If the
+Program specifies that a certain numbered version of the GNU General
+Public License "or any later version" applies to it, you have the
+option of following the terms and conditions either of that numbered
+version or of any later version published by the Free Software
+Foundation.  If the Program does not specify a version number of the
+GNU General Public License, you may choose any version ever published
+by the Free Software Foundation.
+
+  If the Program specifies that a proxy can decide which future
+versions of the GNU General Public License can be used, that proxy's
+public statement of acceptance of a version permanently authorizes you
+to choose that version for the Program.
+
+  Later license versions may give you additional or different
+permissions.  However, no additional obligations are imposed on any
+author or copyright holder as a result of your choosing to follow a
+later version.
+
+  15. Disclaimer of Warranty.
+
+  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+  16. Limitation of Liability.
+
+  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+SUCH DAMAGES.
+
+  17. Interpretation of Sections 15 and 16.
+
+  If the disclaimer of warranty and limitation of liability provided
+above cannot be given local legal effect according to their terms,
+reviewing courts shall apply local law that most closely approximates
+an absolute waiver of all civil liability in connection with the
+Program, unless a warranty or assumption of liability accompanies a
+copy of the Program in return for a fee.
+
+                     END OF TERMS AND CONDITIONS
+
+            How to Apply These Terms to Your New Programs
+
+  If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these terms.
+
+  To do so, attach the following notices to the program.  It is safest
+to attach them to the start of each source file to most effectively
+state the exclusion of warranty; and each file should have at least
+the "copyright" line and a pointer to where the full notice is found.
+
+    <one line to give the program's name and a brief idea of what it does.>
+    Copyright (C) <year>  <name of author>
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+  If the program does terminal interaction, make it output a short
+notice like this when it starts in an interactive mode:
+
+    <program>  Copyright (C) <year>  <name of author>
+    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+    This is free software, and you are welcome to redistribute it
+    under certain conditions; type `show c' for details.
+
+The hypothetical commands `show w' and `show c' should show the appropriate
+parts of the General Public License.  Of course, your program's commands
+might be different; for a GUI interface, you would use an "about box".
+
+  You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU GPL, see
+<https://www.gnu.org/licenses/>.
+
+  The GNU General Public License does not permit incorporating your program
+into proprietary programs.  If your program is a subroutine library, you
+may consider it more useful to permit linking proprietary applications with
+the library.  If this is what you want to do, use the GNU Lesser General
+Public License instead of this License.  But first, please read
+<https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `baca2-package-manager-0.2.2/PKG-INFO` & `baca2-package-manager-0.2.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1
-Name: baca2-package-manager
-Version: 0.2.2
-Summary: A package manager for Baca2 project
-Home-page: https://github.com/BaCa2-project/BaCa2-package-manager
-Author: Baca2 Team
-Author-email: bartosz.deptula@student.uj.edu.pl
-Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# BaCa2-package-manager
-_Package manager for BaCa2 (to be exported as PyPI package)._
-
-Package manager designed to automatically interpret and work with task packages for BaCa2 checker.
-It is needed for every kind of broker, and BaCa2 itself.
+Metadata-Version: 2.1
+Name: baca2-package-manager
+Version: 0.2.3
+Summary: A package manager for Baca2 project
+Home-page: https://github.com/BaCa2-project/BaCa2-package-manager
+Author: Baca2 Team
+Author-email: bartosz.deptula@student.uj.edu.pl
+Classifier: Programming Language :: Python :: 3
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# BaCa2-package-manager
+_Package manager for BaCa2 (to be exported as PyPI package)._
+
+Package manager designed to automatically interpret and work with task packages for BaCa2 checker.
+It is needed for every kind of broker, and BaCa2 itself.
```

### Comparing `baca2-package-manager-0.2.2/baca2PackageManager/__init__.py` & `baca2-package-manager-0.2.3/baca2PackageManager/__init__.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-from .manager import *
-from pathlib import Path
-
-import baca2PackageManager.consts as consts
-
-
-def base_dir() -> Path:
-    """
-    Get base directory for package manager.
-
-    :return: A path to directory.
-    """
-    if consts.BASE_DIR is None:
-        raise ValueError("Base directory is not set")
-    return consts.BASE_DIR
-
-
-def set_base_dir(path: Path):
-    """
-    Set base directory for package manager.
-
-    :param path: A path to directory.
-    :return: None.
-    """
-    consts.BASE_DIR = path
-
-
-def add_supported_extensions(*args):
-    """
-    Add supported extensions for package manager.
-
-    :param args: A list of extensions.
-    :return: None.
-    """
-    consts.SUPPORTED_EXTENSIONS.extend(args)
+from .manager import *
+from pathlib import Path
+
+import baca2PackageManager.consts as consts
+
+
+def base_dir() -> Path:
+    """
+    Get base directory for package manager.
+
+    :return: A path to directory.
+    """
+    if consts.BASE_DIR is None:
+        raise ValueError("Base directory is not set")
+    return consts.BASE_DIR
+
+
+def set_base_dir(path: Path):
+    """
+    Set base directory for package manager.
+
+    :param path: A path to directory.
+    :return: None.
+    """
+    consts.BASE_DIR = path
+
+
+def add_supported_extensions(*args):
+    """
+    Add supported extensions for package manager.
+
+    :param args: A list of extensions.
+    :return: None.
+    """
+    consts.SUPPORTED_EXTENSIONS.extend(args)
```

### Comparing `baca2-package-manager-0.2.2/baca2PackageManager/manager.py` & `baca2-package-manager-0.2.3/baca2PackageManager/manager.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,678 +1,681 @@
-from copy import deepcopy
-from pathlib import Path
-from os import remove, replace, walk, mkdir, rename, listdir
-from shutil import rmtree, copytree
-from yaml import safe_load, dump
-from re import match
-
-from .validators import isAny, isNone, isInt, isIntBetween, isFloat, isFloatBetween, isStr, is_, isIn, isShorter, \
-    isDict, isPath, isSize, isList, memory_converting, valid_memory_size, isBool
-from .consts import SUPPORTED_EXTENSIONS, BASE_DIR
-from .manager_exceptions import NoTestFound, NoSetFound, TestExistError
-
-__all__ = ['Package', 'TSet', 'TestF']
-
-def merge_settings(default: dict, to_add: dict) -> dict:
-    """
-    It takes two dictionaries, and returns a new dictionary that has the keys of the first dictionary, and the values of the
-    second dictionary if they exist, otherwise the values of the first dictionary. It overwrites default dict with valuses from to_add
-
-    :param default: The default settings
-    :type default: dict
-    :param to_add: The settings you want to add to the default settings
-    :type to_add: dict
-
-    :return: A dictionary with the keys of the default dictionary and the values of the to_add dictionary.
-    """
-    new = {}
-    for i in default.keys():
-        if to_add is not None:
-            if i in to_add.keys() and to_add[i] is not None:
-                new[i] = to_add[i]
-            else:
-                new[i] = default[i]
-        else:
-            new[i] = default[i]
-    return new
-
-
-class PackageManager:
-    """
-    It's a class that manages a package's settings
-    """
-    def __init__(self, path: Path, settings_init: Path or dict, default_settings: dict):
-        """
-        If the settings_init is a dict, assign it to settings. If not, load the settings_init yaml file and assign it to
-        settings. Then merge the settings with the default settings
-
-        :param path: Path to the settings file
-        :type path: Path
-        :param settings_init: This is the path to the settings file
-        :type settings_init: Path or dict
-        :param default_settings: a dict with default settings
-        :type default_settings: dict
-        """
-        self._path = path
-        # if type of settings_init is a dict assign settings_init to processed settings
-        settings = {}
-        if type(settings_init) == dict:
-            if bool(settings_init):
-                settings = settings_init
-        # if not, make dict from settings_init yaml
-        else:
-            # unpacking settings file to dict
-            with open(settings_init, mode="rt", encoding="utf-8") as file:
-                settings = safe_load(file)
-        # merge external settings with default
-        self._settings = merge_settings(default_settings, settings)
-
-    def __getitem__(self, arg: str):
-        """
-        If the key is in the dictionary, return the value. If not, raise a KeyError
-
-        :param arg: The name of the key to get the value of
-        :type arg: str
-
-        :return: The value of the key in the dictionary.
-        """
-        try:
-            return self._settings[arg]
-        except KeyError:
-            raise KeyError(f'No key named {arg} has found in self_settings')
-
-    def __setitem__(self, arg: str, val):
-        """
-        `__setitem__` is a special method that allows us to use the `[]` operator to set a value in a dictionary
-
-        :param arg: str
-        :type arg: str
-        :param val: the value to be set
-        """
-        self._settings[arg] = val
-        # effect changes to yaml settings
-        self.save_to_config(self._settings)
-
-    def check_validation(self, validators) -> bool:
-        """
-        It checks if the value of the setting is valid by checking if it matches any of the validators for that setting
-
-        :param validators: A dictionary of validators. The keys are the names of the settings, and the values are lists of
-        validators. Each validator is a tuple of the form (function, *args, **kwargs). The function is called with the
-        setting value as the first argument, followed by the *
-
-        :return: The check variable is being returned.
-        """
-        for i, j in self._settings.items():
-            check = False
-            for k in validators[i]:
-                check |= k[0](j, *k[1:])
-        return check
-
-    def save_to_config(self, settings):
-        """
-        It opens a file called config.yml in the directory specified by the path attribute of the object, and writes the
-        settings dictionary to it.
-
-        :param settings: The settings to save
-        """
-        with open(self._path / 'config.yml', mode="wt", encoding="utf-8") as file:
-            dump(settings, file)
-
-    def read_from_config(self):
-        """
-        It reads the config.yml file from the path and returns the contents
-
-        :return: The dict from config.yml file is being returned.
-        """
-        with open(self._path / 'config.yml', mode="rt", encoding="utf-8") as file:
-            return safe_load(file)
-
-    def add_empty_file(self, filename):
-        """
-        It creates an empty file if it doesn't already exist
-
-        :param filename: The name of the file to be created
-        """
-        if not isPath(self._path / filename):
-            with open(self._path / filename, 'w') as f:
-                pass
-
-
-class Package(PackageManager):
-    """
-    It's a class that represents a package.
-    """
-
-    #: Largest file acceptable to upload
-    MAX_SUBMIT_MEMORY = '10G'
-    #: Largest acceptable submit time
-    MAX_SUBMIT_TIME = 600
-    MAX_CPUS = 16
-    SETTINGS_VALIDATION = {
-        'title': [[isStr]],
-        'points': [[isInt], [isFloat]],
-        'memory_limit': [[isSize, MAX_SUBMIT_MEMORY]],
-        'time_limit': [[isIntBetween, 0, MAX_SUBMIT_TIME], [isFloatBetween, 0, MAX_SUBMIT_TIME]],
-        'allowedExtensions': [[isIn, *SUPPORTED_EXTENSIONS], [isList, [isIn, *SUPPORTED_EXTENSIONS]]],
-        'hinter': [[isNone], [isPath]],
-        'checker': [[isNone], [isPath]],
-        'test_generator': [[isNone], [isPath]],
-        'network': [[isNone], [isBool]],
-        'cpus': [[isNone], [isIntBetween, 1, MAX_CPUS]]
-    }
-    """
-    Validation for ``Package`` settings.
-    
-    Available options are:
-    
-        * ``title``: package name
-        * ``points``: maximum amount of points to earn
-        * ``memory_limit``: is a memory limit
-        * ``time_limit``: is a time limit
-        * ``allowedExtensions``: extensions witch are accepted
-        * ``hinter``: is a path or None value to actual hinter
-        * ``checker``: is a path or None value to actual checker
-        * ``test_generator``: is a path or None value to actual generator
-        * ``network``: is a bool value to allow network access
-        * ``cpus``: is a number of cpus to use
-    """
-
-    #: Default values for Package settings
-    DEFAULT_SETTINGS = {
-        'title': 'p',
-        'points': 0,
-        'memory_limit': '512M',
-        'time_limit': 10,
-        'allowedExtensions': 'cpp',
-        'hinter': None,
-        'checker': None,
-        'test_generator': None,
-        'network': False,
-        'cpus': 1
-    }
-
-    def __init__(self, path: Path, commit: str) -> None:
-        """
-        It takes a path to a folder, and then it creates a list of all the subfolders in that folder, and then it creates a
-        TSet object for each of those subfolders
-
-        :param path: Path - the path to the package
-        :type path: Path
-        """
-        self._path = path
-        self._commit = commit
-
-        config_path = self.commit_path / 'config.yml'
-        sets_path = self.commit_path / 'tests'
-        super().__init__(path, config_path, Package.DEFAULT_SETTINGS)
-        print(sets_path)
-        self._sets = []
-        for i in [x[0].replace(str(sets_path) + '\\', '') for x in walk(sets_path)][1:]:
-            self._sets.append(TSet(sets_path / i))
-
-    def prepare_build(self, build_name: str):
-        """
-        It prepares the build
-
-        :param build_name: The name of the build
-        :type build_name: str
-        """
-        if not (self.commit_path / '.build').is_dir():
-            mkdir(self.commit_path / '.build')
-
-        if not (self.commit_path / '.build' / build_name).is_dir():
-            mkdir(self.commit_path / '.build' / build_name)
-
-        return self.commit_path / '.build' / build_name
-
-    def check_build(self, build_name: str):
-        """
-        It checks if the build exists
-
-        :param build_name: The name of the build
-        :type build_name: str
-        """
-        build_dir = self.commit_path / '.build' / build_name
-
-        if not build_dir.is_dir():
-            return False
-
-        return any(list(walk(build_dir))[0][1:])
-
-    def delete_build(self, build_name: str = None):
-        """
-        Deletes the build. If build_name is None, it deletes all builds.
-
-        :param build_name: The name of the build, if None, it clears all builds
-        :type build_name: str
-        """
-        if build_name is None:
-            rmtree(self.commit_path / '.build')
-        else:
-            rmtree(self.commit_path / '.build' / build_name)
-
-    @property
-    def commit_path(self) -> Path:
-        """
-        It returns the path to the commit
-        TODO: After implementing internal git system, this should be changed
-
-        :return: The path to the commit
-        :rtype: Path
-        """
-        return self._path / self._commit
-
-    def rm_tree(self, set_name):
-        """
-        It removes a directory tree
-
-        :param set_name: The name of the test set
-        """
-        if isPath(self.commit_path / 'tests' / set_name):
-            rmtree(self.commit_path / 'tests' / set_name)
-
-    def make_commit(self, new_commit: str) -> 'Package':
-        """
-        Function copies the package instance and creates new one/
-
-        :param new_path: The path of the package
-        :param new_commit: New unique commit
-
-        :return: new Package
-        """
-        new_commit_path = self._path / new_commit
-        copytree(self.commit_path, new_commit_path)
-        return Package(self._path, new_commit)
-
-    def delete(self) -> None:
-        """
-        Function deletes the package (itself) from directory
-
-        :return: None
-        """
-        rmtree(self.commit_path)
-        del self
-
-    def _add_new_set(self, set_name) -> 'TSet':
-        """
-        This function adds a new test set to the test suite
-
-        :param set_name: The name of the new test set
-
-        :return: A new TSet object.
-        """
-        settings = {'name': set_name} | self._settings
-        set_path = self.commit_path / 'tests' / set_name
-        if not isPath(set_path):
-            mkdir(set_path)
-            with open(set_path / 'config.yml', 'w') as file:
-                dump({'name': set_name}, file)
-        new_set = TSet(set_path)
-        self._sets.append(new_set)
-        return new_set
-
-    def sets(self, set_name: str, add_new: bool = False) -> 'TSet':
-        """
-        It returns the set with the name `set_name` if it exists, otherwise it raises an error
-
-        :param set_name: The name of the set you want to get
-        :type set_name: str
-        :param add_new: If True, it will create a new set directory if it doesn't exist, defaults to False
-        :type add_new: bool (optional)
-
-        :return: The set with the name set_name
-        """
-        for i in self._sets:
-            if i['name'] == set_name:
-                return i
-        if add_new:
-            self._add_new_set(set_name)
-        else:
-            raise NoSetFound(f'Any set directory named {set_name} has found')
-
-    def delete_set(self, set_name: str):
-        """
-        It deletes a set from the sets list and removes the directory of the set
-
-        :param set_name: The name of the set you want to delete
-        :type set_name: str
-        :return: the list of sets.
-        """
-        for i in self._sets:
-            if i['name'] == set_name:
-                self._sets.remove(i)
-                self.rm_tree(set_name)
-                return
-        raise NoSetFound(f'Any set directory named {set_name} has found to delete')
-
-    def check_package(self, subtree: bool = True) -> bool | int:
-        """
-        It checks the package.
-
-        :param subtree: bool = True, defaults to True
-        :type subtree: bool (optional)
-        :return: The result of the check_validation() method and the result of the check_set() method.
-        """
-        result = True
-        if subtree:
-            for i in self._sets:
-                result &= i.check_set()
-        return self.check_validation(Package.SETTINGS_VALIDATION) & result
-
-
-class TSet(PackageManager):
-    """
-    It's a class that represents a set of tests and modifies it
-    """
-    SETTINGS_VALIDATION = {
-        'name': [[isStr]],
-        'weight': [[isInt], [isFloat]],
-        'points': [[isInt], [isFloat]],
-        'memory_limit': [[isNone], [isSize, Package.MAX_SUBMIT_MEMORY]],
-        'time_limit': [[isNone], [isIntBetween, 0, Package.MAX_SUBMIT_TIME],
-                       [isFloatBetween, 0, Package.MAX_SUBMIT_TIME]],
-        'checker': [[isNone], [isPath]],
-        'test_generator': [[isNone], [isPath]],
-        'tests': [[isNone], [isAny]],
-        'makefile': [[isNone], [isPath]]
-    }
-
-    """
-        Validation for ``TSet`` settings.
-
-        Available options are:
-            * ``name``: set name
-            * ``weight``: impact of set score on final score
-            * ``points``: maximum amount of points to earn in set
-            * ``memory_limit``: is a memory limit for set
-            * ``time_limit``: is a time limit for set
-            * ``checker``: is a path or None value to actual checker
-            * ``test_generator``: is a path or None value to actual generator
-            * ``tests``: tests to run in set
-            * ``makefile``: name of a makefile
-        """
-    #: Default values for set settings
-    DEFAULT_SETTINGS = {
-        'name': 'set0',
-        'weight': 10,
-        'points': 0,
-        'memory_limit': '512M',
-        'time_limit': 10,
-        'checker': None,
-        'test_generator': None,
-        'tests': {},
-        'makefile': None
-    }
-
-    def __init__(self, path: Path):
-        """
-        It reads the config file and creates a list of tests
-
-        :param path: Path - path to the test set
-        :type path: Path
-        """
-        config_path = path / 'config.yml'
-        super().__init__(path, config_path, TSet.DEFAULT_SETTINGS)
-        self._tests = []
-        self._test_settings = {
-            'name': '0',
-            'memory_limit': self._settings['memory_limit'],
-            'time_limit': self._settings['time_limit'],
-            'points': 0
-        }
-        if self._settings['tests'] is not None:
-            for i in self._settings['tests'].values():
-                self._tests.append(TestF(path, i, self._test_settings))
-        self._add_test_from_dir()
-
-    def move_test_file(self, to_set, filename):
-        """
-        It moves a file from one directory to another
-
-        :param to_set: the set you want to move the file to
-        :param filename: the name of the file to move
-        """
-        if isPath(to_set._path):
-            if isPath(self._path / filename):
-                replace(self._path / filename, to_set._path / filename)
-
-    def _add_test_from_dir(self):
-        """
-        It takes a directory, finds all the files in it, and then adds all the tests that have both an input and output file
-        """
-        test_files_ext = listdir(self._path)
-        tests = []
-        for i in test_files_ext:
-            tests.append(match('.*[^.in|out]', i).group(0))
-        tests_to_do = []
-        for i in tests:
-            if tests.count(i) == 2:
-                tests_to_do.append(i)
-        tests_to_do = set(tests_to_do)
-        names = [i["name"] for i in self._tests]
-        for i in tests_to_do:
-            if i not in names:
-                name_dict = {'name': i}
-                self._tests.append(TestF(self._path, name_dict, self._test_settings))
-
-    def tests(self, test_name: str, add_new: bool = False) -> 'TestF':
-        """
-        It returns a test object with the given name, if it exists, or creates a new one if it doesn't
-
-        :param test_name: The name of the test
-        :type test_name: str
-        :param add_new: if True, then if the test is not found, it will be created, defaults to False
-        :type add_new: bool (optional)
-
-        :return: A TestF object
-        """
-        for i in self._tests:
-            if i['name'] == test_name:
-                return i
-        if add_new:
-            new_test = TestF(self._path, {'name': test_name}, self._test_settings)
-            self._tests.append(new_test)
-            self.add_empty_file(test_name + '.in')
-            self.add_empty_file(test_name + '.out')
-            return new_test
-        raise NoTestFound(f'Any test named {test_name} has found')
-
-    def remove_file(self, filename):
-        """
-        It removes a file from the current directory
-
-        :param filename: The name of the file to remove
-        """
-        if isPath(self._path / filename):
-            remove(self._path / filename)
-
-    def _delete_chosen_test(self, test: 'TestF'):
-        """
-        It removes the test from the list of tests, deletes the files associated with the test,
-        and removes the test from the config file
-
-        :param test: the test to be deleted
-        :type test: 'TestF'
-        """
-        self._tests.remove(test)
-        self.remove_file(test['name'] + '.in')
-        self.remove_file(test['name'] + '.out')
-
-        # removes settings for this test (from _settings and from config file)
-        new_settings = deepcopy(self._settings)
-        for k, v in self._settings['tests'].items():
-            if v['name'] == test['name']:
-                new_settings['tests'].pop(k)
-        self._settings = new_settings
-        self.save_to_config(self._settings)
-
-    def delete_test(self, test_name: str):
-        """
-        It deletes a test from the list of tests, and deletes associated files.
-
-        :param test_name: The name of the test to delete
-        :type test_name: str
-        :raise NoTestsFound: If there is no test with name equal to the test_name argument.
-        """
-        for test in self._tests:
-            if test['name'] == test_name:
-                self._delete_chosen_test(test)
-                return
-
-        raise NoTestFound(f'No test named {test_name} has found to delete')
-
-    def _move_chosen_test(self, test: 'TestF', to_set: 'TSet'):
-        """
-         Move a test from one test set to another
-
-        :param test: 'TestF' - the test to be moved
-        :type test: 'TestF'
-        :param to_set: the set to which the test will be moved
-        :type to_set: 'TSet'
-        """
-        name_list_ta = [j['name'] for j in to_set._tests]
-        if test['name'] not in name_list_ta:
-            to_set._tests.append(test)
-            self._tests.remove(test)
-        else:
-            raise TestExistError(f'Test named {test["name"]} exist in to_set files')
-
-        self.move_test_file(to_set, test['name'] + '.in')
-        self.move_test_file(to_set, test['name'] + '.out')
-
-    def _move_config(self, to_set: 'TSet', test_name: str):
-        """
-        It takes a test name and a set object, and moves the test from the current set to the set object
-
-        :param to_set: The set to move the test to
-        :type to_set: 'TSet'
-        :param test_name: The name of the test you want to move
-        :type test_name: str
-        """
-        new_settings = deepcopy(self._settings)
-        for i, j in self._settings['tests'].items():
-            if j['name'] == test_name:
-                to_set._settings['tests'][i] = j
-                new_settings['tests'].pop(i)
-
-        self._settings = new_settings
-        self.remove_file('config.yml')
-        self.save_to_config(self._settings)
-        to_set.remove_file('config.yml')
-        to_set.save_to_config(to_set._settings)
-
-    # moves test to to_set (and all settings pinned to this test in self._settings)
-    def move_test(self, test_name: str, to_set: 'TSet'):
-        """
-        It moves a test from one set to another
-
-        :param test_name: The name of the test to move
-        :type test_name: str
-        :param to_set: The set to which the test will be moved
-        :type to_set: 'TSet'
-        """
-        search = False
-        for i in self._tests:
-            if i['name'] == test_name:
-                self._move_chosen_test(i,  to_set)
-                self._move_config(to_set, test_name)
-                search |= True
-                return
-            search |= False
-
-        if not search:
-            raise NoTestFound(f'Any test named {test_name} has found to move to to_set')
-
-    # check set validation
-    def check_set(self, subtree=True) -> bool | int:
-        """
-        It checks the set.
-
-        :param subtree: If True, check the subtree of tests, defaults to True (optional)
-
-        :return: The result of the check_validation() method and the result of the check_set() method.
-        """
-        result = True
-        if subtree:
-            for i in self._tests:
-                result &= i.check_test()
-
-        return self.check_validation(TSet.SETTINGS_VALIDATION) & result
-
-
-class TestF(PackageManager):
-    """
-    It's a class that represents test in a set.
-    """
-    SETTINGS_VALIDATION = {
-        'name': [[isStr]],
-        'memory_limit': [[isNone], [isSize, Package.MAX_SUBMIT_MEMORY]],
-        'time_limit': [[isNone], [isIntBetween, 0, Package.MAX_SUBMIT_TIME],
-                       [isFloatBetween, 0, Package.MAX_SUBMIT_TIME]],
-        'points': [[isInt], [isFloat]]
-    }
-    """
-       Validation for ``TestF`` settings.
-
-       Available options are:
-        * ``name``: test name
-        * ``points``: maximum amount of points to earn in test
-        * ``memory_limit``: is a memory limit for test
-        * ``time_limit``: is a time limit for test
-       """
-
-    def __init__(self, path: Path, additional_settings: dict or Path, default_settings: dict):
-        """
-        This function initializes the class by calling the superclass's __init__ function, which is the __init__ function of
-        the Config class
-
-        :param path: The path to the file that contains the settings
-        :type path: Path
-        :param additional_settings: This is a dictionary of settings that you want to override the default settings with
-        :type additional_settings: dict or Path
-        :param default_settings: This is a dictionary of default settings that will be used if the settings file doesn't
-        contain a value for a setting
-        :type default_settings: dict
-        """
-        super().__init__(path, additional_settings, default_settings)
-
-    def _rename_files(self, old_name, new_name):
-        """
-        It renames a file
-
-        :param old_name: The name of the file you want to rename
-        :param new_name: The new name of the file
-        """
-        rename(self._path / old_name, self._path / new_name)
-
-    def __setitem__(self, arg: str, val):
-        """
-        It renames the files and changes the name in the yaml file
-
-        :param arg: the key of the dictionary
-        :type arg: str
-        :param val: the new value
-        """
-        # effect changes to yaml settings
-        settings = self.read_from_config()
-        if arg == 'name':
-            self._rename_files(self._settings['name'] + '.in', val + '.in')
-            self._rename_files(self._settings['name'] + '.out', val + '.out')
-
-            for i, j in settings['tests'].items():
-                if j['name'] == self._settings['name']:
-                    new_key = 'test' + val
-                    j[arg] = val
-                    settings['tests'][new_key] = j
-                    del settings['tests'][i]
-                    break
-
-        self.save_to_config(settings)
-        self._settings[arg] = val
-
-    def check_test(self) -> bool:
-        """
-        It checks if the test is valid
-        :return: The return value is the result of the check_validation method.
-        """
-        return self.check_validation(TestF.SETTINGS_VALIDATION)
+import shutil
+from copy import deepcopy
+from pathlib import Path
+from os import remove, replace, walk, mkdir, rename, listdir
+from shutil import rmtree, copytree
+from yaml import safe_load, dump
+from re import match
+
+from .validators import isAny, isNone, isInt, isIntBetween, isFloat, isFloatBetween, isStr, is_, isIn, isShorter, \
+    isDict, isPath, isSize, isList, memory_converting, valid_memory_size, isBool
+from .consts import SUPPORTED_EXTENSIONS, BASE_DIR
+from .manager_exceptions import NoTestFound, NoSetFound, TestExistError
+
+__all__ = ['Package', 'TSet', 'TestF']
+
+def merge_settings(default: dict, to_add: dict) -> dict:
+    """
+    It takes two dictionaries, and returns a new dictionary that has the keys of the first dictionary, and the values of the
+    second dictionary if they exist, otherwise the values of the first dictionary. It overwrites default dict with valuses from to_add
+
+    :param default: The default settings
+    :type default: dict
+    :param to_add: The settings you want to add to the default settings
+    :type to_add: dict
+
+    :return: A dictionary with the keys of the default dictionary and the values of the to_add dictionary.
+    """
+    new = {}
+    for i in default.keys():
+        if to_add is not None:
+            if i in to_add.keys() and to_add[i] is not None:
+                new[i] = to_add[i]
+            else:
+                new[i] = default[i]
+        else:
+            new[i] = default[i]
+    return new
+
+
+class PackageManager:
+    """
+    It's a class that manages a package's settings
+    """
+    def __init__(self, path: Path, settings_init: Path or dict, default_settings: dict):
+        """
+        If the settings_init is a dict, assign it to settings. If not, load the settings_init yaml file and assign it to
+        settings. Then merge the settings with the default settings
+
+        :param path: Path to the settings file
+        :type path: Path
+        :param settings_init: This is the path to the settings file
+        :type settings_init: Path or dict
+        :param default_settings: a dict with default settings
+        :type default_settings: dict
+        """
+        self._path = path
+        # if type of settings_init is a dict assign settings_init to processed settings
+        settings = {}
+        if type(settings_init) == dict:
+            if bool(settings_init):
+                settings = settings_init
+        # if not, make dict from settings_init yaml
+        else:
+            # unpacking settings file to dict
+            with open(settings_init, mode="rt", encoding="utf-8") as file:
+                settings = safe_load(file)
+        # merge external settings with default
+        self._settings = merge_settings(default_settings, settings)
+
+    def __getitem__(self, arg: str):
+        """
+        If the key is in the dictionary, return the value. If not, raise a KeyError
+
+        :param arg: The name of the key to get the value of
+        :type arg: str
+
+        :return: The value of the key in the dictionary.
+        """
+        try:
+            return self._settings[arg]
+        except KeyError:
+            raise KeyError(f'No key named {arg} has found in self_settings')
+
+    def __setitem__(self, arg: str, val):
+        """
+        `__setitem__` is a special method that allows us to use the `[]` operator to set a value in a dictionary
+
+        :param arg: str
+        :type arg: str
+        :param val: the value to be set
+        """
+        self._settings[arg] = val
+        # effect changes to yaml settings
+        self.save_to_config(self._settings)
+
+    def check_validation(self, validators) -> bool:
+        """
+        It checks if the value of the setting is valid by checking if it matches any of the validators for that setting
+
+        :param validators: A dictionary of validators. The keys are the names of the settings, and the values are lists of
+        validators. Each validator is a tuple of the form (function, *args, **kwargs). The function is called with the
+        setting value as the first argument, followed by the *
+
+        :return: The check variable is being returned.
+        """
+        for i, j in self._settings.items():
+            check = False
+            for k in validators[i]:
+                check |= k[0](j, *k[1:])
+        return check
+
+    def save_to_config(self, settings):
+        """
+        It opens a file called config.yml in the directory specified by the path attribute of the object, and writes the
+        settings dictionary to it.
+
+        :param settings: The settings to save
+        """
+        with open(self._path / 'config.yml', mode="wt", encoding="utf-8") as file:
+            dump(settings, file)
+
+    def read_from_config(self):
+        """
+        It reads the config.yml file from the path and returns the contents
+
+        :return: The dict from config.yml file is being returned.
+        """
+        with open(self._path / 'config.yml', mode="rt", encoding="utf-8") as file:
+            return safe_load(file)
+
+    def add_empty_file(self, filename):
+        """
+        It creates an empty file if it doesn't already exist
+
+        :param filename: The name of the file to be created
+        """
+        if not isPath(self._path / filename):
+            with open(self._path / filename, 'w') as f:
+                pass
+
+
+class Package(PackageManager):
+    """
+    It's a class that represents a package.
+    """
+
+    #: Largest file acceptable to upload
+    MAX_SUBMIT_MEMORY = '10G'
+    #: Largest acceptable submit time
+    MAX_SUBMIT_TIME = 600
+    MAX_CPUS = 16
+    SETTINGS_VALIDATION = {
+        'title': [[isStr]],
+        'points': [[isInt], [isFloat]],
+        'memory_limit': [[isSize, MAX_SUBMIT_MEMORY]],
+        'time_limit': [[isIntBetween, 0, MAX_SUBMIT_TIME], [isFloatBetween, 0, MAX_SUBMIT_TIME]],
+        'allowedExtensions': [[isIn, *SUPPORTED_EXTENSIONS], [isList, [isIn, *SUPPORTED_EXTENSIONS]]],
+        'hinter': [[isNone], [isPath]],
+        'checker': [[isNone], [isPath]],
+        'test_generator': [[isNone], [isPath]],
+        'network': [[isNone], [isBool]],
+        'cpus': [[isNone], [isIntBetween, 1, MAX_CPUS]]
+    }
+    """
+    Validation for ``Package`` settings.
+    
+    Available options are:
+    
+        * ``title``: package name
+        * ``points``: maximum amount of points to earn
+        * ``memory_limit``: is a memory limit
+        * ``time_limit``: is a time limit
+        * ``allowedExtensions``: extensions witch are accepted
+        * ``hinter``: is a path or None value to actual hinter
+        * ``checker``: is a path or None value to actual checker
+        * ``test_generator``: is a path or None value to actual generator
+        * ``network``: is a bool value to allow network access
+        * ``cpus``: is a number of cpus to use
+    """
+
+    #: Default values for Package settings
+    DEFAULT_SETTINGS = {
+        'title': 'p',
+        'points': 0,
+        'memory_limit': '512M',
+        'time_limit': 10,
+        'allowedExtensions': 'cpp',
+        'hinter': None,
+        'checker': None,
+        'test_generator': None,
+        'network': False,
+        'cpus': 1
+    }
+
+    def __init__(self, path: Path, commit: str) -> None:
+        """
+        It takes a path to a folder, and then it creates a list of all the subfolders in that folder, and then it creates a
+        TSet object for each of those subfolders
+
+        :param path: Path - the path to the package
+        :type path: Path
+        """
+        self._path = path
+        self._commit = commit
+
+        config_path = self.commit_path / 'config.yml'
+        sets_path = self.commit_path / 'tests'
+        super().__init__(path, config_path, Package.DEFAULT_SETTINGS)
+        self._sets = []
+        for i in [x[0].replace(str(sets_path) + '\\', '') for x in walk(sets_path)][1:]:
+            self._sets.append(TSet(sets_path / i))
+
+    def prepare_build(self, build_name: str):
+        """
+        It prepares the build
+
+        :param build_name: The name of the build
+        :type build_name: str
+        """
+        if not (self.commit_path / '.build').is_dir():
+            mkdir(self.commit_path / '.build')
+
+        build_dir = self.commit_path / '.build' / build_name
+
+        if build_dir.is_dir():
+            rmtree(build_dir)
+        mkdir(build_dir)
+
+        return build_dir
+
+    def check_build(self, build_name: str):
+        """
+        It checks if the build exists
+
+        :param build_name: The name of the build
+        :type build_name: str
+        """
+        build_dir = self.commit_path / '.build' / build_name
+
+        if not build_dir.is_dir():
+            return False
+
+        return any(list(walk(build_dir))[0][1:])
+
+    def delete_build(self, build_name: str = None):
+        """
+        Deletes the build. If build_name is None, it deletes all builds.
+
+        :param build_name: The name of the build, if None, it clears all builds
+        :type build_name: str
+        """
+        if build_name is None:
+            rmtree(self.commit_path / '.build')
+        else:
+            rmtree(self.commit_path / '.build' / build_name)
+
+    @property
+    def commit_path(self) -> Path:
+        """
+        It returns the path to the commit
+        TODO: After implementing internal git system, this should be changed
+
+        :return: The path to the commit
+        :rtype: Path
+        """
+        return self._path / self._commit
+
+    def rm_tree(self, set_name):
+        """
+        It removes a directory tree
+
+        :param set_name: The name of the test set
+        """
+        if isPath(self.commit_path / 'tests' / set_name):
+            rmtree(self.commit_path / 'tests' / set_name)
+
+    def make_commit(self, new_commit: str) -> 'Package':
+        """
+        Function copies the package instance and creates new one/
+
+        :param new_path: The path of the package
+        :param new_commit: New unique commit
+
+        :return: new Package
+        """
+        new_commit_path = self._path / new_commit
+        copytree(self.commit_path, new_commit_path)
+        return Package(self._path, new_commit)
+
+    def delete(self) -> None:
+        """
+        Function deletes the package (itself) from directory
+
+        :return: None
+        """
+        rmtree(self.commit_path)
+        del self
+
+    def _add_new_set(self, set_name) -> 'TSet':
+        """
+        This function adds a new test set to the test suite
+
+        :param set_name: The name of the new test set
+
+        :return: A new TSet object.
+        """
+        settings = {'name': set_name} | self._settings
+        set_path = self.commit_path / 'tests' / set_name
+        if not isPath(set_path):
+            mkdir(set_path)
+            with open(set_path / 'config.yml', 'w') as file:
+                dump({'name': set_name}, file)
+        new_set = TSet(set_path)
+        self._sets.append(new_set)
+        return new_set
+
+    def sets(self, set_name: str, add_new: bool = False) -> 'TSet':
+        """
+        It returns the set with the name `set_name` if it exists, otherwise it raises an error
+
+        :param set_name: The name of the set you want to get
+        :type set_name: str
+        :param add_new: If True, it will create a new set directory if it doesn't exist, defaults to False
+        :type add_new: bool (optional)
+
+        :return: The set with the name set_name
+        """
+        for i in self._sets:
+            if i['name'] == set_name:
+                return i
+        if add_new:
+            self._add_new_set(set_name)
+        else:
+            raise NoSetFound(f'Any set directory named {set_name} has found')
+
+    def delete_set(self, set_name: str):
+        """
+        It deletes a set from the sets list and removes the directory of the set
+
+        :param set_name: The name of the set you want to delete
+        :type set_name: str
+        :return: the list of sets.
+        """
+        for i in self._sets:
+            if i['name'] == set_name:
+                self._sets.remove(i)
+                self.rm_tree(set_name)
+                return
+        raise NoSetFound(f'Any set directory named {set_name} has found to delete')
+
+    def check_package(self, subtree: bool = True) -> bool | int:
+        """
+        It checks the package.
+
+        :param subtree: bool = True, defaults to True
+        :type subtree: bool (optional)
+        :return: The result of the check_validation() method and the result of the check_set() method.
+        """
+        result = True
+        if subtree:
+            for i in self._sets:
+                result &= i.check_set()
+        return self.check_validation(Package.SETTINGS_VALIDATION) & result
+
+
+class TSet(PackageManager):
+    """
+    It's a class that represents a set of tests and modifies it
+    """
+    SETTINGS_VALIDATION = {
+        'name': [[isStr]],
+        'weight': [[isInt], [isFloat]],
+        'points': [[isInt], [isFloat]],
+        'memory_limit': [[isNone], [isSize, Package.MAX_SUBMIT_MEMORY]],
+        'time_limit': [[isNone], [isIntBetween, 0, Package.MAX_SUBMIT_TIME],
+                       [isFloatBetween, 0, Package.MAX_SUBMIT_TIME]],
+        'checker': [[isNone], [isPath]],
+        'test_generator': [[isNone], [isPath]],
+        'tests': [[isNone], [isAny]],
+        'makefile': [[isNone], [isPath]]
+    }
+
+    """
+        Validation for ``TSet`` settings.
+
+        Available options are:
+            * ``name``: set name
+            * ``weight``: impact of set score on final score
+            * ``points``: maximum amount of points to earn in set
+            * ``memory_limit``: is a memory limit for set
+            * ``time_limit``: is a time limit for set
+            * ``checker``: is a path or None value to actual checker
+            * ``test_generator``: is a path or None value to actual generator
+            * ``tests``: tests to run in set
+            * ``makefile``: name of a makefile
+        """
+    #: Default values for set settings
+    DEFAULT_SETTINGS = {
+        'name': 'set0',
+        'weight': 10,
+        'points': 0,
+        'memory_limit': '512M',
+        'time_limit': 10,
+        'checker': None,
+        'test_generator': None,
+        'tests': {},
+        'makefile': None
+    }
+
+    def __init__(self, path: Path):
+        """
+        It reads the config file and creates a list of tests
+
+        :param path: Path - path to the test set
+        :type path: Path
+        """
+        config_path = path / 'config.yml'
+        super().__init__(path, config_path, TSet.DEFAULT_SETTINGS)
+        self._tests = []
+        self._test_settings = {
+            'name': '0',
+            'memory_limit': self._settings['memory_limit'],
+            'time_limit': self._settings['time_limit'],
+            'points': 0
+        }
+        if self._settings['tests'] is not None:
+            for i in self._settings['tests'].values():
+                self._tests.append(TestF(path, i, self._test_settings))
+        self._add_test_from_dir()
+
+    def move_test_file(self, to_set, filename):
+        """
+        It moves a file from one directory to another
+
+        :param to_set: the set you want to move the file to
+        :param filename: the name of the file to move
+        """
+        if isPath(to_set._path):
+            if isPath(self._path / filename):
+                replace(self._path / filename, to_set._path / filename)
+
+    def _add_test_from_dir(self):
+        """
+        It takes a directory, finds all the files in it, and then adds all the tests that have both an input and output file
+        """
+        test_files_ext = listdir(self._path)
+        tests = []
+        for i in test_files_ext:
+            tests.append(match('.*[^.in|out]', i).group(0))
+        tests_to_do = []
+        for i in tests:
+            if tests.count(i) == 2:
+                tests_to_do.append(i)
+        tests_to_do = set(tests_to_do)
+        names = [i["name"] for i in self._tests]
+        for i in tests_to_do:
+            if i not in names:
+                name_dict = {'name': i}
+                self._tests.append(TestF(self._path, name_dict, self._test_settings))
+
+    def tests(self, test_name: str, add_new: bool = False) -> 'TestF':
+        """
+        It returns a test object with the given name, if it exists, or creates a new one if it doesn't
+
+        :param test_name: The name of the test
+        :type test_name: str
+        :param add_new: if True, then if the test is not found, it will be created, defaults to False
+        :type add_new: bool (optional)
+
+        :return: A TestF object
+        """
+        for i in self._tests:
+            if i['name'] == test_name:
+                return i
+        if add_new:
+            new_test = TestF(self._path, {'name': test_name}, self._test_settings)
+            self._tests.append(new_test)
+            self.add_empty_file(test_name + '.in')
+            self.add_empty_file(test_name + '.out')
+            return new_test
+        raise NoTestFound(f'Any test named {test_name} has found')
+
+    def remove_file(self, filename):
+        """
+        It removes a file from the current directory
+
+        :param filename: The name of the file to remove
+        """
+        if isPath(self._path / filename):
+            remove(self._path / filename)
+
+    def _delete_chosen_test(self, test: 'TestF'):
+        """
+        It removes the test from the list of tests, deletes the files associated with the test,
+        and removes the test from the config file
+
+        :param test: the test to be deleted
+        :type test: 'TestF'
+        """
+        self._tests.remove(test)
+        self.remove_file(test['name'] + '.in')
+        self.remove_file(test['name'] + '.out')
+
+        # removes settings for this test (from _settings and from config file)
+        new_settings = deepcopy(self._settings)
+        for k, v in self._settings['tests'].items():
+            if v['name'] == test['name']:
+                new_settings['tests'].pop(k)
+        self._settings = new_settings
+        self.save_to_config(self._settings)
+
+    def delete_test(self, test_name: str):
+        """
+        It deletes a test from the list of tests, and deletes associated files.
+
+        :param test_name: The name of the test to delete
+        :type test_name: str
+        :raise NoTestsFound: If there is no test with name equal to the test_name argument.
+        """
+        for test in self._tests:
+            if test['name'] == test_name:
+                self._delete_chosen_test(test)
+                return
+
+        raise NoTestFound(f'No test named {test_name} has found to delete')
+
+    def _move_chosen_test(self, test: 'TestF', to_set: 'TSet'):
+        """
+         Move a test from one test set to another
+
+        :param test: 'TestF' - the test to be moved
+        :type test: 'TestF'
+        :param to_set: the set to which the test will be moved
+        :type to_set: 'TSet'
+        """
+        name_list_ta = [j['name'] for j in to_set._tests]
+        if test['name'] not in name_list_ta:
+            to_set._tests.append(test)
+            self._tests.remove(test)
+        else:
+            raise TestExistError(f'Test named {test["name"]} exist in to_set files')
+
+        self.move_test_file(to_set, test['name'] + '.in')
+        self.move_test_file(to_set, test['name'] + '.out')
+
+    def _move_config(self, to_set: 'TSet', test_name: str):
+        """
+        It takes a test name and a set object, and moves the test from the current set to the set object
+
+        :param to_set: The set to move the test to
+        :type to_set: 'TSet'
+        :param test_name: The name of the test you want to move
+        :type test_name: str
+        """
+        new_settings = deepcopy(self._settings)
+        for i, j in self._settings['tests'].items():
+            if j['name'] == test_name:
+                to_set._settings['tests'][i] = j
+                new_settings['tests'].pop(i)
+
+        self._settings = new_settings
+        self.remove_file('config.yml')
+        self.save_to_config(self._settings)
+        to_set.remove_file('config.yml')
+        to_set.save_to_config(to_set._settings)
+
+    # moves test to to_set (and all settings pinned to this test in self._settings)
+    def move_test(self, test_name: str, to_set: 'TSet'):
+        """
+        It moves a test from one set to another
+
+        :param test_name: The name of the test to move
+        :type test_name: str
+        :param to_set: The set to which the test will be moved
+        :type to_set: 'TSet'
+        """
+        search = False
+        for i in self._tests:
+            if i['name'] == test_name:
+                self._move_chosen_test(i,  to_set)
+                self._move_config(to_set, test_name)
+                search |= True
+                return
+            search |= False
+
+        if not search:
+            raise NoTestFound(f'Any test named {test_name} has found to move to to_set')
+
+    # check set validation
+    def check_set(self, subtree=True) -> bool | int:
+        """
+        It checks the set.
+
+        :param subtree: If True, check the subtree of tests, defaults to True (optional)
+
+        :return: The result of the check_validation() method and the result of the check_set() method.
+        """
+        result = True
+        if subtree:
+            for i in self._tests:
+                result &= i.check_test()
+
+        return self.check_validation(TSet.SETTINGS_VALIDATION) & result
+
+
+class TestF(PackageManager):
+    """
+    It's a class that represents test in a set.
+    """
+    SETTINGS_VALIDATION = {
+        'name': [[isStr]],
+        'memory_limit': [[isNone], [isSize, Package.MAX_SUBMIT_MEMORY]],
+        'time_limit': [[isNone], [isIntBetween, 0, Package.MAX_SUBMIT_TIME],
+                       [isFloatBetween, 0, Package.MAX_SUBMIT_TIME]],
+        'points': [[isInt], [isFloat]]
+    }
+    """
+       Validation for ``TestF`` settings.
+
+       Available options are:
+        * ``name``: test name
+        * ``points``: maximum amount of points to earn in test
+        * ``memory_limit``: is a memory limit for test
+        * ``time_limit``: is a time limit for test
+       """
+
+    def __init__(self, path: Path, additional_settings: dict or Path, default_settings: dict):
+        """
+        This function initializes the class by calling the superclass's __init__ function, which is the __init__ function of
+        the Config class
+
+        :param path: The path to the file that contains the settings
+        :type path: Path
+        :param additional_settings: This is a dictionary of settings that you want to override the default settings with
+        :type additional_settings: dict or Path
+        :param default_settings: This is a dictionary of default settings that will be used if the settings file doesn't
+        contain a value for a setting
+        :type default_settings: dict
+        """
+        super().__init__(path, additional_settings, default_settings)
+
+    def _rename_files(self, old_name, new_name):
+        """
+        It renames a file
+
+        :param old_name: The name of the file you want to rename
+        :param new_name: The new name of the file
+        """
+        rename(self._path / old_name, self._path / new_name)
+
+    def __setitem__(self, arg: str, val):
+        """
+        It renames the files and changes the name in the yaml file
+
+        :param arg: the key of the dictionary
+        :type arg: str
+        :param val: the new value
+        """
+        # effect changes to yaml settings
+        settings = self.read_from_config()
+        if arg == 'name':
+            self._rename_files(self._settings['name'] + '.in', val + '.in')
+            self._rename_files(self._settings['name'] + '.out', val + '.out')
+
+            for i, j in settings['tests'].items():
+                if j['name'] == self._settings['name']:
+                    new_key = 'test' + val
+                    j[arg] = val
+                    settings['tests'][new_key] = j
+                    del settings['tests'][i]
+                    break
+
+        self.save_to_config(settings)
+        self._settings[arg] = val
+
+    def check_test(self) -> bool:
+        """
+        It checks if the test is valid
+        :return: The return value is the result of the check_validation method.
+        """
+        return self.check_validation(TestF.SETTINGS_VALIDATION)
```

### Comparing `baca2-package-manager-0.2.2/baca2PackageManager/validators.py` & `baca2-package-manager-0.2.3/baca2PackageManager/validators.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,251 +1,251 @@
-from pathlib import Path
-from re import findall, split
-
-
-def isAny(val):
-    """
-    any non-empty value is allowed
-
-    :return: A boolean value.
-    """
-    return bool(val)
-
-
-def isNone(val):
-    """
-    check if val is None
-
-    :return: A boolean value.
-    """
-    return val is None
-
-
-def isInt(val):
-    """
-    check if val can be converted to int
-
-    :return: A boolean value.
-    """
-    if type(val) == float:
-        return False
-    try:
-        int(val)
-        return True
-    except ValueError:
-        return False
-
-
-def isIntBetween(val, a: int, b: int):
-    """
-    check if val is an int value between a and b
-
-    :return: A boolean value.
-    """
-    if isInt(val):
-        if a <= val < b:
-            return True
-    return False
-
-
-def isFloat(val):
-    """
-    check if val can be converted to float
-
-    :return: A boolean value.
-    """
-    try:
-        float(val)
-        return True
-    except ValueError:
-        return False
-
-
-def isFloatBetween(val, a: int, b: int):
-    """
-    check if val is a float value between a and b
-
-    :return: A boolean value.
-    """
-    if isFloat(val):
-        if a <= val < b:
-            return True
-    return False
-
-
-def isStr(val):
-    """
-    check if val can be converted to string
-
-    :return: A boolean value.
-    """
-    if type(val) == str:
-        return True
-    return False
-
-
-def is_(val, schema: str):
-    """
-    check if val is exactly like schema
-
-    :return: A boolean value.
-    """
-    if isStr(val):
-        return val == schema
-    return False
-
-
-def isIn(val, *args):
-    """
-    check if val is in args
-
-    :return: A boolean value.
-    """
-    return val in args
-
-
-def isBool(val):
-    """
-    check if val is bool
-
-    :return: A boolean value.
-    """
-    return type(val) == bool
-
-
-def isShorter(val, l: int):
-    """
-    check if val is string and has len < len(l)
-
-    :return: A boolean value.
-    """
-    if isStr(val):
-        return len(val) < l
-    return False
-
-
-def isDict(val):
-    """
-    check if val has dict type
-
-    :return: A boolean value.
-    """
-    return type(val) == dict
-
-
-def isPath(val):
-    """
-    check if val is path in package_dir
-
-    :return: A boolean value.
-    """
-    if val is None:
-        return False
-    try:
-        val = Path(val)
-        if val.exists():
-            return True
-        return False
-    except ValueError:
-        return False
-
-
-def resolve_validator(func_list, arg):
-    """
-    takes the validator function with arguments, and check that if validator function is true for arg (other arguments for func)
-    """
-    func_name = str(func_list[0])
-    func_arguments_ext = ',' + ','.join(func_list[1:])
-    return eval(func_name + '("' + str(arg) + '"' + func_arguments_ext + ')')
-
-
-def hasStructure(val, struct: str):
-    """
-    check if val has structure provided by struct and fulfills validators functions from struct
-
-    :return: A boolean value.
-    """
-    validators = findall("<.*?>", struct)
-    validators = [i[1:-1].split(',') for i in validators]
-    constant_words = findall("[^<>]{0,}<", struct) + findall("[^>]{0,}$", struct)
-    constant_words = [i.strip("<") for i in constant_words]
-    if len(validators) == 1:
-        values_to_check = [val]
-    else:
-        # words_in_pattern = [i for i in constant_words if i != '|' and i != '']
-        # regex_pattern = '|'.join([i for i in constant_words if i != '|' and i != ''])
-        values_to_check = split('|'.join([i for i in constant_words if i != '|' and i != '']), val)
-    if struct.startswith('<') == False:
-        values_to_check = values_to_check[1:]
-    valid_idx = 0
-    const_w_idx = 0
-    values_idx = 0
-    temp_alternative = False
-    result = True
-    while valid_idx < len(validators) and values_idx < len(values_to_check):
-        temp_alternative |= resolve_validator(validators[valid_idx], values_to_check[values_idx])
-        if constant_words[const_w_idx] == '|':
-            if constant_words[const_w_idx + 1] != '|':
-                values_idx += 1
-        else:
-            if constant_words[const_w_idx + 1] != '|':
-                values_idx += 1
-                result &= temp_alternative
-                temp_alternative = False
-        valid_idx += 1
-        const_w_idx += 1
-    return result
-
-
-def memory_converting(val: str):
-    """
-     function is converting memory from others units to bytes
-
-     :return: Memory converted to bytes. (In INT type)
-    """
-    if val[-1] == 'B':
-        return int(val[0:-1])
-    elif val[-1] == 'K':
-        return int(val[0:-1]) * 1024
-    elif val[-1] == 'M':
-        return int(val[0:-1]) * 1024 * 1024
-    elif val[-1] == 'G':
-        return int(val[0:-1]) * 1024 * 1024 * 1024
-
-
-def valid_memory_size(first: str, second: str):
-    """
-    checks if first is smaller than second considering memory
-
-    :return: A boolean value.
-    """
-    if memory_converting(first) <= memory_converting(second):
-        return True
-    return False
-
-
-def isSize(val: str, max_size: str):
-    """
-    check if val has structure like <isInt><isIn, 'B', 'K', 'M', 'G'>
-
-    :return: A boolean value.
-    """
-    val = val.strip()
-    return hasStructure(val[:-2], "<isInt>") and hasStructure(val[-1],
-                                                              "<isIn, 'B', 'K', 'M', 'G'>") and valid_memory_size(val,
-                                                                                                                  max_size)
-
-
-def isList(val, *args):
-    """
-    check if val is a list and every element from list fulfill at least one validator from args
-
-    :return: A boolean value.
-    """
-    if type(val) == list:
-        result = False
-        for i in val:
-            for j in args:
-                result |= hasStructure(i, j)
-            if not result:
-                return result
-    return True
+from pathlib import Path
+from re import findall, split
+
+
+def isAny(val):
+    """
+    any non-empty value is allowed
+
+    :return: A boolean value.
+    """
+    return bool(val)
+
+
+def isNone(val):
+    """
+    check if val is None
+
+    :return: A boolean value.
+    """
+    return val is None
+
+
+def isInt(val):
+    """
+    check if val can be converted to int
+
+    :return: A boolean value.
+    """
+    if type(val) == float:
+        return False
+    try:
+        int(val)
+        return True
+    except ValueError:
+        return False
+
+
+def isIntBetween(val, a: int, b: int):
+    """
+    check if val is an int value between a and b
+
+    :return: A boolean value.
+    """
+    if isInt(val):
+        if a <= val < b:
+            return True
+    return False
+
+
+def isFloat(val):
+    """
+    check if val can be converted to float
+
+    :return: A boolean value.
+    """
+    try:
+        float(val)
+        return True
+    except ValueError:
+        return False
+
+
+def isFloatBetween(val, a: int, b: int):
+    """
+    check if val is a float value between a and b
+
+    :return: A boolean value.
+    """
+    if isFloat(val):
+        if a <= val < b:
+            return True
+    return False
+
+
+def isStr(val):
+    """
+    check if val can be converted to string
+
+    :return: A boolean value.
+    """
+    if type(val) == str:
+        return True
+    return False
+
+
+def is_(val, schema: str):
+    """
+    check if val is exactly like schema
+
+    :return: A boolean value.
+    """
+    if isStr(val):
+        return val == schema
+    return False
+
+
+def isIn(val, *args):
+    """
+    check if val is in args
+
+    :return: A boolean value.
+    """
+    return val in args
+
+
+def isBool(val):
+    """
+    check if val is bool
+
+    :return: A boolean value.
+    """
+    return type(val) == bool
+
+
+def isShorter(val, l: int):
+    """
+    check if val is string and has len < len(l)
+
+    :return: A boolean value.
+    """
+    if isStr(val):
+        return len(val) < l
+    return False
+
+
+def isDict(val):
+    """
+    check if val has dict type
+
+    :return: A boolean value.
+    """
+    return type(val) == dict
+
+
+def isPath(val):
+    """
+    check if val is path in package_dir
+
+    :return: A boolean value.
+    """
+    if val is None:
+        return False
+    try:
+        val = Path(val)
+        if val.exists():
+            return True
+        return False
+    except ValueError:
+        return False
+
+
+def resolve_validator(func_list, arg):
+    """
+    takes the validator function with arguments, and check that if validator function is true for arg (other arguments for func)
+    """
+    func_name = str(func_list[0])
+    func_arguments_ext = ',' + ','.join(func_list[1:])
+    return eval(func_name + '("' + str(arg) + '"' + func_arguments_ext + ')')
+
+
+def hasStructure(val, struct: str):
+    """
+    check if val has structure provided by struct and fulfills validators functions from struct
+
+    :return: A boolean value.
+    """
+    validators = findall("<.*?>", struct)
+    validators = [i[1:-1].split(',') for i in validators]
+    constant_words = findall("[^<>]{0,}<", struct) + findall("[^>]{0,}$", struct)
+    constant_words = [i.strip("<") for i in constant_words]
+    if len(validators) == 1:
+        values_to_check = [val]
+    else:
+        # words_in_pattern = [i for i in constant_words if i != '|' and i != '']
+        # regex_pattern = '|'.join([i for i in constant_words if i != '|' and i != ''])
+        values_to_check = split('|'.join([i for i in constant_words if i != '|' and i != '']), val)
+    if struct.startswith('<') == False:
+        values_to_check = values_to_check[1:]
+    valid_idx = 0
+    const_w_idx = 0
+    values_idx = 0
+    temp_alternative = False
+    result = True
+    while valid_idx < len(validators) and values_idx < len(values_to_check):
+        temp_alternative |= resolve_validator(validators[valid_idx], values_to_check[values_idx])
+        if constant_words[const_w_idx] == '|':
+            if constant_words[const_w_idx + 1] != '|':
+                values_idx += 1
+        else:
+            if constant_words[const_w_idx + 1] != '|':
+                values_idx += 1
+                result &= temp_alternative
+                temp_alternative = False
+        valid_idx += 1
+        const_w_idx += 1
+    return result
+
+
+def memory_converting(val: str):
+    """
+     function is converting memory from others units to bytes
+
+     :return: Memory converted to bytes. (In INT type)
+    """
+    if val[-1] == 'B':
+        return int(val[0:-1])
+    elif val[-1] == 'K':
+        return int(val[0:-1]) * 1024
+    elif val[-1] == 'M':
+        return int(val[0:-1]) * 1024 * 1024
+    elif val[-1] == 'G':
+        return int(val[0:-1]) * 1024 * 1024 * 1024
+
+
+def valid_memory_size(first: str, second: str):
+    """
+    checks if first is smaller than second considering memory
+
+    :return: A boolean value.
+    """
+    if memory_converting(first) <= memory_converting(second):
+        return True
+    return False
+
+
+def isSize(val: str, max_size: str):
+    """
+    check if val has structure like <isInt><isIn, 'B', 'K', 'M', 'G'>
+
+    :return: A boolean value.
+    """
+    val = val.strip()
+    return hasStructure(val[:-2], "<isInt>") and hasStructure(val[-1],
+                                                              "<isIn, 'B', 'K', 'M', 'G'>") and valid_memory_size(val,
+                                                                                                                  max_size)
+
+
+def isList(val, *args):
+    """
+    check if val is a list and every element from list fulfill at least one validator from args
+
+    :return: A boolean value.
+    """
+    if type(val) == list:
+        result = False
+        for i in val:
+            for j in args:
+                result |= hasStructure(i, j)
+            if not result:
+                return result
+    return True
```

### Comparing `baca2-package-manager-0.2.2/baca2_package_manager.egg-info/PKG-INFO` & `baca2-package-manager-0.2.3/baca2_package_manager.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1
-Name: baca2-package-manager
-Version: 0.2.2
-Summary: A package manager for Baca2 project
-Home-page: https://github.com/BaCa2-project/BaCa2-package-manager
-Author: Baca2 Team
-Author-email: bartosz.deptula@student.uj.edu.pl
-Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# BaCa2-package-manager
-_Package manager for BaCa2 (to be exported as PyPI package)._
-
-Package manager designed to automatically interpret and work with task packages for BaCa2 checker.
-It is needed for every kind of broker, and BaCa2 itself.
+Metadata-Version: 2.1
+Name: baca2-package-manager
+Version: 0.2.3
+Summary: A package manager for Baca2 project
+Home-page: https://github.com/BaCa2-project/BaCa2-package-manager
+Author: Baca2 Team
+Author-email: bartosz.deptula@student.uj.edu.pl
+Classifier: Programming Language :: Python :: 3
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# BaCa2-package-manager
+_Package manager for BaCa2 (to be exported as PyPI package)._
+
+Package manager designed to automatically interpret and work with task packages for BaCa2 checker.
+It is needed for every kind of broker, and BaCa2 itself.
```

### Comparing `baca2-package-manager-0.2.2/setup.py` & `baca2-package-manager-0.2.3/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-import setuptools
-
-setuptools.setup(
-    name='baca2-package-manager',
-    version='0.2.2',
-    author='Baca2 Team',
-    author_email='bartosz.deptula@student.uj.edu.pl',
-    description='A package manager for Baca2 project',
-    long_description=open('README.md').read(),
-    long_description_content_type='text/markdown',
-    url='https://github.com/BaCa2-project/BaCa2-package-manager',
-    packages=setuptools.find_packages(),
-    classifiers=[
-        'Programming Language :: Python :: 3',
-        'Development Status :: 4 - Beta',
-        'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
-    ],
-    python_requires='>=3.10',
-    install_requires=[
-        'pyyaml',
-    ]
-)
+import setuptools
+
+setuptools.setup(
+    name='baca2-package-manager',
+    version='0.2.3',
+    author='Baca2 Team',
+    author_email='bartosz.deptula@student.uj.edu.pl',
+    description='A package manager for Baca2 project',
+    long_description=open('README.md').read(),
+    long_description_content_type='text/markdown',
+    url='https://github.com/BaCa2-project/BaCa2-package-manager',
+    packages=setuptools.find_packages(),
+    classifiers=[
+        'Programming Language :: Python :: 3',
+        'Development Status :: 4 - Beta',
+        'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
+    ],
+    python_requires='>=3.10',
+    install_requires=[
+        'pyyaml',
+    ]
+)
```

