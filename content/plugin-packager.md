---
title: Plugin Packager
description: "Our internal plugin packager GUI application, which allows us to generate manifests, checksums and archives plugins before pushing them to our custom plugins repository."
repository: plugin-packager
weight: 60
---

This is our internal plugin package program, which allows us to:

- Generate/check manifests
- Cross-compile to multiple platforms
- Strip binaries
- Calculate checksums
- Archive the binary (using `xz`)

It then places it in the marketplace repository, and stores them in categories
depending on the platform (just like Debian's APT).

### Screenshot

![Screenshot of the plugin packager](/plugin-packager.jpg)
