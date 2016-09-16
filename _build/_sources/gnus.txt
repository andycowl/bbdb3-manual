====
Gnus
====

Although using BBDB interactively illustrates key features, the real
power of BBDB is when used in conjunction with a mail or news reader.

BBDB calls any such mail/news reader a Mail User Agent (MUA) and
offers similar functionality for all supported MUA's.

This MUA abstraction makes it relatively easy to add support for new
mail readers.

BBDB also supports 'message-mode' which is commonly used by mail
programs to send outbound email messages. Again, as BBDB integrates
with 'message-node', it automatically works with any Emacs mail
program that supports 'message-mode'.

The real power is the ability to automatically add entries to BBDB
when reading email or news.

--------------------------------
What version of Gnus do I need ?
--------------------------------

BBDB works with any version of Gnus bundled with Emacs 23 (and later).

-------------------------
Automatically add entries
-------------------------

To ensure Gnus and message mode both use BBDB, add these lines to
'init.el'::

  (bbdb-initialize 'gnus 'message)
  (bbdb-mua-auto-update-init 'gnus 'message)
  ;
  ; Display BBDB in popup window
  (setq bbdb-mua-pop-up t)
  ;
  ; Look for existing contact, interactively prompt to create
  (setq bbdb-mua-update-interactive-p '(query . create))

This configuration integrates Gnus into BBDB. No contacts will be
added to BBDB unless the user explicitly requests this action.

For an *interesting* contact, simply type ';' in the Gnus summary buffer
which invokes 'bbdb-mua-edit-field-sender'.

BBDB offers the following options::

  Michael Stipe is not in BBDB; add (y ! n s q ?)
  Type ? for this help
  Type 'y to add the current record
  Type ! to add all the remaining records
  Type n to skip the current record (You may also use space)
  Type s to switch from annotate to search mode
  Type q to quit updating records. No more search or annotation is done.

Type 'y' to add the contact and annotate as required. For example, a
personal contact might be tagged with 'Family' in the 'Notes' field.

When composing or replying to a message, you can use 'TAB'
('message-tab') to complete names from BBDB.

To enable fully automatic and insidious mode, use::

  ; Silently add record to BBDB (if not already present)
  (setq bbdb-update-records-p 'create)
  ; Update BBDB silently
  (setq bbdb-mua-pop-up nil)

-------------------------
Whitelists and blacklists
-------------------------

[ Check this and test ]

There are some scenarios where it is not useful for BBDB to mindlessly
collect contact information. One example is the Gmane mailing lists
where the true email addresses of posters are masked::

  (setq bbdb/mail-auto-create-p 'bbdb-ignore-some-messages-hook)
  (setq bbdb/news-auto-create-p 'bbdb-ignore-some-messages-hook)
  (setq bbdb-ignore-some-messages-alist
    `(("From" . "public.gmane.org")
     ("Newsgroups" . "gmane.*")
     ))

-------------
Use full name
-------------

[ Check this example too ]

Some people (or their IT administrators) have malformed names in their
email configuration. If you prefer to see names correctly capitalized
as 'Mike Mills' rather than 'mike mills' or, worse, 'MIKE MILLS', you
can ask Gnus to display the name stored in BBDB in preference to the name
supplied in the mail or article header information::

  ; display names as in BBDB database
  (autoload 'bbdb/gnus-lines-and-from "bbdb-gnus")

-----------------
Gnus Summary Line
-----------------

To get Gnus to display the BBDB name together with a indication (the
'+' character) that the sender is known to BBDB, use::

  ; Default with %f ('Name, To header or Newsgroups header')
  ; replaced by %uB (BBDB Name + Known poster indicator '+')
  ;
  ; Original Gnus setting
  ;
  ; ‘%U%R%z%I%(%[%4L: %-23,23f%]%) %s\n’.
  (setq gnus-summary-line-format "%U%R%z%I%(%[%4L: %-23,23uB%]%) %s\n")
