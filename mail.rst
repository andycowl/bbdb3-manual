====
Mail
====

Apparently there are other mail readers for Emacs besides Gnus. Most
of these mail handling programs are supported by BBDB.

As mailing handling is abstracted to a generic Mail user Agent (MUA),
adding support for a new Emacs mail reader program should be
relatively straightforward.

To use BBDB in conjunction with any of the following mail programs,
simply add the appropriate program to :function:`bbdb-initialize` in
``init.el``. If you are using message-mode, include 'message as well.

For example

.. code-block:: emacs-lisp

   (bbdb-initialize 'mu4e 'message)

For other mail programs, substitute 'mu4e as follows:

* mail - Mail
* mh-e - MH-E
* notmuch - notmuch
* rmail - Rmail
* vm - ViewMail
* wl - Wanderlust

----
MH-E
----

https://www.gnu.org/software/emacs/manual/html_mono/mh-e.html

----
mu4e
----

http://www.djcbsoftware.nl/code/mu/mu4e.html

-------
notmuch
-------

https://notmuchmail.org/

-----
rmail
-----

https://www.gnu.org/software/emacs/manual/html_node/emacs/Rmail.html

--
VM
--

http://www.nongnu.org/viewmail/

----------
Wanderlust
----------

https://www.emacswiki.org/emacs/WanderLust
