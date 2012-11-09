Org-Mode to Confluence exporter
===============================

Forked from https://github.com/hgschmie/org-confluence, which provided
inspiration to move this code to the new org-export.el shipped with
org-mode 7.9.2.

Installation
------------

Get a release of org-mode >= 7.9.2, or the latest one from
git://orgmode.org/org-mode.git.

Install it and make sure that your emacs has access to the
org-export.el file that's part of org-mode's contrib section.

Copy org-confluence.el onto the load path of the emacs installation.

Add

  (require 'org-confluence)

to the .emacs startup file.

If all went well, the command M-x org-e-confluence-export-as-confluence 
should write a buffer with a confluence styled export.

What it does
------------

- bold, italics, underline, strikethrough and monospaced text
- headings
- "internal" Confluence links with `confluence:Space:Page` notation
- external links
- BLOCK_SRC and BLOCK_EXAMPLE to code blocks (with different theme)
- lists (unnumbered and numbered)
- tables (header lines, body lines)

That is, exactly everything that's used in test.org.

What it does not
----------------

- everything else


What would be cool
------------------

- Integration with http://code.google.com/p/confluence-el/
- reformat existing text blocks to be lines without breaks (confluence likes it this way)

Copyright
---------

Copyright 2012 Sébastien Delafond
\\
Copyright 2012 Henning Schmiedehausen
