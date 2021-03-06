==========
Change log
==========

`Next version`_
===============

`1.3`_ (2017-09-22)
====================

- Fixed a case where tags with content between them were erroneously merged.
- Added a ``tox.ini`` file for running style checks and tests.
- Replaced ``REPLACEMENTS`` and ``element_filters`` with the more
  general ``element_preprocessors`` and ``element_postprocessors``
  settings.
- Removed the restriction that ``<span>`` tags are never allowed.


`1.2`_ (2017-05-25)
====================

- Fixed the erroneous removal of all whitespace between adjacent
  elements.
- Fixed a few occasions where ``<br>`` tags were erroneously removed.
- Back to beautifulsoup4 for especially broken HTML respectively HTML
  with Emojis on macOS.
- Used a ``<div>`` instead of ``<anything>`` to wrap the document (since
  beautifulsoup4 does not like custom tags too much)


`1.1`_ (2017-05-02)
====================

- Added ``html_sanitizer.django.get_sanitizer`` to provide an official
  way of configuring HTML sanitizers using Django settings.


`1.0`_ (2017-05-02)
====================

- Initial public release.


.. _feincms-cleanse: https://pypi.python.org/pypi/feincms-cleanse/
.. _html-sanitizer: https://pypi.python.org/pypi/html-sanitizer/

.. _1.0: https://github.com/matthiask/html-sanitizer/commit/4a995538f
.. _1.1: https://github.com/matthiask/html-sanitizer/compare/1.0...1.1
.. _1.2: https://github.com/matthiask/html-sanitizer/compare/1.1...1.2
.. _1.3: https://github.com/matthiask/html-sanitizer/compare/1.2...1.3
.. _Next version: https://github.com/matthiask/html-sanitizer/compare/1.3...master
