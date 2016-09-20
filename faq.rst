===
FAQ
===

What version of Emacs do I need ?
---------------------------------

Versions 23, 24 and the recently released 25.1 of GNU Emacs are
supported.

XEmacs is longer supported


How to get help with BBDB ?
---------------------------

The best place to get help with BBDB3 is the mailing list::

  There is a mailing list for discussion of BBDB:
    bbdb-info@lists.sourceforge.net
  To join, send mail to bbdb-info-request@lists.sourceforge.net

How to report a problem with BBDB ?
-----------------------------------

Send a detailed report to the BBDB mailing list including the
following information:-

* Emacs version
* BBDB version
* BBDB/Message/Mail customizations
* What you expected to happen
* What happened

File format information
-----------------------

The BBDB file format version is embedded within the file header (first
two lines) of the BBDB database file. It's unlikely you will ever need
to know this but it may prove helpful when diagnosing V2 to V3
migration issues.

For BBDBV2 (2.35)::

  ;; -*-coding: utf-8-emacs;-*-
  ;;; file-version: 6

For BBDBV3 (3.1.2)::

  ;; -*- mode: Emacs-Lisp; coding: utf-8; -*-
  ;;; file-format: 7


Incorrect BBDB version
----------------------

If BBDB is built from source, :function:`bbdb-version` reports the version::

  BBDB version 3.1.2 (2016-07-21 01:18:24 -0500)

However, if you are using the version of BBDB downloaded from Melpa,
'M-x bbdb-version' reports::

  BBDB version @PACKAGE_VERSION@ (@PACKAGE_DATE@)

This is a known issue_ with the packaging process on Melpa.

.. _issue: https://github.com/melpa/melpa/issues/1470

If you need to know the correct BBDB version (e.g. for a bug report),
then either cite the date of the Melpa package. Alternatively, use::

  M-x locate-library
  Enter 'bbdb-site'
  'Library is file /path/to/bbdb/lisp/bbdb-site.elc'
  $ grep bbdb-version /path/to/bbdb/lisp/bbdb-site.el
  (defconst bbdb-version "3.1.2" "Version of BBDB.")
  (defconst bbdb-version-date "2016-07-21 01:18:24 -0500"

Automatic save
--------------

Can I prevent BBDB constantly asking me to save the bbdb ?::

  (add-hook 'bbdb-after-change-hook (lambda (arg) (bbdb-save)))

How to record contacts on outbound emails ?
-------------------------------------------

[ Ask Roland ]

This thread implies it's possible but I don't know the magic elisp
snippet

https://www.mail-archive.com/bbdb-info@lists.sourceforge.net/msg06286.html

Terminology
-----------

BBDB3 attempted to rationalise the terminology which meant the
changing of some lisp variables and functions.

In BBDB3, "address" is used to refer to snail mail addresses, "mail"
for email addresses and "name" for real names.

BBDB3 treats outgoing messages (i.e. Emacs message and mail mode) like
incoming messages in your Emacs MUA (Gnus, Rmail, VM, etc).  So you
can configure BBDB such that it updates BBDB based on outgoing
messages in much the same way you can do this with incoming messages.
