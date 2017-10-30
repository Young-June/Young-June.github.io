---
layout: post
title:  "MacOS X 10.13 High Sierra 에서 Android Emulator 문제 해결"
date:   2017-10-30 12:46:41 +0900
categories: jekyll update
---



https://stackoverflow.com/questions/45896535/intel-haxm-on-macos-high-sierra-10-13


Use the new Hypervisor.Framework support on macOS.

Add this line in ~/.android/advancedFeatures.ini (create this file if it doesn't exist already).

HVF = on
Issue answered here: https://issuetracker.google.com/issues/62395878#comment7

That's worked for me. Hope it help.

shareimprove this answer
