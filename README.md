# root-skeleton
Super-basic structure for compiling some code using ROOT libraries

## Usage
This is a simple CMake skeleton for code linked against ROOT (also built with CMake) and a very simple library. It should a jumping off point for implementing your own code as this does nothing.

## Things to Know
When using this, there are a few things and default assumptions to consider and tweak in the `CMakeLists.txt`:
- When you setup the project, it uses the `$CLICOLOR_FORCE` environment variable to force compilers to emit coloured output (useful for some build systems like *ninja*)
- It assumes you're using `.cxx` as file extension, it can be changed in line 31 and 36
- It assumes you want to compile every source file in the `/src` directory, if not, delete line 31 and replace `${LIBRARY_SOURCES}` in the line below with the explicit files (that's a safer approach but less convenient)
- Optimisation flag is set to `-O2` in line 8, so consider the usual caveats that come with optimisation flags and tune to your liking
