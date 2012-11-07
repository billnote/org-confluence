Org-Mode to Confluence exporter
===============================

Cobbled together from various pieces of org-mm.el and org-mw.el with a
hint of org-odt.el, All taken from the circa-7.7 org-mode trunk at
git://repo.or.cz/org-mode.git.

I would feel embarrassed to claim any copyright on this.

Installation
------------

Get a release of org-mode >= 7.9, or the latest one from
git://orgmode.org/org-mode.git.

Install it and make sure that your emacs has access to the
org-export.el file that's part of org-mode.

Copy org-confluence.el onto the load path of the emacs installation.

Add

    (require 'org-confluence)

to the .emacs startup file.

If all went well, the command M-x org-confluence-export should write a buffer with a confluence styled export. 

What it does
------------

- bold, italics, underline, strikethrough and monospaced text.
- headings
- links
- support Confluence internal links with `confluence:Space:Page` notation.
- BLOCK_SRC and BLOCK_EXAMPLE to code blocks
- lists (unnumbered and numbered)
- tables (header lines, body lines)


What it does not
----------------

Everything else. It is, pretty much, dumb as a rock.


What would be cool
------------------

- Integration with http://code.google.com/p/confluence-el/
- reformat existing text blocks to be lines without breaks (confluence likes it this way).
