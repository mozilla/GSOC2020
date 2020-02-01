# Improve infrastructure underpinning Firefox's in-tree documentation proposal

**Mentor:** Sylvestre Ledru

**Email:** s@mozilla.com

## Project Description

[Firefox's in-tree documentation](https://firefox-source-docs.mozilla.org/) is "underpinning Firefox's in-tree documentation".

## Skills Required

An applicant needs to be experienced in the following technologies:

* Mercurial
* Python
* Rst (or Markdown)

An applicant needs the following skills:

* Contributing to Open Source
* Familiarity with Source Docs Infrastructure
* Enjoy working with others
* Able to work remotely

## Project Details

Writing docs for Firefox's in-tree source docs can be time consuming and difficult.

With MDN de-prioritizing build and workflow docs, we need a suitable replacement for all of Firefox's contribution and workflow documentation. The great advantage of documentation living in-tree, is that it can be updated along with the source. Unfortunately the current system to build and generate docs is difficult to write for and slow to build. Even if we made some progress in 2019, we want more developers creating or updating docs. Therefore, we want to make this easier.

The project will focus on:

* Improve performances of the doc build pipeline
* Maintain well structured hierarchies
* Automatic rendering at review phase in Phabricator to simplify review
* Run and generate the doc when one of the files is touched at review phase
* Develop a mechanism to import remaining docs from MDN into the source tree
* Improve the caching mechanism when publishing a new documentation
* Improve markdown support

