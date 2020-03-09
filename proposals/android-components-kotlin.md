# Android Components - Kotlin/Native, Kotlin/JS, Jetpack Compose

**Mentor**: Sebastian Kaspari

**Email:**: skaspari@mozilla.com

**Chat** (_Matrix_): _Android Components_ room on chat.mozilla.org.

## Project Description

The [Android Components project](https://github.com/mozilla-mobile/android-components) creates reusable components to build browsers or browser-like applications. Those components are Android libraries written in Kotlin and are used by mobile apps like [Firefox Preview](https://play.google.com/store/apps/details?id=org.mozilla.fenix&hl=en) and [Firefox Lockwise](https://play.google.com/store/apps/details?id=mozilla.lockbox&hl=en) (See KotlinConf talk [Build a Browser by Kotlin](https://www.youtube.com/watch?v=JKNSrBxqSs4)).

The goal of this _Google Summer of Code_ project is it to build prototype components in order to evaluate and experiment with new Kotlin and Android technologies or frameworks like [Kotlin/Native](https://kotlinlang.org/docs/reference/native-overview.html), [Kotlin/JS](https://kotlinlang.org/docs/reference/js-overview.html) and [Jetpack Compose](https://developer.android.com/jetpack/compose).

## Skills Required

* Proficient knowledge of [Kotlin](https://kotlinlang.org/)

* Experience developing [Android applications and/or libraries](https://developer.android.com/)

* (Optional) Experience developing iOS applications

## Project Details

The goal of this "Google Summer of Code" project is to create one or multiple prototype components making use of one or multiple of the frameworks mentioned below (scope and size to be defined by the student) and to include those components into a build of our [Reference Browser](https://github.com/mozilla-mobile/reference-browser) for testing purposes.

### Kotlin/Native

[Kotlin/Native](https://kotlinlang.org/docs/reference/native-overview.html) is a technology for compiling Kotlin code to native binaries that can be used on many platforms (like _iOS, macOS, Windows, Linux, Android_).

For evaluating _Kotlin/Native_, pick (or adapt) an existing Android component to be compiled to a native binary. Then use this native binary from an Android application (like [Reference Browser](https://github.com/mozilla-mobile/reference-browser)) and an iOS application (like [Firefox for iOS](https://github.com/mozilla-mobile/firefox-ios)).

### Kotlin/JS

[Kotlin/JS](https://kotlinlang.org/docs/reference/js-overview.html) allows it to transpile Kotlin code into JavaScript.

Some of our Android components (like [feature-readerview](https://github.com/mozilla-mobile/android-components/tree/master/components/feature/readerview)) come with a [WebExtension](https://developer.mozilla.org/en-US/docs/Mozilla/Add-ons/WebExtensions) that is implemented in JavaScript. With the help of the _WebExtension_ Kotlin code can interact with web content by passing messages between Kotlin and JavaScript.

For evaluating _Kotlin/JS_, pick (or adapt) an existing Android component that uses JavaScript and try to replace the JavaScript code with Kotlin code that gets compiled into JavaScript at build time. Then integrate this component into a [Reference Browser](https://github.com/mozilla-mobile/reference-browser) build.

### Jetpack Compose

[Jetpack Compose](https://developer.android.com/jetpack/compose) is a modern and new toolkit for building Android UI, that is currently in development.

To evaluate _Jetpack Compose_ and compare it to the existing Android _View_ system, reimplement (simplified) a UI-focused component (like [browser-toolbar](https://github.com/mozilla-mobile/android-components/tree/master/components/browser/toolbar)). Then integrate this component into a [Reference Browser](https://github.com/mozilla-mobile/reference-browser) build.
