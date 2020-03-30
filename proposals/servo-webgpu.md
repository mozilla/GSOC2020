# Bring Servo WebGPU to fruition

### Mentor: Dzmitry Malyshau 
### Email: dmalyshau@mozilla.com 

## Project Description 

There is a an initial implementation of WebGPU in Servo.
This GSoC proposal is for improving this to a point where basic examples can be ran, and a fair portion of the conformance test suite is covered.

## Skills Required

An applicant needs:

* good understanding of at least one of the graphics APIs, and will to learn more (WebGPU)
* will to learn or experience working with Rust language
* ability to navigate large code bases and communicate with relevant teams remotely

Prior experience working with Servo or wgpu-rs is a plus.

## Project Details

[WebGPU](https://gpuweb.github.io/gpuweb/) is an emerging API or the Web that efficiently exposes graphics and compute capabilities. It's not based on an existing native API but is inspired by, and targeting Vulkan, D3D12, and Metal.

[Servo](https://github.com/servo/servo/) is an experimental browser engine written in [Rust](https://www.rust-lang.org/) language. It was an early home for [Stylo](https://hacks.mozilla.org/2017/08/inside-a-super-fast-css-engine-quantum-css-aka-stylo/) and [WebRender](https://hacks.mozilla.org/2017/10/the-whole-web-at-maximum-fps-how-webrender-gets-rid-of-jank/), which are now parts of Firefox. Servo is currently used to experiment with VR/AR applications, where latency, power consumption, and performance requirements are extremely tight. Therefore, implementing WebGPU in Servo opens the doors for more immersive experience in VR and AR.

Basic implementation in Servo was delivered by the [Szeged team](https://github.com/szeged/). Meta issue for tracking the state - https://github.com/servo/servo/issues/24706. The implementation is based on [wgpu-core](https://github.com/gfx-rs/wgpu), which is also written in Rust.

Roughly, these are the steps of accomplishing the task:
  1. (~1 week) learning about WebGPU, Servo constellation, and wgpu-core API. Identifying the areas in need of improvement.
  2. (~3 weeks) implementing the missing functionality according to the [meta-issue](https://github.com/servo/servo/issues/24706).
  3. (~4 weeks) working through the [Conformance Test Suite](https://github.com/gpuweb/cts) and unlocking the tests in Servo.
  4. (~2 weeks) profiling and benchmarking against the current WebGL implementation on similar workloads.
  5. (~2 weeks) writing notes about the progress and issues.

Minimal expectation: Servo is able to run [Austin's samples](https://austineng.github.io/webgpu-samples/) on at least one graphics backend.

## Additional Information

Logistically, the student would make changes in pull requests to Servo, gfx-rs repositories, and potentially some of their dependencies. They would communicate on [Matrix](https://matrix.to/#/#gfx:matrix.org) to ask questions and get feedback.
