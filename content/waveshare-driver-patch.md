---
title: Waveshare Driver Patch
description: "A patch for the Waveshare epd2in13_V2.py driver to draw the screen upside-down due to limitations of our 3D printed build."
repository: waveshare-driver-patch
weight: 100
---

This is a patch for the Python Waveshare `epd2in13_V2.py` driver, which flips
the output upside-down.

This is because of the limitations of our 3D printed build, and where the USB
power port is located on the Raspberry Pi Zero W.

Instructions on using this patch is available in the project's repository page.
