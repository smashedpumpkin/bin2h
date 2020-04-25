# bin2h

A small tool for converting binary data to a C-style uchar array for compiling straight into C/C++ code. 

Builds with CMake & tested on Windows, MacOS. 

Binaries for tested platforms available via GitHub package feed.

Carried over from http://code.google.com/p/bin2h.

---

```bin2h utility v1.01

Interprets any file as plain binary data and dumps to a raw C/C++ array.
usage: bin2h <in-file> <out-file> <opt-args>

Valid optional arguments:
-id=<name> the C array is identified as "name". identifier is "data" if this argument is not present. bin2h does not check the identifier is valid in C/C++.
-ns=<namespace> causes the data to be wrapped in a namespace. no namespace is inserted if this argument is not used.```