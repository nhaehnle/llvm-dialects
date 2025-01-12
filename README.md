llvm-dialects
=============

Dummy change to test GitHub features.

Overview
========
The LLVM Dialects library allows defining "dialects" on top of the LLVM IR
"substrate" in a TableGen-based DSL that looks, on purpose, very much like the
DSL used to define MLIR dialects.

Its main user is [LLPC](https://github.com/GPUOpen-Drivers/llpc). We welcome
other interested parties. Development of llvm-dialects happens on GitHub,
using Issues and Pull Requests.

LLVM Compatibility
==================
The `main` branch is generally expected to work with (a recent version of) the
`main` branch of the llvm-project repository. No promises are made about
compatibility with any specific LLVM version.

Components
==========

- lib/Dialect: a helper library that allows the creation of basic dialects (in
  the MLIR sense) for LLVM IR
- lib/TableGen: common code for interpreting TableGen records that define a
  dialect
- utils/llvm-dialects-tblgen: a standalone CLI tool which reads a .td dialect
  definition and outputs C++ header and source files
