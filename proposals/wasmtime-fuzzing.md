# Fuzzing the Wasmtime WebAssembly runtime

**Mentor:** Nick Fitzgerald and Deian Stefan

**Email:** fitzgen@mozilla.com, deian@cs.ucsd.edu

## Project Description

Fuzz test the Wasmtime runtime to find security bugs.

## Skills Required

* Programming in Rust
* Familiarity with fuzzing, libFuzzer in particular
* Some familiarity with WebAssembly and/or Cranelift (or willing to learn)

## Project Details

The goal of this project is to extend the existing [Wasmtime fuzzing infrastructure](https://bytecodealliance.github.io/wasmtime/contributing-fuzzing.html) to find potential security bugs in Wasm binaries.  In particular, the student will be writing new _oracles_ that will check the safety of a Wasm binary and _test generators_ that will generate Wasm modules to exercise code paths that could potentially affect safety.

The exact safety properties to check will be determined in collaboration with the mentors, but will most likely include: trampoline/ABI safety (e.g., ensure that callee-saved registered are not clobbered), stack safety (e.g., ensure that a function can only modify values local to its frame), heap safety (e.g., ensure that all memory accesses are within the Wasm sandbox), and control-flow integrity (i.e., ensure that indirect calls can only call valid functions).  The goal is to find Wasm programs that pass Wasm validation but fail any of these safety checks.

The student will build on a research prototype that implements a subset of these safety checks. Indeed, initially the student can use this validator as a black-box as part of an oracle.  

## Additional Information

- [Existing oracles](https://github.com/bytecodealliance/wasmtime/blob/master/crates/fuzzing/src/oracles.rs)
- [Existing test generators](https://github.com/bytecodealliance/wasmtime/blob/master/crates/fuzzing/src/generators.rs)
