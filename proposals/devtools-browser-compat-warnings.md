# Inline browser compatibility warnings for CSS properties in DevTools

**Mentor:** Micah Tigley & Daisuke Akatsuka

**Email:** mtigley@mozilla.com & dakatsuka.birchill@mozilla.com

## Project Description

The layout tools team at Firefox Developer Tools aims to provide users with first-class CSS debugging tools. This also means providing a simple way for users to identify problems with their CSS due to browser compatibility issues. This project will use and extend existing APIs in DevTools to integrate important browser compatibility information for users when debugging code in the CSS Rules panel.

## Skills Required

* Proficient knowledge of JavaScript, HTML, CSS
* Ability to effectively communicate with relevant teams in a remote environment, especially when navigating large codebases.
* Experience using browser developer tools

## Project Details

There is already a feature in DevTools that identifies browser compatibility issues for CSS properties. It’s available in the Compatibility panel of the Inspector. The plan for this project is to make the [existing library for getting web compatibility](https://searchfox.org/mozilla-central/source/devtools/client/inspector/compatibility/lib/MDNCompatibility.js) issues to be a shared module and have the CSS Rules panel consume this information.

The steps to complete the project are roughly outlined below:
* Phase 1 (May 18 - June 19)
    * (~1 week) Migrate library for getting web compatibility issues to a shared place in DevTools
    * (~3 weeks) Connect MDN Compatibility library to the CSS Rules panel.
* Phase 2 (June 19 - July 17)
    * (~4 weeks) Implement basic UI for displaying web compatibility information in the CSS Rules panel.
* Phase 3 (July 17 - ~August 17)
    * (~4 weeks) Stabilize and refine feature. Adding telemetry to track usage for feature.
    
### UI mock-up
![browser_compat_tooltip](https://user-images.githubusercontent.com/14285585/75567604-cd1df500-5a1f-11ea-887f-aa4a54d84257.png)

## Additional Information
* Student will be submitting their work for code review on [Mozilla’s Phabricator](https://wiki.mozilla.org/Phabricator) instance.
* Communication will be through the [Firefox DevTools’ Slack](https://devtools-html-slack.herokuapp.com/).
