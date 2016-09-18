===
FAQ
===

What version of Emacs do I need ?
---------------------------------

Version 23, 24 or 25 of GNU Emacs. XEmacs is longer supported

How do you automatically save BBDB on exit ?
--------------------------------------------

How to get help with BBDB ?
---------------------------

The best place to get help with BBDB3 is the mailing list::

  There is a mailing list for discussion of BBDB:
    bbdb-info@lists.sourceforge.net
  To join, send mail to bbdb-info-request@lists.sourceforge.net

How to report a problem with BBDB ?
-----------------------------------

Send a detailed report to the BBDB mailing list including the
following info:-

* Emacs version
* BBDB version
* BBDB/Message/Mail customizations
* What you expected to happen
* What happened

File format information
-----------------------

You don't need to know this but the BBDB file format version is
embedded within the database file::

  $ head -2 ~/.emacs.d/bbdb
  ;; -*- mode: Emacs-Lisp; coding: utf-8; -*-
  ;;; file-format: 7

Incorrect BBDB version
----------------------

If BBDB is built from source, 'M-x bbdb-version' reports the version::

  BBDB version 3.1.2 (2016-07-21 01:18:24 -0500)

However, if you are using BBDB diownloaded from Melpa, 'M-x
bbdb-version' reports::

  'BBDB version @PACKAGE_VERSION@ (@PACKAGE_DATE@)'

This is a known issue with the packaging process on Melpa.

If you need to know the correct BBDB version (e.g for a bug report),
then either cite the date of the Melpa package. Alternatively, use::

  M-x locate-library
  bbdb-site
  'Library is file /path/to/bbdb/lisp/bbdb-site.elc'
  $ grep bbdb-version /path/to/bbdb/lisp/bbdb-site.el
  (defconst bbdb-version "3.1.2" "Version of BBDB.")
  (defconst bbdb-version-date "2016-07-21 01:18:24 -0500"
