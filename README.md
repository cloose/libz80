libz80 - Z80 emulation library 
===============================

*© Gabriel Gambetta (gabriel.gambetta@gmail.com) 2000 - 2013*

*Version 2.1.0*

Building and Installing
-----------------------

The Makefile creates `libz80.so`, which together with `z80.h` make up the binary
package. `make install` installs these files in `/usr/lib` and `/usr/include`
respectively.

Emulation code itself is generated by the `codegen` folder. `mktables.spec`
includes a specification of the opcodes, using regular expressions to express
similar opcodes in a compact way. Binary representation of the opcodes is listed
in `opcodes.lst`. This makes tweaking the 'processor' relatively easy, as it
isn't done manually.

The tests folder includes a simple test framework and a few tests to ensure the
current behavior of the processor.

Authors
-------

Gabriel Gambetta (gabriel.gambetta@gmail.com)

Wayne Conrad (wconrad@yagni.com) - MAJOR fixes and emulation improvements.


