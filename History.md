0.3.1 / 2011-11-25
=================
* Now relying on cheerio-soupselect instead of node-soupselect
* Removed all lingering htmlparser dependencies
* parser now returns parent "root" element. Root now never needs to be updated when there is multiple roots. This fixes ongoing issues with before(...), after(...) and other manipulation functions
* Added jQuery's $(...).replaceWith(...)

0.3.0 / 2011-11-19
=================
* Now using htmlparser2 for parsing (2x speed increase, cleaner, actively developed)
* Added benchmark directory for future speed tests
* $("...").dom() was funky, so it was removed in favor of $("...").get(). $.dom() still works the same.
* $.root now correctly static across all instances of $
* Added a screencast

0.2.2 / 2011-11-9
=================

  * Traversing will select `<script>` and `<style>` tags (Closes Issue: #8)
  * .text(string) now working with empty elements (Closes Issue: #7)
  * Fixed before(...) & after(...) again if there is no parent (Closes Issue: #2)

0.2.1 / 2011-11-5
=================

  * Fixed before(...) & after(...) if there is no parent (Closes Issue: #2)
  * Comments now rendered correctly (Closes Issue: #5)
  

< 0.2.0 / 2011-10-31
==================

  * Initial release (untracked development)