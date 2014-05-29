auto-project
==================

auto-project is a template repository for autotools-based projects.

## First-Time Configuration

* Run `libtoolize -c -f`
* Edit `configure.ac`
* Run `autoconf`
* Run `autoheader`
* Edit `Makefile.am`
* Edit `src/Makefile.am`
* Edit `t/Makefile.am`
* Run `automake`

Or you can edit all files in one time, then run:

* `./autogen.sh`

## Build

    ./configure
    make

## Test

    make check
