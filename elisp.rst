===================
Elisp Documentation
===================

.. el:require:: bbdb
.. el:require:: bbdb-anniv
.. el:require:: bbdb-com
.. el:require:: bbdb-gnus
.. el:require:: bbdb-ispell
.. el:require:: bbdb-message
.. el:require:: bbdb-mhe
.. el:require:: bbdb-migrate
.. el:require:: bbdb-mu4e
.. el:require:: bbdb-mua
.. el:require:: bbdb-pgp
.. el:require:: bbdb-print
.. el:require:: bbdb-rmail
.. el:require:: bbdb-sc
.. el:require:: bbdb-site
.. el:require:: bbdb-snarf
.. el:require:: bbdb-vm
.. el:require:: bbdb-wl

Summary of BBDB commands, functions, variables and hooks.


Command Index
-------------

.. el:command:: bbdb
   :binding: b
   :auto:

.. el:command:: bbdb-add-mail-alias
   :binding: a
   :auto:

.. el:command:: bbdb-append-display
   :binding: +
   :auto:

.. el:command:: bbdb-browse-url
   :binding: u
   :auto:

.. el:command:: bbdb-copy-fields-as-kill
   :binding: C r
   :auto:

.. el:command:: bbdb-copy-records-as-kill
   :binding: C r
   :auto:

.. el:command:: bbdb-create
   :binding: c
   :auto:

.. el:command:: bbdb-delete-field-or-record
   :binding: C-k or d
   :auto:

.. el:command:: bbdb-dial
   :binding: M-d
   :auto:

.. el:command:: bbdb-display-current-record
   :binding: C-x n d
   :auto:

.. el:command:: bbdb-display-all-records
   :binding: C-x n w
   :auto:

.. el:command:: bbdb-display-records-completely
   :binding: T
   :auto:

.. el:command:: bbdb-do-all-records
   :binding: *
   :auto:

.. el:command:: bbdb-edit-field
   :binding: e
   :auto:

.. el:command:: bbdb-edit-foo
   :binding: ;
   :auto:

.. el:command:: bbdb-help
   :binding: ?

   Display brief help

.. el:command:: bbdb-info
   :binding: h

   Display BBDB manual

.. el:command:: bbdb-insert-field
   :binding: i
   :auto:

.. el:command:: bbdb-mail
   :binding: m
   :auto:

.. el:command:: bbdb-mail-address
   :binding: M
   :auto:

.. el:command:: bbdb-mail-aliases
   :binding: A
   :auto:

.. el:command:: bbdb-merge-records
   :auto:

.. el:command:: bbdb-omit-record
   :binding: o
   :auto:

.. el:command:: bbdb-search-address
   :binding: / a
   :auto:

.. el:command:: bbdb-search-changed
   :binding: / c
   :auto:

.. el:command:: bbdb-search-duplicates
   :binding: / d
   :auto:

.. el:command:: bbdb-search-invert
   :binding: !
   :auto:

.. el:command:: bbdb-search-mail
   :binding: / m
   :auto:

.. el:command:: bbdb-search-name
   :binding: / n
   :auto:

.. el:command:: bbdb-search-organization
   :binding: / o
   :auto:

.. el:command:: bbdb-search-phone
   :binding: / p
   :auto:

.. el:command:: bbdb-search-prog
   :auto:

.. el:command:: bbdb-search-read
   :auto:

.. el:command:: bbdb-search-xfields
   :binding: / x
   :auto:

.. el:command:: bbdb-transpose-fields
   :binding: C-x C-t
   :auto:

.. el:command:: bbdb-toggle-records-layout
   :binding: t
   :auto:


.. el:command:: bbdb-display-records
   :binding: / 1
   :auto:

.. el:command:: bbdb-next-field
   :binding: <TAB>
   :auto:

.. el:command:: bbdb-next-record
   :binding: n
   :auto:

.. el:command:: bbdb-prev-field
   :binding: <DEL>
   :auto:

.. el:command:: bbdb-prev-record
   :binding: p
   :auto:

.. el:command:: bbdb-save
   :binding: s
   :auto:



Function Index
--------------

.. el:function:: bbdb-accept-message
   :auto:

.. el:function:: bbdb-address-continental-p
   :auto:

.. el:function:: bbdb-after-save
   :auto:

.. el:function:: bbdb-anniv-diary-entries
   :auto:

