---
content_type: page
description: This section provides instructions for installing the Scmutils system,
  an integrated library of procedures, embedded in the programming language Scheme,
  and intended to support teaching and research in mathematical physics and electrical
  engineering.
draft: false
learning_resource_types:
- Tools
ocw_type: CourseSection
title: Tools
uid: 221703f1-ba37-98ab-abda-f82c0d8278c2
---
## Scheme Mechanics Installation for GNU/Linux or Mac OS X

Installation (requires root access)

All files will be installed in the subdirectory structure /usr/local/scmutils. The mechanics system has several parts:

- One part is the Scheme system itself. We provide a Scheme system as part of this distribution. It will install itself so as to not interfere with any other Scheme you may currently have. The installation will install a script named mechanics in /usr/local/bin that invokes the Scheme system that runs the mechanics system.
- The other part is Scmutils, the numerical and algebraic packages, written in Scheme, that we will use for the mechanics work.

The installed system requires about 50 Megabytes of disk space.

Installation instructions:

1. Download the system (a TAR file, compressed with gzip) into a temporary directory of your choice. This file is about 20 megabytes long.
2. Be sure you are logged in with root privileges. If your system does not have a directory /usr/local, you will need to create one. Then execute the command lines:   
    cd /usr/local   
    tar -xvzf \[your-tarball.tar.gz\]
3. The command line to start the Scheme mechanics system is   
    /usr/local/bin/mechanics   
    (If /usr/local/bin is on your search path you need not specify the whole path.)
4. If everything seems to work you can now remove the tarball.

**Note**: We have tested this Scheme system under Debian GNU/Linux Etch, Ubuntu GNU/Linux Gutsy Gibbon, and Mac OS X 10.5. The Gutsy Gibbon version works under Ubuntu Hardy Heron. If these will not work for you, you can ask for help, but note that we know nothing about MS Windows.

Useful documents are included in the /usr/local/scmutils/manual/ subdirectory that will be unpacked with the tar file. Scheme sources for the entire system are included in the /usr/local/scmutils/src/ subdirectory.

The main interface to the system is edwin, an Emacs18 implemented in Scheme. If you are not familiar with Emacs you **should** run the tutorial, which can be accessed in edwin by holding down the control key and typing h, then, releasing the control key, type t. (C-h t)

Note that this is all free software, as defined by the GNU General Public License. Also, this is all software developed for education and research at MIT. This code is not carefully tested so it may have errors. We hope that it can help you, but we make no warranty.