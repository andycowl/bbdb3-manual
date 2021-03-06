============
Introduction
============

The Big Brother Database (BBDB) is a contact management system for
GNU Emacs version 23 or later.

BBDB offers the following features:

* integration with Emacs news and mail readers (Gnus, MH-e, mu4e,
  notmuch, Rmail, Wanderlust, VM).
* automatic creation of entries from mail messages and news articles.
* extensible database format with standard and user-defined fields.
* support for different address and phone formats.
* integration of events with Emacs calendar and Orgmode.
* printing of address book entries using TeX.
* database management (de-duplication, purging historic data).
* support for signed and encrypted messages using PGP.

-------
History
-------

Jamie Zawinski implemented the original BBDB package in 1992 and the
package was subsequently maintained bu Waider and later by Robert
Widhopf-Fenk.

The last release of BBDB2 was version 2.35 (released on 30 January 2007).

In May 2010, Roland Winkler announced he was resurrecting the project
and embarking on a major rewrite.

--------------------
Where to get BBDB3 ?
--------------------

The latest stable release of BBDB is currently 3.1.2 (released on 27
April 2014) and available for download from:

http://download.savannah.gnu.org/releases/bbdb/

The source of the latest development version is available at:

http://savannah.nongnu.org/projects/bbdb/

BBDB3 is also available via `Melpa`_. This version tracks the latest
development version.

.. _Melpa: https://melpa.org/#/

--------
Building
--------

There are a couple of prerequisites for compiling BBDB3 from source:

* autoconf (2.69 or higher)
* automake (1.13 or higher)

Most Linux distributions will have the required versions of these
packages available in the standard repositories.

A quickstart guide for building the latest version of BBDB3 from
source on Linux

.. code-block:: sh

   $ git clone git://git.savannah.nongnu.org/bbdb.git
   $ sh ./autogen
   $ ./configure
   $ make
   $ sudo make install

-------------
Configuration
-------------

To get started with BBDB, two lines are required in ``init.el``

.. code-block:: emacs-lisp

   (add-to-list 'load-path "/path/to/bbdb/lisp")
   (require 'bbdb-loaddefs)

---------
Upgrading
---------

BBDB3 will automatically detect a BBDB2 database and convert the
contents to the new format. This conversion is done automatically
although it may be prudent to take a copy of the existing BBDB
database.

The default location for the BBDB database was ``~/.bbdb`` in BBDB2
and changed to ``~/.emacs.d/bbdb`` in BBDB3.
