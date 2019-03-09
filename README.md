# idris-bare-metal-manifest
Manifest for bare-metal apps written in Idris running on ARM

## Get the Code!
Run the following commands to get the code:

```
mkdir idris-bare-metal-manifest
cd idris-bare-metal-manifest
repo init -u https://github.com/mokshasoft/idris-bare-metal-manifest.git
repo sync
```

## Build it
To build:


```
mkdir build
cd build
cmake -G Ninja -DCMAKE_TOOLCHAIN_FILE=../core/cmake/gcc-toolchain.cmake ..
ninja hello-world
```

## QEMU
To run the simulation in QEMU:

```
ninja qemu.hello-world
```
