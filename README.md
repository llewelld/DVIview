# DVIview

View DVI files on RISC OS

Written by Paul Field

## Building from Source

DVIview can be built in a number of different ways - debug, release, profile and memcheck. The last two use HeirProf and MemCheck, commercial software available from Julian Smith that was distributed by Warm Silence Software to do profiling and to check for memory access errors and memory leaks. These aren't needed to build the release version.

The different builds all have their own !Run files and use something called Makatic to create the relevant Makefiles. If you don't have Makatic, you can use the included MakeNew Obey file instead to build the release executable.

DVIview also uses some separate libraries: ToolLib, ADTLib and OSLib. The first two were also written by Paul Field and copies are included in the repository.

## Contact

To get in contact with Paul about DVIview, or the related libraries, please use the following email address:

- Paul Field
- dviview@cloudinthesky.co.uk

I'm releasing DVIview with agreement from Paul under a GPL licence (see the LICENSE file). I can be contacted as follows:

- David Llewellyn-Jones
- david@flypig.co.uk
- http://www.flypig.oc.uk

