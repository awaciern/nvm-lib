# nvm-lib
Non-Volatile Memory Library Function Definitions as described in the paper "Hardware Supported Persistent Object Address Translation" by Dr. James Tuck (NCSU).

Designed by Avery Acierno (Undergraduate Research).

# Versioning
This project has has gone through multiple design iterations. Different versions exist on different branches. The master branch contains the most recent finished version (V9).

### Version 3
Pools and regular C file I/O operate in parallel.

### Version 4
Uses pools to manipulate data seperate from C file I/O, but also have interfaces to read data from and write data to C files. Uses char data and txt files.

### Version 5
Uses pools to manipulate data seperate from C file I/O, but also have interfaces to read data from and write data to C files. Uses int* data and binary files.

### Version 7
Uses pools to manipulate data seperate from C file I/O, but also have interfaces to read data from and write data to C files. Uses void* data and is compatible with both binary and txt files.

### Version 8
Builds upon Version 7 with following enhancements:
1. Adds a closed variable to indicate when a pool is closed instead of freeing all oids in a pool when it is closed. 
2. Enables other oids to be stored in data.

### Version 9
Builds upon Version 8 with the following enhancement:
Pools and files operate seperately not in pairs: save file data into pool, manipulate, then save back.
