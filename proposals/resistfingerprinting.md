# Making Resist Fingerprinting Usable

**Mentor:** Tom Ritter, Tim Huang

**Email:** tom@mozilla.com

## Project Description

Presently, Resist Fingerprinting applies browser and Web API changes uniformly to all webpages. The goal of this GSOC project is to make the Resistfingerprinting checks accept an origin so that users can specify individual top level domains they wish to disable the Resist Fingerprinting checks on. This will mitigate one of the most common annoyances with Resist Fingerprinting where a particular domain they use is broken and they must disable the entire setting.

## Skills Required

An applicant needs:

* Familiarity with C++
* Familiary with HTML/JavaScript and the Web API

## Project Details

[Bug 1450398](https://bugzilla.mozilla.org/show_bug.cgi?id=1450398) captures this task and related discussion.  Current thinking is that nsILoadInfo is the correct object to find and pass to [ShouldResistFingerprinting](https://searchfox.org/mozilla-central/search?q=shouldresistfingerprinting&path=).

From there we can look at the principal and origin attributes and apply the Resist Fingerprinting behavior selectively - disabling it for Web Extensions, possibly restricting it to Private Browsing Mode, and exempting user-specified (via a pref initially) top level domains.

We [evaluated the fingerprinting changes we made](https://docs.google.com/document/d/1xglvY9Ly3kxvZQal3Mk1AssNJoerTW-hGYotQjBBygA/edit) and found that the majority of them are simple to cut over to this model.  Other ones do not make sense (like window size protections.) Finally, a small number are difficult and would probably be exempt from an initial implementation - this includes locale and timezone changes.