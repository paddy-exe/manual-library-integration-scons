# Manual library integration with scons
This project is an example on how libraries built with cmake build-system could be manually integrated into a C++ program built using the scons build-system. It is part of a blog post of mine explaining how to use the scons build-system either manually with cmake built libraries and package managers such as vcpkg and conan.

## Build requirements
- Python
- SCons
- CMake
- C++ compiler

## Build instructions
1. Enter the `sumlib` directory
```sh
cd sumlib
```

2. Install cmake
```sh
cmake .
```

3. Build the library with cmake
```sh
cmake --build .
```

4. Go back to the root directory
```sh
cd ..
```

5. Build the program with scons
```sh
scons
```

6. Run program (This may differ slightly on Windows)
```sh
./helloworld
```
