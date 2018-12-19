spdx
====

A Python module incorporating an interface to the SPDX license database.

This library serves purely as a holder for the database that can be
found on `the SPDX website <https://spdx.org/licenses/>`__.

To more easily query this database or detect licenses, consider using
something like
`spdx-lookup <https://pypi.python.org/pypi/spdx-lookup>`__.

Usage
-----

See the ``spdx/__init__.py`` file for the very simple interface.

tl;dr: ``spdx.licenses()`` gets you the licenses, and ``spdx.License``
is a nice wrapper for interacting with them.

Updating
-----
To update the SPDX data, delete the content of ``spdx/data`` and copy the new content of https://github.com/spdx/license-list-data. Update the version of this Python module respectively.
Furthermore update the ``data/db.json``, which is named upstream ``json/licenses.json``.
