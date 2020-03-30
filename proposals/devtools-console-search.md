# DevTools WebConsole search

**Mentor:** Nicolas Chevobbe, Jan Odvarko, Jason Laster

**Email:** nchevobbe@mozilla.com, honza@mozilla.com, jlaster@mozilla.com


## Project Description

Add a new search functionality to the Firefox DevTools WebConsole, 
where the matching part of messages would be highlighted, 
and that would allow the user to cycle through the different results, 
in a similar way to how Firefox "Search in page" works.

## Skills Required

Applicants needs:

* Good HTML, CSS and Javascript skills
* React and Redux knowledge would be a plus, but not required
* be able to communicate clearly, as most of the interaction with the mentor / members of the team will be asynchronous
* not be afraid of asking questions, in order to not stay blocked on something

## Project Details

In Firefox DevTools WebConsole, you can currently filter the output with a given string.
When you do so, only the messages matching said string are displayed in the console output.
But it might happen that a user want to still see the context of a given message (what are
the messages that were emitted before and/or after a given value for example).

This project would add a new Search functionality to the WebConsole, where the matching part of messages
would be highlighted, and that would allow the user to cycle through the different results (similar to how
Firefox "Search in page" feature works).

You can check [Bug 992594](https://bugzilla.mozilla.org/show_bug.cgi?id=992594) to get more information about this.

A stretch goal would be to also search into the first level of objects logged in the output.
