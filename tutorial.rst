========
Tutorial
========

This is a gentle, step-by-step tutorial, aimed at newcomers to BBDB,
which includes worked examples showing how to use the software.

The best way to demonstrate the features in BBDB is to actually
illustrate some standard tasks. If you are already an experienced BBDB
user, you may wish to skip this section.

Creating an entry
-----------------

The first task to to add a contact to our BBDB::

  M-x bbdb-create

Enter 'Ivan McCormick' as the name.

Leave the fields 'Organizations', 'E-Mail Addresses', 'Snail Mail
Address Label', 'Phone Label' and 'notes' fields blank (simply by
typing 'Enter').

Add another entry for 'David Evans' in the same manner.

Now we have two entries, we can navigate and search our embryonic
BBDB.

Searching
---------

To examine the contents of BBDB, use::

  M-x bbdb

Type 'return' to 'Search records using regexp' which displays all
entries.

BBDB then displays all known contacts and the modeline includes
'1/2/2' which indicates the current entry is '1' out of a current data
set of 2 from a grand total of 2.

The entries are initially sorted by 'Name' order so 'David Evans'
appears first despite being added last.

Navigation uses the familiar 'n' (`bbdb-next-record`) and 'p'
(`bbdb-prev-record`) key bindings.

You can also search BBDB using 'b' (`bbdb`) which searches across all
fields. For example, searching for 'evans' displays a single record
('David Evans'). The search is case insensitive.

Updating
--------

Occasionally, you may want to change contact details.  Search BBDB
(using 'b') to find the contact named 'David Evans'.

Type 'e' (`bbdb-edit-field`) to change this contact's first name to
'Dave'.

Save your changes using 's' (`bbdb-save`). Your changes are now saved
to the BBDB which resides in '~/.emacs.d/bbdb' (`bbdb-file`) by
default.

Adding fields
-------------

Add a new contact called 'Adam Clayton' using 'c' (`bbdb-create`). This
time, include additional information for the organization, address,
phone number and email address as follows::

  For 'Organizations' enter, 'Island Records'
  For email, enter 'adam.clayton@island.com'
  Street, line 1 - '721 Fifth Avenue'
  Street, line 2 - 'Midtown Center'
  Street, line 2 - 'Manhattan'
  City - 'New York City'
  State - 'NY'
  Postcode - 10022
  Country - 'US'
  For 'Phone (home), enter '0012127654321'
  For the 'notes' field, enter 'U2'

Now we have a record populated with five fields in addition to
'Name'. The newly created record is displayed.

You can use 't' (`toggle-layout`) to view a brief one line summary and
'T' (`show-all-fields`) to expose all fields of the contact. The
expanded view includes two standard audit timestamp fields that are
automatically created and maintained by BBDB; 'creation-date' and
'timestamp'

For a newly created record, both timestamp fields will be identical
but the 'timestamp' field will automatically track whenever a
subsequent update is made to the record. The timestamps can be
valuable in purging historic, outdated data and examining recent
records.

Use 'TAB' (`bbdb-next-field`) to navigate to the next field and
'BACKSPACE' (`bbdb-prev-field`) to go back to the previous field.

If you made any errors during the creation of the contact, you can
navigate to the field and then use 'e' (`bbdb-edit-field`) to edit and
correct the field.

Searching on fields
-------------------

In addition to the general search ('b') which searches across all
fields, you can also search for contacts on individual fields (which
is quicker and more efficient for larger databases).

For example, to search for all contacts with an email address
containing 'island.com', use '/ m' and enter 'island'.

The full list of field searches is

+-------------+---------------+
| Key binding | Field         |
+=============+===============+
| 'b'         | General       |
+-------------+---------------+
| '/ 1'       | Single record |
+-------------+---------------+
| '/ m'       | Email         |
+-------------+---------------+
| '/ n'       | Name          |
+-------------+---------------+
| '/ o'       | Organization  |
+-------------+---------------+
| '/ p'       | Phone         |
+-------------+---------------+
| '/ a'       | Address       |
+-------------+---------------+
| '/ x'       | Xfields       |
+-------------+---------------+
| '/ m'       | Email         |
+-------------+---------------+
| '/ d'       | Duplicates    |
+-------------+---------------+
| '/ c'       | Changed       |
+-------------+---------------+
| '+'         | Append        |
+-------------+---------------+
| '!'         | Invert        |
+-------------+---------------+

Duplicates
----------

BBDB offers help in managing a contact database. A common problem is
that of duplicate entries; a person who has different aliases ('Dave',
'David') or multiple email addresses (e.g. home, work) or historic,
outdated fields.

Add a new entry for 'Larry Mullen' with an email address of
'larry.mullen@islandrecords.com'.

Add another entry for 'Larry Mullen Jnr' with the same email address
of 'larry.mullen@islandrecords.com'.

Display all entries using 'b' and use '/ d' (`bbdb-search-duplicates`)
to search for duplicate entries.

The two similar entries for 'Larry Mullen' should be displayed.

To merge these two entries, use M-x bbdb-merge-records. BBDB will use
the currently displayed record ('Larry Mullen Jnr') as the first entry
and prompt for the second record::

  merge record "Larry Mullen Jnr" into:

Type 'Larry Mullen' to identify the second record. BBDB will ask::

  Use name "Larry Mullen Jnr" instead of "Larry Mullen"? (y or n)

followed by::

  Keep "Larry Mullen" as an alternate name? (y or n)

