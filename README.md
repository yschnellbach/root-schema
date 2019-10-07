# root-skeleton
Super-basic structure for compiling some code using ROOT libraries

## Usage
This is a simple CMake skeleton for code linked against ROOT (also built with CMake) and a very simple library. It should a jumping off point for implementing your own code as this does nothing.

## Things to consider
When using this, there are a few things and default assumptions to consider and tweak in the `CMakeLists.txt`:
- It assumes you're using `.cxx` as file extension, it can be changed in line 31 and 36
- It assumes you want to compile every source file in the `/src` directory, if not, delete line 31 and replace `${LIBRARY_SOURCES}` in the line below with the explicit files
- Optimisation flag is set to `-O2` in line 8