.. el:function:: bbdb-annotate-message
   :auto:

.. el:function:: bbdb-annotate-record
   :auto:

.. el:function:: bbdb-append-display-p
   :auto:

.. el:function:: bbdb-auto-notes
   :auto:

.. el:function:: bbdb-before-save
   :auto:

.. el:function:: bbdb-buffer
   :auto:

.. el:function:: bbdb-canonicalize-mail-1
   :auto:

.. el:function:: bbdb-change-record
   :auto:

.. el:function:: bbdb-check-name
   :auto:

.. el:function:: bbdb-check-type
   :auto:

.. el:function:: bbdb-clean-address-components
   :auto:

.. el:function:: bbdb-complete-mail
   :auto:

.. el:function:: bbdb-complete-mail-cleanup
   :auto:

.. el:function:: bbdb-completing-read-mails
   :auto:

.. el:function:: bbdb-completing-read-record
   :auto:

.. el:function:: bbdb-completing-read-records
   :auto:

.. el:function:: bbdb-completion-predicate
   :auto:

.. el:function:: bbdb-compose-mail
   :auto:

.. el:function:: bbdb-concat
   :auto:

.. el:function:: bbdb-create-internal
   :auto:

.. el:function:: bbdb-creation-date
   :auto:

.. el:function:: bbdb-creation-newer
   :auto:

.. el:function:: bbdb-creation-no-change
   :auto:

.. el:function:: bbdb-creation-older
   :auto:

.. el:function:: bbdb-current-field
   :auto:

.. el:function:: bbdb-current-record
   :auto:

.. el:function:: bbdb-decompose-bbdb-address
   :auto:

.. el:function:: bbdb-display-list
   :auto:

.. el:function:: bbdb-display-name-organization
   :auto:

.. el:function:: bbdb-display-record
   :auto:

.. el:function:: bbdb-display-record-multi-line
   :auto:

.. el:function:: bbdb-display-record-one-line
   :auto:

.. el:function:: bbdb-divide-name
   :auto:

.. el:function:: bbdb-delete-records
   :auto:

.. el:function:: bbdb-delete-redundant-mails
   :auto:

.. el:function:: bbdb-dial-number
   :auto:

.. el:function:: bbdb-display-records-with-layout
   :auto:

.. el:function:: bbdb-do-records
   :auto:

.. el:function:: bbdb-dwim-mail
   :auto:

.. el:function:: bbdb-editable
   :auto:

.. el:function:: bbdb-edit-address-default
   :auto:

.. el:function:: bbdb-edit-address-street
   :auto:

.. el:function:: bbdb-empty-record
   :auto:

.. el:function:: bbdb-extract-address-components
   :auto:

.. el:function:: bbdb-field-menu
   :auto:

.. el:function:: bbdb-fix-records
   :auto:

.. el:function:: bbdb-format-address
   :auto:

.. el:function:: bbdb-format-address-default
   :auto:

.. el:function:: bbdb-gethash
   :auto:

.. el:function:: bbdb-get-address-components
   :auto:

.. el:function:: bbdb-get-mail-aliases
   :auto:

.. el:function:: bbdb-get-records
   :auto:

.. el:function:: bbdb-goto-first-record
   :auto:

.. el:function:: bbdb-grab-url
   :auto:

.. el:function:: bbdb-hash-p
   :auto:

.. el:function:: bbdb-hash-record
   :auto:

.. el:function:: bbdb-hash-update
   :auto:

.. el:function:: bbdb-ident-point
   :auto:

.. el:function:: bbdb-ignore-message
   :auto:

.. el:function:: bbdb-initialize
   :auto:

.. el:function:: bbdb-insert-field-menu
   :auto:

.. el:function:: bbdb-insinuate-gnus
   :auto:

.. el:function:: bbdb-insinuate-message
   :auto:

.. el:function:: bbdb-insinuate-mh
   :auto:

.. el:function:: bbdb-insinuate-mu4e
   :auto:

.. el:function:: bbdb-insinuate-rmail
   :auto:

.. el:function:: bbdb-insinuate-sc
   :auto:

.. el:function:: bbdb-insinuate-vm
   :auto:

.. el:function:: bbdb-insinuate-wl
   :auto:

.. el:function:: bbdb-ispell-collect-words
   :auto:

