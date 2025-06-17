MicroPython 32-bit Unix PowerPC port
=====================
Currently only a minimal variant is possible.

## Minimal PowerPC
```
# apt install build-essential git python3 pkg-config libffi-dev gcc-powerpc-linux-gnu
```
starting from the top-level MicroPython directory:

    $ cd ports/unix-ppc32
    $ make submodules
    $ make VARIANT=minimal CROSS_COMPILE=powerpc-linux-gnu-

it compiled but right now it cant find ld.s . with qemu-ppc. leaving this for future me