# recompiler_backends

LLVM alone's ends of `tests/recompiler_backends.c`'s programs, which the native back ends are held to (`--frozen`): a
hash a function over its states and data memory, in `tests/support/frozen.h`'s format. Each file's args line is the
generator's options that draw its programs, and a test reads the file of its options.

Recorded by `tests/recompiler_backends_record.py BUILD --out <this folder>` in a build that had LLVM, which the
recompiler no longer has: another file needs another reference.