.. el:function:: bbdb-ispell-export
   :auto:

.. el:function:: bbdb-list-transpose
   :auto:

.. el:function:: bbdb-layout-get-option
   :auto:

.. el:function:: bbdb-list-strings
   :auto:

.. el:function:: bbdb-mail-yank
   :auto:

.. el:function:: bbdb-merge-concat
   :auto:

.. el:function:: bbdb-merge-concat-remove-duplicates
   :auto:

.. el:function:: bbdb-merge-lists
   :auto:

.. el:function:: bbdb-merge-string-least
   :auto:

.. el:function:: bbdb-merge-string-most
   :auto:

.. el:function:: bbdb-merge-xfield
   :auto:

.. el:function:: bbdb-message-clean-name-default
   :auto:

.. el:variable:: bbdb-message-clean-name-function
   :auto:

.. el:function:: bbdb-message-header
   :auto:

.. el:function:: bbdb-message-search
   :auto:

.. el:function:: bbdb-migrate
   :auto:

.. el:function:: bbdb-migrate-add-country-field
   :auto:

.. el:function:: bbdb-migrate-change-dates
   :auto:

.. el:function:: bbdb-migrate-change-dates-change-field
   :auto:

.. el:function:: bbdb-migrate-organization-to-list
   :auto:

.. el:function:: bbdb-migrate-postcodes-to-strings
   :auto:

.. el:function:: bbdb-migrate-record-lambda
   :auto:

.. el:function:: bbdb-migrate-streets-to-list
   :auto:

.. el:function:: bbdb-migrate-versions-lambda
   :auto:

.. el:function:: bbdb-migrate-xfields-to-list
   :auto:

.. el:function:: bbdb-mouse-menu
   :auto:

.. el:function:: bbdb-mua
   :auto:

.. el:function:: bbdb-mua-annotate-field-interactive
   :auto:

.. el:function:: bbdb-mua-annotate-recipients
   :auto:

.. el:function:: bbdb-mua-annotate-sender
   :auto:

.. el:function:: bbdb-mua-auto-update
   :auto:

.. el:function:: bbdb-mua-auto-update-init
   :auto:

.. el:function:: bbdb-mua-display-all-recipients
   :auto:

.. el:function:: bbdb-mua-display-all-records
   :auto:

.. el:function:: bbdb-mua-display-records
   :auto:

.. el:function:: bbdb-mua-display-recipients
   :auto:

.. el:function:: bbdb-mua-display-sender
   :auto:

.. el:function:: bbdb-mua-edit-field
   :auto:

.. el:function:: bbdb-mua-edit-field-interactive
   :auto:

.. el:function:: bbdb-mua-edit-field-recipients
   :auto:

.. el:function:: bbdb-mua-edit-field-sender
   :auto:

.. el:function:: bbdb-mua-summary-mark
   :auto:
   :noindex:

.. el:function:: bbdb-mua-summary-unify
   :auto:

.. el:function:: bbdb-mua-update-interactive-p
   :auto:
   :noindex:

.. el:function:: bbdb-mua-update-records
   :auto:

.. el:function:: bbdb-mua-window-p
   :auto:

.. el:function:: bbdb-mua-wrapper
   :auto:

.. el:function:: bbdb-multiple-buffers-default
   :auto:

.. el:function:: bbdb-parse-phone
   :auto:

.. el:function:: bbdb-parse-postcode
   :auto:

.. el:function:: bbdb-parse-records
   :auto:

.. el:function:: bbdb-phone-string
   :auto:

.. el:function:: bbdb-pop-up-window
   :auto:

.. el:function:: bbdb-pop-up-window-simple
   :auto:

.. el:function:: bbdb-puthash
   :auto:

.. el:function:: bbdb-puthash-mail
   :auto:

.. el:function:: bbdb-pgp
   :auto:

.. el:function:: bbdb-prefix-message
   :auto:

.. el:function:: bbdb-print
   :auto:

.. el:function:: bbdb-print-phone
   :auto:

.. el:function:: bbdb-print-record
   :auto:

.. el:function:: bbdb-print-tex-quote
   :auto:

.. el:function:: bbdb-query-create
   :auto:

.. el:function:: bbdb-read-string
   :auto:

.. el:function:: bbdb-redisplay-record-globally
   :auto:

.. el:function:: bbdb-redisplay-record
   :auto:

