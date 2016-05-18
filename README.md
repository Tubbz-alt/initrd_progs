initrd_progs
============

programs, including busybox, statically linked for the initial ram disk

This should produce all the statically linked programs required for a Puppy Linux initrd.gz

This is also a place of experimentation.

Usage
-----
Run `./build.sh` or `./build.sh -help` to see the available options

- hopefully a musl build environment downloads from http://landley.net/aboriginal/
- by default an attempt will be made to build all packages in the queue defined in build.conf
- for more options look in build.conf

The script can also generate an initrd.gz file ready to test, you can add these files:
- 0initrd/DISTRO_SPECS (optional, otherwise it will use the system one)
- 0initrd/init (optional custom init script)

BUGS
----
- some builds may need some fine tuning
- some builds might fail

Report any issues you find