The single, resulting merged record is now displayed. 'Larry Mullen'
is now is an 'AKA' field for the 'Larry Mullen Jnr' record.

Extended Fields
---------------

BBDB supports extended fields ('xfields') which allow the user to
define additional fields for contacts. The predefined 'notes' field in
BBDB2 is simply an example of an extended field in BBDB3.

You can add a note field to an existing contact using ';'
(`edit-some-field`).

As no contacts were initially created with a 'note' field, BBDB
prompts::

  "notes" is an unknown field name. Define it? (y or n)

In addition to the 'notes' field, you can extend BBDB with additional
user defined fields.

Use 'i' (`bbdb-insert-field`) to add a new field called 'Instrument'
and set this field to 'Guitar' for Dave Evans.

Of course, the U2 guitarist is more commonly known as 'The Edge' so
navigate to the AKA ('Also Known As') field and add 'The Edge' as an
alias for 'David Evans'.

Sending email
-------------

BBDB allows sending email to a single contact or a set of contacts.

Search and navigate to a specfic contact and type 'm' (`bbdb-mail`)
which composes an email to the current contact.

If a set of contacts has been created, type '* m' to send an email to
all contacts in the list.

You can use this feature to manage simple mail groups; if you tag a
group of contacts with 'curry', you can use '* m' to invite your
friends for the traditional Thursday night meal.

Omitting an entry
-----------------

If you have selected a list of contacts, it is possible to omit a
contact (or multiple contacts) from the list of recipients while
preserving the entry in BBDB.

You use 'o' (`omit-record`) which hides the entry and type '* m' to
compose an email to the reduced list of contacts.

Deleting a field
----------------

You can delete the contents of a field by navigating to the field of
the contact (use 'n' and 'p' to navigate between contacts and 'TAB'
and 'DEL' between fields). Once positioned on the correct field, use
'd' or 'C-k' (which are both bound to `bbdb-delete-field-or-record`).

BBDB will prompt::

  delete this 'mail' field (of Michael Stipe)? (y or n).

-----------------
Deleting an entry
-----------------

Deleting an entry in BBDB is similar. Navigate to the desired entry
and use 'd' or C-k.

BBDB will prompt::

  Delete the entry of Stephen Morrissey ? (y or n)

Deletions of multiple records is possible in the normal way; selecting
the desired data set and use C-k. A prompt will be issued for each
record.

---------------------------
Birthdays and anniversaries
---------------------------

To use birthday and anniversaries in BBDB, you must ensure 'anniv is
included in the list of parameters when calling `bbdb-initialize` in
'init.el'::

  (bbdb-initialize 'gnus 'message 'anniv)

To ensure BBDB birthdays and anniversaries are displayed in the Emacs
calendar, add the following line to 'init.el'::

  (add-hook 'diary-list-entries-hook 'bbdb-anniv-diary-entries)

Birthdays are implemented as another extended field named 'birthday'.

Find the contact called 'Adam Clayton' and add a new extended field
called 'birthday' using 'i' (`bbdb-insert-field`).

The default date format setting is 'American' ('mm/dd/yyyy') so, to
add Adam Clayton's birthday which is '13 March 1960', enter::

  '03/13/1960'

The default date format is controlled by the variable
'calendar-date-style' which may be set to:-

* 'american' (mm/dd/yyyy - default)
* 'european' (dd/mm/yyyy)
* 'iso'      (yyyy/mm/dd)

Check the birthday has been added to the Emacs calendar::

  M-x calendar

Navigate to 13 March and type 'd' (`diary-view-entries`). The birthday
should be displayed as follows::

  Sunday, March 13, 2016
  ======================
  Adam Clayton's 56th birthday

Housekeeping
------------

BBDB uses the built-in audit timestamps ('creation-date' and
'timestamp') to offer useful searches to identify ancient or recent
records:

* bbdb-creation-newer
* bbdb-creation-older
* bbdb-timestamp-newer
* bbdb-timestamp-older

For example, to list all records created before 2014, use
'M-x bbdb-creation-older-than'. BBDB prompts::

  'Older than date (yyyy-mm-dd):'

Enter '2014-01-01' to displayed all contacts created prior to 2014.

There is a complementary function `bbdb-creation-newer-than` to
identify recently created records.

Similarly, using the 'timestamp' field can identify records modified
in the last month (`bbdb-timestamp-newer`).

Another useful function to assist in identifying records that have
been created and never subsequently updated is
`bbdb-creation-no-change`.

Snarfing
--------

Given a text file with the following .. contents::

  Michael Stipe
  245 Dan Rather Avenue
  Atlanta
  GA
  Email: stipey@remhq.com

If you highlight the region, position point at 'Michael Stipe' and
type 'M-x bbdb-snarf', BBDB will attempt to parse the region and
create a BBDB entry for this individual.

Unfortunately, snarfing is complex and doesn't always deliver perfect
results::

  Michael Stipe
         mail:  stipey@remhq.com
         notes: 245 Dan Rather Avenue
         Atlanta
         GA

Printing
--------

`bbdb-print` produces a TeX file for the current set of contacts and
uses bbdb-print-tex-path (typically /path/to/bbdb/tex) to locate the
TeX templates.

BBDB then creates a TeX file which must be processed using TeX (not
LaTeX) to produce a PDF ready for printing.

Dialing
-------

`bbdb-dial` dials the number under point.
