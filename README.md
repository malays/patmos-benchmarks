patmos-benchmarks
=================

A collection of benchmarks and tests for the Patmos processor and compiler.

1. Requirements

 - LLVM toolchain for Patmos (or either Sparc or PowerPc)
   https://github.com/t-crest/patmos-llvm
   https://github.com/t-crest/patmos-clang
   https://github.com/t-crest/patmos-compiler-rt
   https://github.com/t-crest/patmos-newlib
   https://github.com/t-crest/patmos-gold
   http://www.llvm.org/

 - Absint a3 tools (optional)
   http://www.absint.com/a3/index.htm

2. Configure and build

  mkdir build
  cd build
  cmake .. -DCMAKE_TOOLCHAIN_FILE=../cmake/patmos-clang-toolchain.cmake -DENABLE_TESTING=true
  make

For a list of pre-defined compiler/processor toolchain configurations see the
cmake directory (currently leon3-clang, mpc5554-cland, patmos-clang). To chose
one of them use:

  cmake .. -DCMAKE_TOOLCHAIN_FILE=../cmake/<processor>-clang-toolchain.cmake


Additional search paths can be provided using the -DCMAKE_PROGRAM_PATH=<path>
option.

Have fun!