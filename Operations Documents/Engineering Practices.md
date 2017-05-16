# Engineering Practices Guide

## Code:
* Everything in its own branch, please use issue numbers on the end of the branch name
* Assume each branch might not get merged, so keep things modular so a release isn’t a big deal. There should be ~0 extra effort needed to make a release.
* Push frequently (if it’s not pushed, it is dead to the company).
* Commit messages should concisely explain the areas of code changed
* Commit messages should end in an issue number
* Branch off of dev, then PR back into dev.
* Release candidate branches are branched off of dev then merged into master.
* Nothing gets into master without being flown
* Follow the objective-c style guide (or whatever style guide is relevant).
* Don’t code without a sufficient understanding of the UX to know the code is absolutely necessary.
* Force the UX to be designed (be annoyingly upfront w/ the team) before touching any UI code.
* Force the Protocol to be agreed to (be annoyingly upfront w/ the team) before coding any network code.
* Anything touching pixels on the screen should have a screenshot uploaded on the ticket and reviewed by Dave before closing the ticket.
* Update tickets and hand them off to other people when you’re blocking.
* Mark tickets as testing, needs merge, etc so we can see the progress on a given ticket
* Where practical, write unit tests for behavior.
* Where not immediately practical to implement, create tickets for unit testing.

## Communication:
* If you’re going to be messing with a server/resource that affects development, ask first to give people a chance to yell
* If you’re going to be messing with a production resource, announce it, give an explanation, post updates, and say when it’s over
* If you’re going to be online/offline doing something, please let people know as it’s happening
* If a tool is broken, yell about it

## Flight Testing:
* Test in sim first, then later fly hardware. If it didn’t work in simulation, it’s not worth your time and risk to fly it.
* People safety first
* Wear safety glasses.
* Always have a testing plan written down before you go out testing.
* Dump notes on what you’re learning live in Slack, or on paper and then immediately type up.
* Don’t leave for the day/weekend without doing that upload of information on testing notes.
* If you touch anything that can reasonably affect flight safety, it requires flight testing on real hardware before we can say it’s releasable.
