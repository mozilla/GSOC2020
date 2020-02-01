# Server Sent Events Inspector

**Mentor:** Jan Honza Odvarko

**Email:** honza@mozilla.com


## Project Description

Traditionally, a web page has to send a request to the server to receive new data; that is, the page requests data from the server. With server-sent events, it's possible for a server to send new data to a web page at any time, by pushing messages to the web page. These incoming messages can be treated as Events + data inside the web page.

This project is about building an inspector intercepting and visualizing server-sent event traffic so, the developer can easily see what exact data are received from the server and when.

## Skills Required

* Experience with Javascript/HTML/CSS required
* Experience with React/Redux is advantage
* Clear English communication
* Enjoy open source environment

## Project Details

The Network panel is already supporting [WebSocket inspection](https://hacks.mozilla.org/2019/10/firefoxs-new-websocket-inspector/) built as part of GSoC 2019. The goal of this project is building on top of this very well received feature and add new support for [Server Sent Events](https://developer.mozilla.org/en-US/docs/Web/API/Server-sent_events) inspection.

The feature should be part of the Network panel and it should allow the user to:

* See list of events received from the server in a side bar (similarly to WebSocket frames)

* See event payload (binary or text data)

* See size & time of every event

* Sort events by size and time

* Filter events

* Explore JSON formatted data using an expandable tree widget

A stretch goal is building binary data inspector and use it for previewing binary packets sent through server-sent events and also WebSocket channels.


## Additional Information

* Student will be submitting their work for code review on [Mozilla’s Phabricator](https://wiki.mozilla.org/Phabricator) instance.

* Communication will be through the [Firefox DevTools’ Slack](https://devtools-html-slack.herokuapp.com/).

* Network panel source code [module](https://searchfox.org/mozilla-central/source/devtools/client/netmonitor)

* WebSocket Inspector source code [module](https://searchfox.org/mozilla-central/source/devtools/client/netmonitor/src/components/websockets)

