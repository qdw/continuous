Continuous Testing
==================

"Continous testing" means automatically running your tests whenever you save
changes to your code. It's a nice approach. It gives you instant feedback,
and it saves you a  lot of typing.

Usage
=====

It's super-simple. Open a terminal emulator and run

    ./autotest my-test-file

This will re-run your test file whenever you save it[1].

Also included is on-file-change-do, a more generic shell quickie for running
some action when a file changes. It works like this:

    ./on-file-change-do file-to-monitor 'shell command to run'

Requirements
============
* A Unix environment.
* Bash. This comes preinstalled with your Unix environment if you're using
  Linux, OS X, or Cygwin.

Installation
============
1. Edit your shell init file and append this directory to PATH.
1. There is no step 2.

Footnotes
=========

[1] This assumes you're able to execute your test file. You will be if you
remember to 'chmod u+x my-test-file', and if you use the shebang syntax
for tests in interpreted programming languages, that is, start the file
with

#!/bin/sh

or

#!/usr/bin/env python

or whatever.
