static functions in C: just limits the usage of the function within that file.
there exists a src.c file in which the functions can be referenced from.
and if it has the 'static' prefix in the declaration. it means that it can ONLY be used within that file, even if it is being referred to from another file, it will return an error as the static function is only available to that file.

compiler directives / linker section attributes: '__init' and '__exit'. this just tells the kernel specific things to "link" it with while doing the linking stage of the overall compilation.

1. __init: this macro tells the kernel to get rid of this block of code from memory after it has been executed.
2. __exit: this macro tells the kernel to run this block of codw when "rmmod" or modprobe-r.

Dictates where in RAM that address is stored (and when it can be deleted).


