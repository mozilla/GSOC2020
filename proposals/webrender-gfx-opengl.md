# OpenGL ES 3.0 backend for WebRender on gfx-rs

### Mentor: Dzmitry Malyshau 
### Email: dmalyshau@mozilla.com 

## Project Description 

Make the experimental WebRender fork by Szeged (that uses gfx-rs for rendering) to run on devices that only support OpenGL ES 3.0, so that the current GL-only code path could be considered for removal in the future.

## Skills Required

An applicant needs:

* good understanding of OpenGL and general principles behind Vulkan
* will to learn or experience working with Rust language
* ability to discover, investigate and fix graphics issues independently, while constantly communicating the progress and requesting feedback

Prior experience working with gfx-rs and/or WebRender is a plus.

## Project Details

We want to move WebRender to a [foundation](https://github.com/gfx-rs/gfx/) that natively supports Vulkan, D3D12, and Metal with low overhead. However, there are still devices on the market that can only support OpenGL ES, e.g. many Android phones, Windows 7, some Linux, etc. We want to have WebRender running on [gfx-backend-gl](https://crates.io/crates/gfx-backend-gl) on those devices, with good efficiency, in order to properly deprecate the current GL-only code path.

Roughly, these are the steps of accomplishing the task:
  1. (~1 week) enabling OpenGL code path for [Szeged's fork of WebRender](https://github.com/szeged/webrender)
  2. (~3 weeks) addressing conceptual compatibility issues (e.g. https://github.com/gfx-rs/gfx/issues/2784) with the GL backend
  3. (~4 weeks) reaching the reftest parity with the [current GL](https://github.com/servo/webrender/) implementation of WebRender
  4. (~2 weeks) profiling and benchmarking against the current GL implementation
  5. (~2 weeks) writing notes about the progress and issues

Minimal expectation: WebRender on `gfx-backend-gl` passes the Wrench tests on OsMesa driver.

## Additional Information

Logistically, the student would make changes in pull requests to the Szeged WR fork, gfx-rs repositories, and potentially some of their dependencies. They would communicate on [Matrix](https://matrix.to/#/#gfx:matrix.org) to ask questions and get feedback, coordinating work with me as well as the Szeged team.
