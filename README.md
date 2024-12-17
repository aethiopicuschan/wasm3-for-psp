# Wasm3 for PSP

Original project: [wasm3/wasm3](https://github.com/wasm3/wasm3)

I, [Chan Aethiopicus](https://github.com/aethiopicuschan), have made the following changes.

- Simplified the README
- Made additions to `CMakeLists.txt`
- Added `psp-toolchain.cmake`
- Remove `publish` workflow

### How to build

```sh
mkdir build
cd build
cmake .. -DCMAKE_TOOLCHAIN_FILE=../psp-toolchain.cmake -DBUILD_SHARED_LIBS=OFF -DBUILD_WASI=none -DCMAKE_INSTALL_PREFIX=~/wasm3
make
make install
```

### License

This project is released under The MIT License (MIT)
