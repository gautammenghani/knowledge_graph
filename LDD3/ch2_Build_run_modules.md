## Kernel modules vs applications
  1. While most small and medium-sized applications perform a single task from begin-
ning to end, every kernel module just registers itself in order to serve future requests,
and its initialization function terminates immediately.
  2. Because no library is linked to modules, source files should never include the usual
header files, \<stdarg.h\> and very special situations being the only exceptions. Only
functions that are actually part of the kernel itself may be used in kernel modules
