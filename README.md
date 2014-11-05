OpenJDK-trim
============

The purpose of this tool is to re-package an existing OpenJDK build to remove
classes that are not used by your application.

This can bring a typical JRE size from 100 MB down to 10 MB.

Usage
=====

1. Configure the files you want to keep in `classes.filter` and `files.filter`
   - `files.filter` will be applied to the whole JDK directory
   - `classes.filter` will be applied to the JRE jars

2. Call jdk-trim with a path to an OpenJDK build and an output path.

Author
======

Gregory Schlomoff <greg@aerofs.com>
