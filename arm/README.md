# arm

LLVM's results at -O0 for the AArch32 blocks of `tests/arm_x64.c` and its machines' programs (`--frozen`): a hash a
block over its states, and the units it consumed, in `tests/support/frozen.h`'s format. Each file's args line draws its
blocks; the `call_abi*` files were made with the test's runtime callbacks (`--callee`), as the call_abi tests run.

Recorded by `tests/arm_frozen.py record PROGRAM --out <this folder>` in a build that had LLVM, which the recompiler no
longer has: another file needs another reference.
