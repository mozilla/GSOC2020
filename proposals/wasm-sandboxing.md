# Sandboxing libraries in Firefox with Wasm

**Mentor:** Deian Stefan, Eric Rahm, and Nathan Froyd

**Email:** deian@cs.ucsd.edu, erahm@mozilla.com, nfroyd@mozilla.com

## Project Description

Sandbox libraries using WebAssembly to reduce Firefox's attack surface.

## Skills Required

* Programming in C++ (and willing to learn C++17 if necessary)
* Programming in C
* Some familiarity with WebAssembly
* Some familiarity building Firefox

## Project Details

The goal of this project is to sandbox libraries in Firefox using WebAssembly.  This is part of our [new effort](https://hacks.mozilla.org/2020/02/securing-firefox-with-webassembly/) to ensure that bugs in libraries cannot be exploited to compromise the browser.

The student will be using the [RLBox toolkit](https://docs.rlbox.dev) to sandbox libraries in Firefox. To date, we used RLBox to sandbox the [graphite library](https://bugzilla.mozilla.org/show_bug.cgi?id=1566288) and are working on [sandboxing more libraries](https://bugzilla.mozilla.org/show_bug.cgi?id=1572616).  The exact libraries the student will be sandboxing will depend on the student's interest and experience, and will be determined in collaboration with the mentor(s), but most likely some of the libraries listed [here](https://bugzilla.mozilla.org/show_bug.cgi?id=1572616#c1).

## Additional Information

The [blog post](https://hacks.mozilla.org/2020/02/securing-firefox-with-webassembly/) and [academic paper](https://arxiv.org/abs/2003.00572) describing the sandboxing effort are useful to read before starting the project.
