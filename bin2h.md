# Introduction #

bin2h is a small tool for converting binary data into a C-style uchar array for compiling with source code.

# Details #

Compiling binary data into an executable can be useful for a whole variety of reasons, such as a need for quick access after process start-up (e.g. splash screens) or guaranteed availability (e.g. optical media or network/cloud based software). bin2h is intended to be a reasonable approximation of a small, sharp tool to convert any binary file into a format suitable for embedding in the executable binary.

# Usage #

bin2h in-file out-file optional-args

possible arguments:

  * out-file is optional, if not specified output is directed to cout
  * -id=_name_ if specified, the identifier of the C array is _name_. The identifier is _data_ if this argument is not specified.
  * -ns=_name_ if specified, the C array is placed inside a C++ namespace called _name_. If not specified, the C array is placed in the global namespace.

# Possible further work #

  * Support other (appropriate) languages
  * Remove windows-specific code, and `*`nix makefiles
  * Provide solution/project files for other version of MSVC
