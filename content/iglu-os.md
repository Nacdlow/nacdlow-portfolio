---
title: iglüOS
description: Our custom Linux distribution (based on Raspbian Buster Lite) built for our Raspberry Pi Zero W, which enables Ethernet Driver, SPI for e-ink display, and our custom services.
repository: iglu-os
weight: 20
---

<img src="/igluOS.jpeg" width="500" />

iglüOS is our custom Raspbian Lite-based distribution built for Nacdlow's iglü.
It allows you to have an OS image for the Raspberry Pi with iglü installed as a
service, which boots on startup.

It also allows you to also set up WiFi configuration (eduroam, in this case)
for expo purposes.

Our distribution includes the following changes:

- Support for Real-time Clock (specifically, PCF8523), and removes the
  `fake-hwclock`.
- Support for using Raspberry Pi's Ethernet adapter (appears as Ethernet gadget
  device over USB, static ip set to `10.0.0.2`).
- Support for eduroam with pre-filled credentials.
- Installs [iglü server](/iglu) and adds it as a service.
- Installs and runs our [e-ink display program](/e-ink/) as a service.
- Enables SPI for e-ink display support.

We ran this distribution on a Raspberry Pi Zero W, which contains a Waveshare
e-ink display and a real-time click (RTC). We placed this in a 3D-printed case
printed on a Prusa 3D printer at the Edinburgh Hacklab.
