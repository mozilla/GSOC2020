# CSS unit conversion in DevTools

**Mentor:** Razvan Caliman

**Email:** rcaliman@mozilla.com

## Project Description

Web designers and developers can choose between many color formats and CSS unit types, both fixed (`px`) and relative (`%`, `em`, `vh`, etc). Starting off with the wrong one usually means a process of manual conversion later on. This is time consuming and not fun.

The goal of this project is to add new capabilities to the CSS Rules panel in Firefox DevTools to convert formats and CSS unit types on-demand.

**UI mock-up:**

![Unit conversion in Rules panel](https://user-images.githubusercontent.com/63899/73087522-eb4d7e00-3ed2-11ea-959e-17d960553386.png)

## Skills Required

* Good grasp of JavaScript and CSS
* Ability to communicate ideas clearly and concisely in English
* Familiarity with a version control system such as Git or Mercurial
* Comfortable with having your code reviewed by others and a genuine willingness to learn

## Project Details

Firefox DevTools already implements some bits for doing conversion.

In the CSS Rules panel, you can cycle between color formats by holding down the Shift key and clicking on the color preview icon next to a color value. It works, but it's not discoverable. In the Fonts panel, there is a dropdown to convert between CSS unit types. It works, but it's limited to only a few font properties.

Tools are most helpful when they're obvious and available in the context where they're needed.

Adding a new UI component next to values to do conversion in the CSS Rules panel will make it obvious that this functionality exists.

Roughly divided, the project would happen in 3 phases:

**Phase 1**:
Expose existing [color format conversion](https://searchfox.org/mozilla-central/rev/f98dad153b59a985efd4505912588d4651033395/devtools/client/shared/output-parser.js#1570-1599) to a new UI in CSS Rules panel

**Phase 2**:
Research and implement approach to do CSS unit conversion for a subset of properties, values and types. Reuse and expand the [unit conversion logic](https://searchfox.org/mozilla-central/rev/f98dad153b59a985efd4505912588d4651033395/devtools/client/inspector/fonts/fonts.js#173-297) from the Fonts panel.

**Phase 3**:
Refine feature, expand list of supported properties, values and unit types

## Additional Information

* Work will need to be submitted for code review on [Mozilla’s Phabricator](https://wiki.mozilla.org/Phabricator) instance.

* Communication will happen through the [Firefox DevTools’ Slack](https://devtools-html-slack.herokuapp.com/).
