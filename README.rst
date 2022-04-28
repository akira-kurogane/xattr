xattr
-----

.. image:: https://travis-ci.org/xattr/xattr.svg?branch=master
    :target: https://travis-ci.org/xattr/xattr

xattr is a Python wrapper for extended filesystem attributes. It is provided as an alternative to  [getfattr](https://man7.org/linux/man-pages/man1/getfattr.1.html), [setfattr](https://man7.org/linux/man-pages/man1/setfattr.1.html) in the [attr](http://savannah.nongnu.org/projects/attr) package for Unix-y environments that don't have those.

Extended attributes extend the basic attributes of files and directories
in the file system.  They are stored as name:data pairs associated with
file system objects (files, directories, symlinks, etc).

Extended attributes are currently only available on Darwin 8.0+ (Mac OS X 10.4)
and Linux 2.6+. Experimental support is included for Solaris and FreeBSD.

Note: On Linux, custom xattr keys need to be prefixed with the `user`
namespace, ie: `user.your_attr`.
