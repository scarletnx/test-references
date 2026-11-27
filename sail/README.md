# sail

LLVM's ends of the words `tests/sail_x64.c` and `tests/sail_mach.c` hold to them rather than to QEMU (`--frozen`): the
words QEMU can't stand for (pointer authentication's, which QEMU signs with keys of its own where the code runs with
authentication off, and those its max CPU decodes as another op), and STXR and STXP of doublewords with the monitor
armed where the memory changed, which no QEMU case starts from. A hash a word over its 64 states
(`tests/sail_qemu.h`), in `tests/support/frozen.h`'s format.

Recorded by `snx-test-sail-frozen --record frozen.txt` (`tests/sail_frozen.c`) in a build that had LLVM, which the
recompiler no longer has: another file needs another reference.