.. el:function:: bbdb-remhash
   :auto:

.. el:function:: bbdb-revert-buffer
   :auto:

.. el:function:: bbdb-read-field
   :auto:

.. el:function:: bbdb-read-organization
   :auto:

.. el:function:: bbdb-read-record
   :auto:

.. el:function:: bbdb-read-xfield
   :auto:

.. el:function:: bbdb-read-xfield-pgp-mail
   :auto:

.. el:function:: bbdb-record-edit-address
   :auto:

.. el:function:: bbdb-record-edit-phone
   :auto:

.. el:function:: bbdb-record-field
   :auto:

.. el:function:: bbdb-record-list
   :auto:

.. el:function:: bbdb-record-name
   :auto:

.. el:function:: bbdb-record-name-lf
   :auto:

.. el:function:: bbdb-record-set-field
   :auto:

.. el:function:: bbdb-record-set-name
   :auto:

.. el:function:: bbdb-record-set-sortkey
   :auto:

.. el:function:: bbdb-record-set-xfield
   :auto:

.. el:function:: bbdb-record-xfield-intern
   :auto:

.. el:function:: bbdb-record-xfield-string
   :auto:

.. el:function:: bbdb-sc-get-attrib
   :auto:

.. el:function:: bbdb-sc-set-attrib
   :auto:

.. el:function:: bbdb-sc-update-from
   :auto:

.. el:function:: bbdb-scan-property
   :auto:

.. el:function:: bbdb-select-message
   :auto:

.. el:function:: bbdb-sendmail-menu
   :auto:

.. el:function:: bbdb-sort-records
   :auto:

.. el:function:: bbdb-split
   :auto:

.. el:function:: bbdb-string-trim
   :auto:

.. el:function:: bbdb-snarf
   :auto:

.. el:function:: bbdb-snarf-address-eu
   :auto:

.. el:function:: bbdb-snarf-address-us
   :auto:

.. el:function:: bbdb-snarf-empty-lines
   :auto:

.. el:function:: bbdb-snarf-label
   :auto:

.. el:function:: bbdb-snarf-mail
   :auto:

.. el:function:: bbdb-snarf-name
   :auto:

.. el:function:: bbdb-snarf-name-mail
   :auto:

.. el:function:: bbdb-snarf-notes
   :auto:

.. el:function:: bbdb-snarf-paragraph
   :auto:

.. el:function:: bbdb-snarf-phone-eu
   :auto:

.. el:function:: bbdb-snarf-phone-nanp
   :auto:

.. el:function:: bbdb-snarf-streets
   :auto:

.. el:function:: bbdb-snarf-surrounding-space
   :auto:

.. el:function:: bbdb-snarf-url
   :auto:

.. el:function:: bbdb-snarf-yank
   :auto:

.. el:function:: bbdb-sort-addresses
   :auto:

.. el:function:: bbdb-sort-phones
   :auto:

.. el:function:: bbdb-sort-xfields
   :auto:

.. el:function:: bbdb-timestamp
   :auto:

.. el:function:: bbdb-timestamp-newer
   :auto:

.. el:function:: bbdb-timestamp-older
   :auto:

.. el:function:: bbdb-touch-records
   :auto:

.. el:function:: bbdb-undisplay-records
   :auto:

.. el:function:: bbdb-undocumented-variables
   :auto:

.. el:function:: bbdb-update-records
   :auto:

.. el:function:: bbdb-version
   :auto:

.. el:function:: bbdb-warn
   :auto:

.. el:function:: bbdb/gnus-nnimap-folder-list-from-bbdb
   :auto:

.. el:function:: bbdb/gnus-score
   :auto:

.. el:function:: bbdb/gnus-score-as-text
   :auto:

.. el:function:: bbdb/gnus-score-invalidate-alist
   :auto:

.. el:function:: bbdb/gnus-split-method
   :auto:

.. el:function:: bbdb/gnus-split-to-group
   :auto:

.. el:function:: bbdb/mh-header
   :auto:

.. el:function:: bbdb/rmail-header
   :auto:

.. el:function:: bbdb/rmail-new-flag
   :auto:

.. el:function:: bbdb/vm-auto-add-label
   :auto:

.. el:function:: bbdb/vm-auto-folder
   :auto:

.. el:function:: bbdb/vm-virtual-folder
   :auto:

