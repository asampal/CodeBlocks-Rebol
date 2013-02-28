This is a [Code::Blocks](http://codeblocks.org) project file for [Rebol](http://rebol.com)


Instructions:

The project assumes the source layout of the official GitHub Rebol repo. Put the project file (r3.cbp) at the root of this directory structure, r3-make.exe (a renamed [Rebol executable](http://rebolsource.com) used in some pre-build steps) in the `make` directory and make-make.r in `src/tools` to overwrite the existing one.

The makefile will build an executable that doesn't include graphics support (as does the one from the official GitHub repo). Saphirion has a build that produces an exe with graphics support, but I'm not sure what the differences are relative to the official source. If you want to build with [Saphirion's source](http://development.saphirion.com/downloads/), be aware that make-make.r might need some slight adjustments. You should be able to diff the one included here and theirs in order to figure out what changes need to be made.

If you select the Release target in Code::Blocks, you'll end up stripping debug symbols from the executable. The Debug target retains them, so use this for debugging. To debug, just choose "Start/Continue" from the debug menu in CB.

If you want to be able to use some of the C code navigation features in CB, like "find functions calling/called by ...", you should install [Cscope](http://code.google.com/p/cscope-win32) (Code::Blocks integrates with this through a built-in plugin). You can, even without this, go to declarations and implementations of functions (right-click on a symbol).


If you've got questions about this or just want some real-time Rebol/Red chat, drop by the [StackOverflow Rebol/Red chat](http://chat.stackoverflow.com/rooms/291/rebol-and-red) and ask away, if I'm (Adrian) there. Come check out the new bot by Graham.
