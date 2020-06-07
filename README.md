A way to include bindir values in executables
=============================================

This is about hwo to include the values for bindir etc. into
executables built using Autoconf and Automake. See

  https://lists.gnu.org/archive/html/autoconf/2020-06/msg00000.html

for a more detailed discussion.


How to build from git sources
-----------------------------

    $ autoreconf -vis .
    $ ./configure
    $ make && ./aip-test
    $ make bindir=/foo/bin && ./aip-test
    $ make bindir=/foo/bin && ./aip-test
    $ make bindir=/bar/bin && ./aip-test
