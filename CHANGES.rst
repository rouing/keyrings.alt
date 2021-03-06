3.1.1
=====

#31: Trap AttributeError in Gnome backend as in some environments
it seems that will happen.

#30: Fix issue where a backslash in the service name would cause
errors on Registry backend on Windows.


3.1
===

``keyrings.alt`` no longer depends on the ``keyring.util.escape``
module.

3.0
===

``keyrings`` namespace should now use the pkgutil native technique
rather than relying on pkg_resources.

2.4
===

#24: File based backends now reject non-string types for passwords.

2.3
===

#21: Raise ValueError on blank username in plaintext
keyring, unsupported in the storage format.

2.2
===

#17: Drop dependency on keyring.py27compat and use six
instead.

#16: Minor tweaks to file-based backends.

2.1
===

Add persistent scheme and version tags for file based backends.
Prepare for associated data handling in file based schemes.

2.0
===

#12: Drop kwallet support, now superseded by the dual kwallet
support in keyring.

1.3
===

#9: Moved base file backend functionality from 'keyrings.alt.file'
to 'keyrings.alt.base_file'. This allows the 'Windows' module to
no longer trigger a circular import with the 'file' module.

1.2
===

Updated project skeleton. Tests now run under tox. Tagged
commits are automatically released to PyPI.

#6: Added license file.

1.1.1
=====

Test cleanup.

Exclude tests during install.

1.1
===

FileBacked backends now have a ``repr`` that includes the file path.

1.0
===

Initial release based on Keyring 7.3.
