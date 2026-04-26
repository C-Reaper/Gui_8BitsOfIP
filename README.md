# Project README

## Overview
This project is a C application that processes images using various image processing algorithms. The application is designed to run on different platforms including Linux, Windows, and the web.

## Features
- **Image Processing Algorithms:** Supports a variety of image processing techniques such as filters, transformations, and effects.
- **Cross-Platform Support:** Can be built and executed on Linux, Windows, and through WebAssembly in the browser.
- **User Interface:** Provides a simple interface to interact with the application using keyboard inputs.

## Project Structure
- `build/`: Contains the executable files produced by compiling the source code.
- `src/`: Contains the source code for the project.
  - `Main.c`: The entry point of the application.
  - Various `.h` files: Standalone header-based C-files without corresponding `.c` files that implement them.

## Prerequisites
- **C/C++ Compiler and Debugger:** GCC, Clang (Linux), x86_64-w64-mingw32-gcc (Windows).
- **Make utility:** For building the project.
- **Standard Development Tools:** Required for compiling and linking the source code.
- **Libraries needed in specific projects:**
  - Linux: `X11`, `png`, `jpeg`.
  - Windows: `user32`, `gdi32`, `winmm`.
  - WebAssembly: None.

## Build & Run
### Building on Linux
```sh
cd <Project>
make -f Makefile.linux all
```
To execute the application:
```sh
make -f Makefile.linux exe
```

### Building on Windows
```sh
cd <Project>
make -f Makefile.windows all
```
To execute the application:
```sh
make -f Makefile.windows exe
```

### Building for WebAssembly
```sh
cd <Project>
make -f Makefile.web all
```
To run the application in a web browser:
```sh
make -f Makefile.web exe
```