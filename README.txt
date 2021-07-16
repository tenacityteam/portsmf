Portsmf is "Port Standard MIDI File", a cross-platform, C++ library
for reading and writing Standard MIDI Files.

License information:
free and open source, see license.txt for details

Building:
PortSMF has no dependencies and uses the CMake build system.
To build it, run:

$ cmake -DCMAKE_INSTALL_PREFIX=/where/you/want/to/install/to -S . -B build
$ cmake --build build --parallel number-of-cpu-cores
$ cmake --install build

Features:

- input and output of Standard MIDI Files
- data structures, classes, etc. for representing music data in memory
    o sequence structure consisting of multiple tracks
    o track structure consisting of multiple events
    o events contain note and control data
    o extensible attribute-value property lists
    o tempo track and time signature representation
- input and output of a text-based representation: Allegro files
- extensive editing operations on sequences and tracks
- conversion to/from binary buffers for archiving, undo/redo, etc.
