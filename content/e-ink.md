---
title: E-Ink Display
description: "The E-Ink interface for our iglü product, which displays home statistics."
repository: e-ink-display
weight: 90
---

<img src="/eink.jpg" width="500"/>

This is a program written in Python which pulls in data from the smart home
system and displays it on the e-ink display. We used FontAwesome icons and
converted them to bitmaps to support the display.

This program uses our [Waveshare Driver Patch](/waveshare-driver-patch/) so the
display is flipped upside-down, due to the space constriction in the 3D printed
case.
