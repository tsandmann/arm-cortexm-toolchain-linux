# arm-cortexm-toolchain-linux
A cross-compiler toolchain for Linux (built on CentOS 8) host and arm-none-eabi targets optimized for cortex-m4f and cortex-m7f.

#### Installation
Checkout somewhere (e.g. to `/usr/local/arm-none-eabi`) and add the `bin` folder of that path (e.g `/usr/local/arm-none-eabi/bin`) to *PATH*.

#### Components and Versions
* gcc 10.2.0, newlib 3.3, binutils 2.35, gdb 9.2 (built with crosstool-ng)
  * newlib is built with nano malloc
  * newlib is available in two versions:
    1. with standard printf (*libc.a*)
    1. with nano formatted io printf (*libc_nano.a*), select with `--specs=nano.specs`
