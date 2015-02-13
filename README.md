# SafariURIs
Apple Safari does not currently ask the user before opening a URI (Uniform Resource Identifier) in another application. Chrome and Firefox recognize the danger of this, and prompt the user first. Because Safari does not, an attacker can:
* Control iTunes and Steam music playback
* Open many applications, possibly all at once
* Cause hundreds of error messages to be created
* Exploit possible vulnerabilites in applications

To see registered URI schemes on your Mac, run `/System/Library/Frameworks/CoreServices.framework/Versions/A/Frameworks/LaunchServices.framework/Versions/A/Support/lsregister -dump`. Anything in bindings followed by a colon is a scheme. If there is a common application with a URI scheme that is not included in this demo, please add it as an issue.

Hopefully Apple will see the danger here, and decide not to trade security for ease-of-use.