.. el:function:: vm-summary-function-B
   :auto:



Variable Index
--------------

.. el:variable:: bbdb-accept-message-alist
   :auto:

.. el:variable:: bbdb-add-aka
   :auto:

.. el:variable:: bbdb-add-mails
   :auto:

.. el:variable:: bbdb-add-name
   :auto:

.. el:variable:: bbdb-address-format-list
   :auto:

.. el:variable:: bbdb-address-label-list
   :auto:

.. el:variable:: bbdb-allow-duplicates
   :auto:

.. el:variable:: bbdb-anniv-alist
   :auto:

.. el:variable:: bbdb-annotate-field
   :auto:

.. el:variable:: bbdb-append-display
   :auto:
   :noindex:

.. el:variable:: bbdb-auto-notes-ignore-headers
   :auto:

.. el:variable:: bbdb-auto-notes-ignore-messages
   :auto:

.. el:variable:: bbdb-auto-notes-rules
   :auto:

.. el:variable:: bbdb-auto-notes-rules-expanded
   :auto:

.. el:variable:: bbdb-auto-revert
   :auto:

.. el:variable:: bbdb-buffer-name
   :auto:

.. el:variable:: bbdb-canonical-hosts
   :auto:

.. el:variable:: bbdb-canonicalize-mail-function
   :auto:

.. el:variable:: bbdb-case-fold-search
   :auto:

.. el:variable:: bbdb-changed-records
   :auto:

.. el:variable:: bbdb-check-auto-save-file
   :auto:

.. el:variable:: bbdb-check-postcode
   :auto:

.. el:variable:: bbdb-city-list
   :auto:

.. el:variable:: bbdb-complete-mail
   :auto:
   :noindex:

.. el:variable:: bbdb-complete-mail-allow-cycling
   :auto:

.. el:variable:: bbdb-completion-display-record
   :auto:

.. el:variable:: bbdb-completion-list
   :auto:

.. el:variable:: bbdb-continental-postcode-regexp
   :auto:

.. el:variable:: bbdb-country-list
   :auto:

.. el:variable:: bbdb-debug
   :auto:

.. el:variable:: bbdb-dedicated-window
   :auto:

.. el:variable:: bbdb-default-area-code
   :auto:

.. el:variable:: bbdb-default-country
   :auto:

.. el:variable:: bbdb-default-domain
   :auto:

.. el:variable:: bbdb-default-label-list
   :auto:

.. el:variable:: bbdb-default-separator
   :auto:

.. el:variable:: bbdb-default-xfield
   :auto:

.. el:variable:: bbdb-dial-function
   :auto:

.. el:variable:: bbdb-dial-local-prefix
   :auto:

.. el:variable:: bbdb-dial-local-prefix-alist
   :auto:

.. el:variable:: bbdb-dial-long-distance-prefix
   :auto:

.. el:variable:: bbdb-edit-foo
   :auto:

.. el:variable:: bbdb-end-marker
   :auto:

.. el:variable:: bbdb-file
   :auto:

.. el:variable:: bbdb-file-remote
   :auto:

.. el:variable:: bbdb-file-remote-save-always
   :auto:

.. el:variable:: bbdb-hashtable
   :auto:

.. el:variable:: bbdb-horiz-pop-up-window-size
   :auto:

.. el:variable:: bbdb-ignore-message-alist
   :auto:

.. el:variable:: bbdb-ignore-redundant-mails
   :auto:

.. el:variable:: bbdb-image
   :auto:

.. el:variable:: bbdb-image-path
   :auto:

.. el:variable:: bbdb-image-suffixes
   :auto:

.. el:variable:: bbdb-info-file
   :auto:

.. el:variable:: bbdb-init-forms
   :auto:

.. el:variable:: bbdb-ispell-dictionary-list
   :auto:

.. el:variable:: bbdb-ispell-field-list
   :auto:

.. el:variable:: bbdb-ispell-ignore-re
   :auto:

.. el:variable:: bbdb-ispell-min-word-length
   :auto:

.. el:variable:: bbdb-ispell-word-list
   :auto:

.. el:variable:: bbdb-lastname-prefixes
   :auto:

.. el:variable:: bbdb-lastname-re
   :auto:

.. el:variable:: bbdb-lastname-suffix-re
   :auto:

.. el:variable:: bbdb-lastname-suffixes
   :auto:

