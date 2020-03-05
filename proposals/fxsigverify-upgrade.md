# Modernize & Enhance Fx-sig-verify

**Mentor:** Hal Wine

**Email:** hwine@mozilla.com


## Project Description

[Fx-sig-verify][fxsigverify] is an AWS lambda function written in Python 2.
It provides an independant check that every Firefox Installer available for
download from Mozilla is signed with the correct key.

The project needs to be ported to Python 3, and other validations added. These
tasks may involve locating or writing some 3rd party libraries used for some
functionality.


## Skills Required

To be successful, we believe you will need the following skills:

* Good knowledge of Python 3
* An understanding of how to work with binary data and basic cryptography
* Familiarity with the constraints of event driven serverless computing
* Beginner knowledge of Docker (used for build and test).

## Project Details

Fx-sig-verify is an important part of our security assurance program for Firefox
products. It currently validates the signature on '.exe' installers for Microsoft
Windows, and we want to extend coverage to '.msi' and our updates.

[Fx-sig-verify][fxsigverify] is a stable application that has operated in
production for years. We want to [modernize it][gh55] so we can more easily
apply security patches from external libraries.

The work currently identified is that for the "[0.5.0 Breaking Changes][v050]"
milestone.

## Additional Information

Before applying, you should review the [documentation][docs] to ensure you feel
comfortable with the technologies involved, with the exception of AWS. We will
be able to provide any AWS consulting, and configuration or service changes needed.

[fxsigverify]: https://github.com/mozilla-services/fx-sig-verify
[gh55]: https://github.com/mozilla-services/fx-sig-verify/issues/55
[v050]: https://github.com/mozilla-services/fx-sig-verify/milestone/2
[docs]: https://fx-sig-verify.readthedocs.io/en/latest/index.html
