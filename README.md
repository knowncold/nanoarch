# nanoarch

nanoarch is a small libretro frontend (nanoarch.c has less than 1000 lines of
code) created for educational purposes. It only provides the required (video,
audio and basic input) features to run most non-libretro-gl cores and there's
no UI or configuration support.

## Building

Other than `make`, `pkg-config` and a working C99 or C++ compiler, you'll need
`alsa` and `glfw` development files installed.

需要安装`-dev`的包

	export PKG_CONFIG_PATH=/lib/x86_64-linux-gnu/pkgconfig/glu.pc:/usr/lib64/pkgconfig:/usr/share/pkgconfig


## Running

    ./nanoarch <core> <uncompressed content>

	./nanoarch ./libretro.so test.nes
