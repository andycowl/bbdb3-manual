Lisp library (bbdb)
===================

.. el:require:: bbdb

Commands
--------

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


Functions
---------

.. el:function:: bbdb-address-continental-p
   :auto:

.. el:function:: bbdb-after-save
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

.. el:function:: bbdb-concat
   :auto:

.. el:function:: bbdb-creation-date
   :auto:

.. el:function:: bbdb-current-field
   :auto:

.. el:function:: bbdb-current-record
   :auto:

.. el:function:: bbdb-decompose-bbdb-address
   :auto:

.. el:function:: bbdb-delete-record-internal
   :auto:

.. el:function:: bbdb-display-list
   :auto:

.. el:function:: bbdb-display-name-organization
   :auto:

.. el:function:: bbdb-display-record-multi-line
   :auto:

.. el:function:: bbdb-display-record-one-line
   :auto:

.. el:function:: bbdb-display-record
   :auto:

.. el:function:: bbdb-divide-name
   :auto:

.. el:function:: bbdb-editable
   :auto:

.. el:function:: bbdb-empty-record
   :auto:

.. el:function:: bbdb-extract-address-components
   :auto:

.. el:function:: bbdb-field-menu
   :auto:

.. el:function:: bbdb-format-address
   :auto:

.. el:function:: bbdb-format-address-default
   :auto:

.. el:function:: bbdb-gethash
   :auto:

.. el:function:: bbdb-goto-first-record
   :auto:

.. el:function:: bbdb-hash-p
   :auto:

.. el:function:: bbdb-hash-record
   :auto:

.. el:function:: bbdb-hash-update
   :auto:

.. el:function:: bbdb-initialize
   :auto:

.. el:function:: bbdb-insert-field-menu
   :auto:

.. el:function:: bbdb-insert-record-internal
   :auto:

.. el:function:: bbdb-layout-get-option
   :auto:

.. el:function:: bbdb-list-strings
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

.. el:function:: bbdb-mouse-menu
   :auto:

.. el:function:: bbdb-message-clean-name-default
   :auto:

.. el:variable:: bbdb-message-clean-name-function
   :auto:

.. el:function:: bbdb-mouse-menu
   :auto:

.. el:function:: bbdb-multiple-buffers-default
   :auto:

.. el:function:: bbdb-overwrite-record-internal
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

.. el:function:: bbdb-read-string
   :auto:

.. el:function:: bbdb-record-field
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

.. el:function:: bbdb-redisplay-record-globally
   :auto:

.. el:function:: bbdb-redisplay-record
   :auto:

.. el:function:: bbdb-remhash
   :auto:

.. el:function:: bbdb-revert-buffer
   :auto:

.. el:function:: bbdb-scan-property
   :auto:

.. el:function:: bbdb-sendmail-menu
   :auto:

.. el:function:: bbdb-sort-records
   :auto:

.. el:function:: bbdb-split
   :auto:

.. el:function:: bbdb-string-trim
   :auto:

.. el:function:: bbdb-timestamp
   :auto:

.. el:function:: bbdb-undisplay-records
   :auto:

.. el:function:: bbdb-version
   :auto:

.. el:function:: bbdb-warn
   :auto:

Variables
---------

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

.. el:variable:: bbdb-do-all-records
      :noindex:

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

.. el:variable:: bbdb-postcode-list
   :auto:

.. el:variable:: bbdb-pop-up-layout
   :auto:

.. el:variable:: bbdb-pop-up-window-size
   :auto:

.. el:variable:: bbdb-read-name-format
   :auto:

.. el:variable:: bbdb-read-only
   :auto:

.. el:variable:: bbdb-records
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
