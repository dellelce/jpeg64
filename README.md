jpeg64
======

A modified JPEGv9 using 64x64 MCU

The standard size of Minimum Code Unit in JPEG is 8x8, my objective is to modify the 
library provided by the Independent JPEG Group to use a minimal 64x64 block and see 
how this compare in performance (size & speed) to standard JPEG.

NOTE:

* DCTSIZE/DCTSIZE2 describe the blocksize, jfdctflt.c needs to be modifed to handle the new size, minor changes in other files  may be needed.

TODO:

* Modify code in jfdctflt.c appropriately, verify other files
* Test with builtin binary
* Attempt using rebuild a viewer with the modified libjpeg
