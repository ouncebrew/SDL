# Ounce fork:
Build:
source $DEVKITPRO/switch2vars.sh
unset CFLAGS CXXFLAGS LDFLAGS
aarch64-none-elf-cmake -G Ninja -S . -B build-switch2-shared -DOUNCE_SHARED=ON -DCMAKE_DISABLE_PRECOMPILE_HEADERS=ON -DSDL_TESTS=OFF -DSDL_SHARED=ON
cmake --build build-switch2-shared -j8

# Original readme
Simple DirectMedia Layer (SDL for short) is a cross-platform library
designed to make it easy to write multi-media software, such as games
and emulators.

You can find the latest release and additional information at:
https://www.libsdl.org/

Installation instructions and a quick introduction is available in
[INSTALL.md](INSTALL.md)

This library is distributed under the terms of the zlib license,
available in [LICENSE.txt](LICENSE.txt).

Enjoy!

Sam Lantinga (slouken@libsdl.org)
