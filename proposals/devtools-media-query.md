# Media Query Visualizer in DevTools

**Mentor:** Brad Werth

**Email:** bwerth@mozilla.com

## Project Description

Firefox’s [Responsive Design Mode](https://developer.mozilla.org/en-US/docs/Tools/Responsive_Design_Mode) provides a way to simulate the appearance and behavior of a website on a device different from the development device.

Many sites use [media queries](https://developer.mozilla.org/en-US/docs/Web/CSS/Media_Queries/Using_media_queries) in CSS to change their styling based on the size of the device rendering them.

This project would add a visualization of the media queries’ size ranges so that developers can quickly confirm which media queries are active and which are not.

## Skills Required

- JavaScript,

- good understanding of CSS media queries,

- experience with React may be helpful.

## Project Details

The goal of this project is to add a toggle-able visualizer to the existing DevTools Responsive Design Mode (aka RDM) tool.
RDM already includes several affordances for changing the device size, the DPI, the user agent string, touch event support, and support for resolution zooming (meta viewport tags).

This project would add one more such feature.

The DevTools already extracts details about media queries and summarizes them in the [Style Editor](https://developer.mozilla.org/en-US/docs/Tools/Style_Editor#The_media_sidebar). This would be an alternative presentation of the existing data.

Here’s a breakdown of the project steps in order we anticipate them being done:

- Add a toggle-able widget to the RDM UI for the new visualizer.

- When turned on, the new visualizer appears above the RDM content area and contains one horizontal band for each media query that checks device width.

- Add text labels to the bands at the extents to show the precise breakpoints.

- Make the bands color-coded based on whether or not they are active.

- Tooltips on the bands show the text of the associated media query.

- Clicking on the band focuses other DevTools tools on the relevant CSS that specifies the associated media query.

- The bug tracking this feature is [Bug 1031585](https://bugzilla.mozilla.org/show_bug.cgi?id=1031585), and there is some documented [discussion of a media query visualizer with users](https://discourse.mozilla.org/t/show-media-queries-in-responsive-design-view/50187).

## Additional Information

- Student will be submitting their work for code review on [Mozilla’s Phabricator](https://wiki.mozilla.org/Phabricator) instance.

- Communication will be through the [Firefox DevTools’ Slack](https://devtools-html-slack.herokuapp.com/).
