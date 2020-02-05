# Performance improvements to rav1e WASM target

**Mentor:** Nathan Egge

**Email:** negge@mozilla.com

## Project Description

Rav1e is an AV1 encoder that is fast enough to be used in videoconference scenarios on x86_64.
This project will implement [wasm-simd](https://doc.rust-lang.org/core/arch/wasm32/index.html) support in rav1e to make viable as in-browser encoder.

## Skills Required

An applicant needs:

* Rust knowledge
* WebAssembly knowledge
* x86_64 or Aarch64 SIMD extensions
* JavaScript knowledge (preferred)

## Project Details

[Rav1e](https://github.com/xiph/rav1e) is currently getting basic wasm32-wasi support as part of the 0.3.0 release.  The student task will build upon this and improve performance by adding WASM-SIMD and other potential WASM speed-ups like multi-threading, improved memory usage, etc.

### Milestones
- Setup a system to profile and benchmark the WASM port.
- SIMD-fy the top 5 functions and produce a report for each.
- Keep optimizing further the next 10.
- **BONUS** prepare a simple encode in-browser demo.
