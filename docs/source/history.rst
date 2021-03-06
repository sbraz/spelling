=================
 Release History
=================

.. spelling::

   unmaintained

.. release-notes::

5.1.2
=====

- Mark as unsafe for parallel builds (contributed by Jared Dillard)
- Add -W arg to sphinx-build in docs so warnings cause error
  (contributed by Elsa Gonsiorowski, PhD)

5.1.0
=====

- Add an option to show the line containing a misspelling for context
  (contributed by Huon Wilson)

5.0.0
=====

- Drop Python 2.7 support. (contributed by Johannes Raggam)
- `allow customizing with classes using import strings
  <https://github.com/sphinx-contrib/spelling/pull/40>`__
- pyenchant is now maintained (contributed by Adam Johnson

4.3.0
=====

- Logging: use warning() instead of its deprecated alias (contributed
  by Sergey Kolosov)
- Support additional contractions (contributed by David Baumgold)
- require sphinx >= 2.0.0
- declare support for python 3.6

4.2.1
=====

- fix remaining logging issue (contributed by Timotheus Kampik)
- Remove usage of deprecated logging API (contributed by Tim Graham)

4.2.0
=====

- Fix a bug with empty word lists (contributed by FabioRosado)
- Update dependency management to use setuptools extras
- Document how to create multiple wordfiles (contributed by
  FabioRosado)
- Note that PyEnchant is unmaintained and fix links (contributed by
  Marti Raudsepp)
- Don’t use mutable default argument (contributed by Daniele Tricoli)

4.1.0
=====

- Make it possible to provide several wordlists (contributed by Tobias
  Olausson)
- Update developer documentation (contributed by Tobias Olausson)
- Update home page link (contributed by Devin Sevilla)

4.0.1
=====

- use the right method to emit warnings
- disable smart quotes so that we can recognize
  contractions/possessives correctly (contributed by Alex Gaynor)

4.0.0
=====

- Don’t fail by default (contributed by Stephen Finucane)
- Mark the extension as safe for parallel reading (contributed by Alex
  Gaynor)
- be more verbose about configuration options
- switch to testrepository for running tests
- update python 3.3 to 3.5

2.3.0
=====

- make it possible to specify tokenizer #7 (contributed by Timotheus
  Kampik)

2.2.0
=====

- Use ``https`` with ``pypi.python.org`` package name checker
  (contributed by John-Scott Atlakson)
- Removed unnecessary shebang lines from non-script files (contributed
  by Avram Lubkin)
- Re-enable the PyEnchant dependency (contributed by Julian Berman)

2.1.2
=====

- Fixed issue with six under python 3.4

2.1.1
=====

- Use ``str.isupper()`` instead of ad-hoc method
- fix syntax for tags directive
- Removed no more used CHANGES file

2.1
===

- Fix unicode error in ``PythonBuiltinsFilter``.
- Make error output useful in emacs compiler mode
- Only show the words being added to a local dictionary if debugging
  is enabled.


2.0
===

- Add python 3.3 support.
- Add PyPy support.
- Use pbr for packaging.
- Update tox config to work with forked version of PyEnchant until
  changes are accepted upstream.

1.4
===

  - Fixed detection of builtins under PyPy, contributed by Hong Minhee
    (https://bitbucket.org/dahlia).

1.3
===

  - Handle text nodes without parents. (#19)
  - Include the input document name in the console output.
  - Use the Sphinx wrapper for registering a directive.

1.2
===

  - Add the document name to the messages showing the contents of a
    local dictionary created by the ``spelling`` directive.
  - Add title nodes to the list of node types checked for
    spelling. Resolves issue #17.
  - Add test/test_wordlist.txt to the manifest so it is included in
    the source distribution and the tests will pass. Resolves issue
    #17.
  - Documentation patch from Hank Gay.

1.1.1
=====

  - Fix initialization so the per-document filters work even if no
    ``spelling`` directive is used.

1.1
===

  - Add an option treat the names of packages on PyPI as spelled
    properly.
  - Add an option to treat CamelCase names as spelled properly.
  - Add an option to treat acronyms as spelled properly.
  - Add an option to treat Python built-ins as spelled properly.
  - Add an option to treat names that can be found as modules as
    spelled properly.
  - Add an option to let the user provide a list of other filter
    classes for the tokenizer.
  - Add ``spelling`` directive for passing local configuration
    settings to the spelling checker. This version allows setting a
    list of words known to be spelled correctly.

1.0
===

  - Re-implement using just a Builder, without a separate visitor
    class.
  - Show the file and line number of any words not appearing in the
    dictionary, instead of the section title.
  - Log the file, line, and unknown words as the documents are
    processed.

0.2
===

  - Warn but otherwise ignore unknown node types.

0.1
===

  - First public release.
