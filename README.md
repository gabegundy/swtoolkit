# Software Construction Toolkit - a set of extensions for SCons

*This is the README.md file for the Software Construction Toolkit.*

You are likely reading this file in one of the following two situations:

 #1 You have downloaded Software Construction Toolkit from code.google.com and are examining the contents.
 #1 This file was included in some other software package so that the package could be built using Software Construction Toolkit. In this case, follow the instructions provided with the rest of the software package for how to use Software Construction Toolkit to build and/or install the software.

## LATEST VERSION

Once upon a time, this code was hosted at [Google Code](http://code.google.com/p/swtoolkit). Now it's been archived. There are a number of GitHub clones, but none appear to be authoritative. I'm cloning here as well, but I'm updating the README.md to reflect this reality.

## EXECUTION REQUIREMENTS

Software Construction Toolkit requires:

  * Python 2.4 or later.
    * For example, from http://www.python.org
    * If on Windows, also need the [pywin32 extensions](http://sourceforge.net/projects/pywin32/)
    * Software Construction Toolkit is not yet compatible with Python 3.

  * SCons 1.2 or later.
    * For example, from http://www.scons.org/download.php
    * A scons or scons-local install is required for building projects.
    * A scons-src install is required for developing Software Construction Toolkit.

There should be no other direct dependencies or requirements to run the
Software Construction Toolkit.

## INSTALLATION

Installation of this package is as simple as copying its directory tree to any
directory.

If you are using the hammer.bat or hammer.sh entry point, you also need to set
up a SCONS_DIR environment variable to point to the directory containing SCons.

  * For a normal SCons install, this is the engine subdir.
  * For a scons-local install, this is the . subdir.
  * For a scons-src install, this is the src/engine subdir.
  * For a Windows install of SCons which used a .exe or .msi installer, SCons may be installed in a subdirectory of the Python directory. For example, `C:\Python24\Lib\site-packages\scons-1.2.0`.

If you are modifying Software Construction Toolkit and need to run the unit tests, set up a SCONS_DEV_DIR environment variable to point to the directory containing the scons-src install.

Once you have installed this package, you should write a main.scons file at the top level of your source tree to build your software.

Then modify the build/install instructions for your package to instruct your users to execute Software Construction Toolkit by running hammer.bat or hammer.sh.

## CONTENTS OF THIS PACKAGE

This package consists of the following:

#### COPYING
A copy of the copyright and terms under which Software Construction Toolkit is distributed (the BSD license).

#### README.md

What you're looking at right now.

#### history.txt

Change history for major releases.

## hammer.bat

The entry point for Software Construction Toolkit on Windows.

#### hammer.sh

The entry point for Software Construction Toolkit on posix and unix-like systems, including Cygwin.

#### wrapper.py

A script called by hammer which does some additional setup and then calls SCons.

#### site_scons/

Tools and modules for Software Construction Toolkit.

#### samples/

Sample projects which demonstrate usage of the Software Construction Toolkit.

#### bin/

Additional executables and utilities for developing the Software Construction Toolkit, including the test-runner.

#### lib/

Additional libraries for developing the Software Construction Toolkit, including the test framework module.

#### test/

Tests for Software Construction Toolkit.

## DOCUMENTATION

At one time, up-to-date documentation for the Software Construction Toolkit could be found online at its [archived homepage](https://code.google.com/archive/p/swtoolkit/). In theory that remains true until someone takes up the project.

## LICENSING

Software Construction Toolkit is distributed under the BSD license, a full copy of which is available in the COPYING file in this package.

## REPORTING BUGS

Once upon a time, you could report Software Construction Toolkit bugs at the Issues link on the Software Construction Toolkit's [Issues Page](https://code.google.com/archive/p/swtoolkit/issues). Now it's just an archive of old issues. You can open issues here too, but I'm not in any position to take this project over. Maybe someone will come along and take it over.

## MAILING LISTS
=============

A mailing list for users of Software Construction Toolkit is available.  You may send questions or comments to the list at:

`swtoolkit@googlegroups.com`

You may subscribe to the mailing list at:

`https://groups.google.com/forum/#!forum/swtoolkit`

It hasn't seen action for a few years.

## AUTHOR INFO

Randall Spangler <randall dot spangler at gmail dot com>

With plenty of help from the Software Construction Toolkit Development team:
  * Brad Nelson
  * Steven Knight
  * Stephen Ng
  * Greg Spencer
