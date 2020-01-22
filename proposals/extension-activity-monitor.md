# Extension Activity Monitor 

**Mentor:** Luca Greco, Andreas Wagner, Rob Wu

**Email:** lgreco@mozilla.com, awagner@mozilla.com, rwu@mozilla.com

## Project Description

Extensions do most of their work invisibly from users, and so  Extension activity is a complete mystery for most users, even advanced ones.

Providing more transparency could help increase reliability of abuse reporting and accountability for developers, as well as providing an
additional useful tool to aid investigating bugs in the extensions or in the Firefox WebExtensions internals.

## Skills Required

An applicant needs:

* Familiarity with front-end web development (JavaScript, HTML, CSS).
* A good understanding of the capabilities of web APIs.
* Be productive with version control systems (e.g. Git or Mercurial).
* Be able to communicate clearly in English.
* Think critically and be able to independently investigate/debug issues.
* Enjoy working with others, in an open-source setting.

Knowledge of browser extension APIs is a bonus.

## Project Details

An `activityLog` API is available (in Firefox >= 70) to privileged extensions, the applicant's goal is leveraging this API to
create a privileged extension which would explore various ways to present this information to the users.

In particular, this project's goal is to expore the following areas:

- An extension page that shows the active extensions and their effect on the browser, such as altered browser settings or network requests,
  and the messages exchanged between the different parts of the extension.
- For the current tab, show the extensions acting on it
- Saving and loading activity logs from file

The applicant will also write a small API doc for the `activityLog` API, in [reStructuredText format](https://en.wikipedia.org/wiki/ReStructuredText)
as the [api docs available for the privileged `telemetry` API](https://searchfox.org/mozilla-central/rev/c52d5f8025b5c9b2b4487159419ac9012762c40c/toolkit/components/telemetry/docs/collection/webextension-api.rst)

Links to the `activityLog `API internals:
- API JSON schema: [activity_log.json](https://searchfox.org/mozilla-central/rev/c52d5f8025b5c9b2b4487159419ac9012762c40c/toolkit/components/extensions/schemas/activity_log.json)
- API test cases: [test_ext_activityLog.html](https://searchfox.org/mozilla-central/source/toolkit/components/extensions/test/mochitest/test_ext_activityLog.html)
- API implementation module: [ext-activityLog.js](https://searchfox.org/mozilla-central/rev/c52d5f8025b5c9b2b4487159419ac9012762c40c/toolkit/components/extensions/parent/ext-activityLog.js#17)
