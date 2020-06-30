---
title: iglü server
description: The core smart home system (both front-end and back-end) code.
repository: iglu-server
weight: 10
---


### Summary

This is the iglü server project, which contains most of the work we have done.
It it a self-contained project, which includes:

- Web server
- Web app files and logic
- Database (SQLite, or can connect to external databases)
- Plugin API

[Visit demo website](https://demo.nacdlow.com)

### Description

iglü server is the web server and control system for the smart home. Its
purpose is to control home appliances and Internet-connected devices. It is
self-contained, handling access-control among other things, and should work
without Internet connection.

### Configuration

A configuration file is automatically generated when run, Dark Sky API is
required for weather information, but is not required to run the app.


### Technical Stack

The server is written in [Go], and uses the [macaron] web framework and [XORM]
for the object-relational mapping library. We have built a custom plugin API
which runs over Remote Procedure Calls (RPC) using HashiCorp's [go-plugin]
library.

For the front-end, iglü uses [MDBootstrap] for the basic design, which we have
built upon. And to provide more interactivity and better user experience
quickly, we have used [jQuery]. Other libraries are used such as [Chart.js],
[FontAwesome], and [Skycons] (from Darksky) to add dynamic graphical elements
on the page.

These are some libraries and frameworks we have used to speed up development
so we could focus on the product.

#### Building and Running

To build and run iglü, you require the following packages:

- git
- Go (1.12+)
- GNU Make
- go-bindata

Then clone the project, build, and run it.

```sh
$ git clone https://github.com/Nacdlow/iglu-server
$ cd iglu-server
$ make
$ ./nacdlow-server run [--port 443] [--dev]
```

No database set-up is required, all required tables will be created
automatically on an SQLite database file.

[Go]: https://golang.org
[macaron]: https://go-macaron.com
[XORM]: https://xorm.io
[go-plugin]: https://github.com/hashicorp/go-plugin
[MDBootstrap]: https://mdbootstrap.com
[jQuery]: https://jquery.com
[Chart.js]: https://github.com/hashicorp/go-plugin
[Skycons]: https://darkskyapp.github.io/skycons/
[FontAwesome]: https://fontawesome.com/
