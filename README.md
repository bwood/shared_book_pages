This module allows Drupal 7 books to share pages.  It's written after
considering the information in https://drupal.org/node/5901.

Version 0.1:

* Taxonomy is used to define relationships between shared pages.
* Sharing page 3 from Book A with Book B means creating a placeholder page in Book B that is tagged with the "shared pages" taxonomy vocabulary.
* When Book B's placeholder page is loaded hook\_entity\_load() is used to swap in the title and body from the source node object. Some people may consider this playing dirty.
