# Chapter 11

## Overview

This directory is dedicated to implementing features that rely on the
`C11 Annex K` Bounds-Checking Interfaces. However, their support is limited in
compilers like `gcc` and `clang`. To address this, we utilize the [safeclib
library][safeclib], which provides an implementation of these interfaces.

## safeclib library

### Manual Installation

Refer to the [safeclib repository][safeclib] for detailed installation
instructions.

### Installation script

For convenience, use our script [install-safeclib.sh](./install-safeclib.sh) for
automated installation. This script is ideal for demonstration and quick setup
purposes.

The installation of `safeclib` can be facilitated using the provided script
[install-safeclib.sh](./install-safeclib.sh). This script is intended for
demonstration purposes. Users may prefer to manually install the library by
following the instructions in the [safeclib GitHub repository][safeclib].

Ensure the following tools are installed:

- libtool
- autoconf
- automake

To use the installation script, execute the following commands:

```sh
sudo ./install-safeclib.sh
```

## Build and Run

To build a program, link the `safeclib` library.

For example:

```sh
cc -o my_program source.c -lsafec
./my_program
```

[safeclib]: https://github.com/rurban/safeclib