.. el:variable:: bbdb-layout
   :auto:

.. el:variable:: bbdb-layout-alist
   :auto:

.. el:variable:: bbdb-legal-postcodes
   :auto:

.. el:variable:: bbdb-mail-alias
   :auto:

.. el:variable:: bbdb-mail-alias-field
   :auto:

.. el:variable:: bbdb-mail-aliases-need-rebuilt
   :auto:

.. el:variable:: bbdb-mail-avoid-redundancy
   :auto:

.. el:variable:: bbdb-mail-name
   :auto:

.. el:variable:: bbdb-mail-name-format
   :auto:

.. el:variable:: bbdb-mail-user-agent
   :auto:

.. el:variable:: bbdb-merge-xfield-function-alist
   :auto:

.. el:variable:: bbdb-message-all-addresses
   :auto:

.. el:variable:: bbdb-message-clean-name-function
   :auto:

.. el:variable:: bbdb-message-headers
   :auto:

.. el:variable:: bbdb-message-mail-as-name
   :auto:

.. el:variable:: bbdb-message-try-all-headers
   :auto:

.. el:variable:: bbdb-mua-auto-update-p
   :auto:

.. el:variable:: bbdb-mua-edit-field
   :auto:

.. el:variable:: bbdb-mua-pop-up
   :auto:

.. el:variable:: bbdb-mua-pop-up-window-size
   :auto:

.. el:variable:: bbdb-mua-summary-mark
   :auto:

.. el:variable:: bbdb-mua-summary-mark-field
   :auto:

.. el:variable:: bbdb-mua-summary-mark-format-letter
   :auto:

.. el:variable:: bbdb-mua-summary-unification-list
   :auto:

.. el:variable:: bbdb-mua-summary-unify-format-letter
   :auto:

.. el:variable:: bbdb-mua-update-interactive-p
   :auto:

.. el:variable:: bbdb-multiple-buffers
   :auto:

.. el:variable:: bbdb-modeline-info
   :auto:

.. el:variable:: bbdb-mode-map
   :auto:

.. el:variable:: bbdb-name-face-alist
   :auto:

.. el:variable:: bbdb-name-format
   :auto:

.. el:variable:: bbdb-new-mails-primary
   :auto:

.. el:variable:: bbdb-offer-to-create
   :auto:

.. el:variable:: bbdb-organization-list
   :auto:

.. el:variable:: bbdb-phone-label-list
   :auto:

.. el:variable:: bbdb-phone-style
   :auto:

.. el:variable:: bbdb-pgp-default
   :auto:

.. el:variable:: bbdb-pgp-field
   :auto:

.. el:variable:: bbdb-pgp-headers
   :auto:

.. el:variable:: bbdb-pgp-method
   :auto:

.. el:variable:: bbdb-pgp-method-alist
   :auto:

.. el:variable:: bbdb-pgp-ranked-actions
   :auto:

.. el:variable:: bbdb-postcode-list
   :auto:

.. el:variable:: bbdb-pop-up-layout
   :auto:

.. el:variable:: bbdb-pop-up-window-size
   :auto:

.. el:variable:: bbdb-print-tex-path
   :auto:

.. el:variable:: bbdb-print-address-format-list
   :auto:

.. el:variable:: bbdb-print-alist
   :auto:

.. el:variable:: bbdb-print-brief-alist
   :auto:

.. el:variable:: bbdb-print-epilog
   :auto:

.. el:variable:: bbdb-print-file
   :auto:

.. el:variable:: bbdb-print-full-alist
   :auto:

.. el:variable:: bbdb-print-mail
   :auto:

.. el:variable:: bbdb-print-name
   :auto:

.. el:variable:: bbdb-print-name-format
   :auto:

.. el:variable:: bbdb-print-omit-fields
   :auto:

.. el:variable:: bbdb-print-prolog
   :auto:

.. el:variable:: bbdb-print-require
   :auto:

.. el:variable:: bbdb-print-tex-quote-alist
   :auto:

.. el:variable:: bbdb-read-name-format
   :auto:

.. el:variable:: bbdb-read-only
   :auto:

.. el:variable:: bbdb-records
   :auto:

.. el:variable:: bbdb-sc-attribution-field
   :auto:

.. el:variable:: bbdb-sc-last-attrib
   :auto:

