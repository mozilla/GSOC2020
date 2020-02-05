# Speed-up rav1e WASM target

**Mentor:** Nathan Egge

**Email:** negge@mozilla.com

## Project Description

Implement [wasm-simd](https://doc.rust-lang.org/core/arch/wasm32/index.html) support in rav1e.
Rav1e is an AV1 encoder that is fast enough to be used in videoconference scenarios on x86_64, we'll leverage the webassembly SIMD support to make so it would be viable as in-browser encoder.

## Skills Required

An applicant needs:

* rust knowledge
* webassembly knowledge
* possibly knowledge of x86_64 simd or Aarch64 simd extensions
* possibly javascript knowledge

## Project Details

Rav1e is currently getting basic wasm32-wasi support for its release 0.3.0, the student task will require him to build upon it and improve its performance.

### Milestones
- Setup a system to profile and benchmark the wasm port.
- SIMD-fy the top 5 functions and produce a report for each.
- Keep optimizing further the next 10.
- **Bonus** prepare a simple encode in-browser demo.

