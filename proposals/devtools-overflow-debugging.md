# Debugging unwanted scrollbars in DevTools

**Mentors:** Brad Werth

**Emails:** bwerth@mozilla.com

## Project Description

It is very common for unwanted scrollbars to appear in webpages when working on complex CSS layouts. Investigating where they come from and why isn't easy though. The goal of this project is to add features to Firefox Developer Tools that solve this common CSS challenge.

## Skills Required

- Experience with JavaScript and C++ and willingness to learn.

- Ability to navigate large code bases and communicate with relevant teams remotely.

- Experience using browser developer tool

## Project Details

An important goal for Firefox Developer Tools is creating CSS layout-related tools for web authors.
Challenges people tend to face with CSS are often very specific, hence we need very focused tools for these challenges.

Firefox has innovated in the past with focused tools that help with [grid](https://developer.mozilla.org/en-US/docs/Tools/Page_Inspector/How_to/Examine_grid_layouts), [flexbox](https://developer.mozilla.org/en-US/docs/Tools/Page_Inspector/How_to/Examine_Flexbox_layouts), [fonts](https://developer.mozilla.org/en-US/docs/Tools/Page_Inspector/How_to/Edit_fonts) and more.

There are many other specific features of CSS that, although very useful and powerful, can easily cause problems that are hard to prevent and debug.

The way content can overflow in a web page is one such CSS feature. Its behavior depends on many things such as the length of content, the type of containers involved, the various box model values, etc.

Firefox Developer Tools added a useful feature to the [Inspector panel](https://developer.mozilla.org/en-US/docs/Tools/Page_Inspector) already that makes it easy to find elements that do overflow.
The goal of this project is to go much further and provide users with a way to easily detect exactly _what_ caused the overflow to happen in the first place, and therefore a scrollbar to become visible.

This will require exposing a new simple internal Gecko API and then make use of it in DevTools to find the elements causing the overflow, and list them in the Inspector panel UI.

This project will give you the opportunity to understand both the Firefox platform (written in both C++ and Rust) and user interface (written in HTML, CSS and JavaScript).

The steps to complete the project are roughly outlined below:

- **Phase 1 (May 18 - June 15)**: Implement the new Gecko API that lists element nodes that cause a given element to overflow.

- **Phase 2 (June 15 - August 1)**: Implement the basic UI in DevTools for displaying this list of elementsd.

- **Phase 3 (August 1 - ~August 17)**: Stabilize and refine the feature. Polish the UI, and perhaps add telemetry to track usage of the feature.

## Additional Information

- Student will be submitting their work for code review on [Mozilla’s Phabricator](https://wiki.mozilla.org/Phabricator) instance.

- Communication will be through the [Firefox DevTools’ Slack](https://devtools-html-slack.herokuapp.com/).