.. el:variable:: bbdb-sc-update-attrib-p
   :auto:

.. el:variable:: bbdb-sc-update-records-p
   :auto:

.. el:variable:: bbdb-search-invert
   :auto:
   :noindex:

.. el:variable:: bbdb-separator-alist
   :auto:

.. el:variable:: bbdb-silent
   :auto:

.. el:variable:: bbdb-silent-internal
   :auto:

.. el:variable:: bbdb-snarf-address-eu-country
   :auto:

.. el:variable:: bbdb-snarf-address-us-country
   :auto:

.. el:variable:: bbdb-snarf-default-label-alist
   :auto:

.. el:variable:: bbdb-snarf-mail-regexp
   :auto:

.. el:variable:: bbdb-snarf-name-regexp
   :auto:

.. el:variable:: bbdb-snarf-phone-eu-regexp
   :auto:

.. el:variable:: bbdb-snarf-phone-nanp-regexp
   :auto:

.. el:variable:: bbdb-snarf-postcode-eu-regexp
   :auto:

.. el:variable:: bbdb-snarf-rule-alist
   :auto:

.. el:variable:: bbdb-snarf-rule-default
   :auto:

.. el:variable:: bbdb-snarf-url
   :auto:

.. el:variable:: bbdb-snarf-url-regexp
   :auto:

.. el:variable:: bbdb-state-list
   :auto:

.. el:variable:: bbdb-street-list
   :auto:

.. el:variable:: bbdb-update-records-address
   :auto:

.. el:variable:: bbdb-update-records-p
   :auto:

.. el:variable:: bbdb-update-unchanged-records
   :auto:

.. el:variable:: bbdb-user-mail-address-re
   :auto:

.. el:variable:: bbdb-user-menu-commands
   :auto:

.. el:variable:: bbdb-wrap-column
   :auto:

.. el:variable:: bbdb-xfield-label-list
   :auto:

.. el:variable:: bbdb-xfields-sort-order
   :auto:

.. el:variable:: bbdb/gnus-score-alist
   :auto:

.. el:variable:: bbdb/gnus-score-default
   :auto:

.. el:variable:: bbdb/gnus-score-field
   :auto:

.. el:variable:: bbdb/gnus-score-rebuild-alist
   :auto:

.. el:variable:: bbdb/gnus-split-crosspost-default
   :auto:

.. el:variable:: bbdb/gnus-split-default-group
   :auto:

.. el:variable:: bbdb/gnus-split-myaddr-regexp
   :auto:

.. el:variable:: bbdb/gnus-split-nomatch-function
   :auto:

.. el:variable:: bbdb/gnus-split-private-field
   :auto:

.. el:variable:: bbdb/gnus-split-public-field
   :auto:

.. el:variable:: bbdb/vm-auto-add-label-field
   :auto:

.. el:variable:: bbdb/vm-auto-add-label-list
   :auto:

.. el:variable:: bbdb/vm-auto-folder-headers
   :auto:

.. el:variable:: bbdb/vm-auto-folder-field
   :auto:

.. el:variable:: bbdb/vm-virtual-folder-field
   :auto:

.. el:variable:: bbdb/vm-virtual-real-folders
   :auto:


Constants
---------

.. el:constant:: bbdb-migration-spec
   :auto:

.. el:constant:: bbdb-mua-mode-alist
   :auto:

.. el:constant:: bbdb-version
   :auto:

.. el:constant:: bbdb-version-date
   :auto:


Hooks
-----

.. el:hook:: bbdb-after-change-hook
   :auto:

.. el:hook:: bbdb-after-read-db-hook
   :auto:

.. el:hook:: bbdb-after-save-hook
   :auto:

.. el:hook:: bbdb-before-save-hook
   :auto:

.. el:hook:: bbdb-change-hook
   :auto:

.. el:hook:: bbdb-complete-mail-hook
   :auto:

.. el:hook:: bbdb-create-hook
   :auto:

.. el:hook:: bbdb-display-hook
   :auto:

.. el:hook:: bbdb-initialize-hook
   :auto:

.. el:hook:: bbdb-mail-abbrev-expand-hook
   :auto:

.. el:hook:: bbdb-mode-hook
   :auto:

.. el:hook:: bbdb-notice-mail-hook
   :auto:

.. el:hook:: bbdb-notice-record-hook
   :auto:
