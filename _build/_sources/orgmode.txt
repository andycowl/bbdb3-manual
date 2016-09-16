========
Org Mode
========

------
Agenda
------

The variable 'org-bbdb-anniversary-field' (default 'anniversary') can
be modified to show birthdays in orgmode.

Ensure the following lines are contained in 'org-default-agenda-files'::

  *Anniversaries
  +CATEGORY: Anniv
  %%(org-bbdb-anniversaries)
