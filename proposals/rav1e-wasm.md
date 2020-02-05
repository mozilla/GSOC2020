# Performance improvements to rav1e WASM target

**Mentor:** Nathan Egge

**Email:** negge@mozilla.com

## Project Description

Implement [wasm-simd](https://doc.rust-lang.org/core/arch/wasm32/index.html) support in rav1e.
Rav1e is an AV1 encoder that is fast enough to be used in videoconference scenarios on x86_64, we'll leverage the webassembly SIMD support to make so it would be viable as in-browser encoder.

## Skills Required

An applicant needs:

* Rust knowledge
* WebAssembly knowledge
* x86_64 or Aarch64 SIMD extensions
* JavaScript knowledge (preferred)

## Project Details

Rav1e is currently getting basic wasm32-wasi support for its release 0.3.0.  The student task will require him to build upon it and improve its performance by adding WASM-SIMD and potential other WASM speed-ups like better threading, improved memory usage, etc.

### Milestones
- Setup a system to profile and benchmark the WASM port.
- SIMD-fy the top 5 functions and produce a report for each.
- Keep optimizing further the next 10.
- **Bonus** prepare a simple encode in-browser demo.
