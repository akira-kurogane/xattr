xattr
-----

.. image:: https://travis-ci.org/xattr/xattr.svg?branch=master
    :target: https://travis-ci.org/xattr/xattr

xattr is a Python script wrapper for viewing and editing extended filesystem attributes on the command line. It is provided as an alternative to getfattr, setfattr, etc. for Unix-y environments that don't have those.

Extended attributes extend the basic attributes of files and directories
in the file system.  They are stored as name:data pairs associated with
file system objects (files, directories, symlinks, etc).

Extended attributes are currently only available on Darwin 8.0+ (Mac OS X 10.4)
and Linux 2.6+. Experimental support is included for Solaris and FreeBSD.

Note: On Linux, custom xattr keys need to be prefixed with the `user`
namespace, ie: `user.your_attr`.

https://man7.org/linux/man-pages/man1/getfattr.1.html
