TODO
====

* Add support for running multiple test files.

* Add support for running tests when your dependencies change, not just when
  your test file itself changes. It's probably best to adopt autoprove's
  approach: monitor a whole tree of files, and re-run the test when any one of
  them changes.
