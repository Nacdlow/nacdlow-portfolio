---
title: Plugin SDK
description: "Our SDK for developing plugins for iglü server, which are loading and communicated over RPC."
repository: plugin-sdk
weight: 50
---

This is our Software Development Kit for developing iglü server plugins in Go.
It is based on HashiCorp's [go-plugin] library, which they use in their products.

Plugins communicate with the iglü server via Remote Procedure Calls (RPC), this
makes it so that if a plugin crashes, the server will continue running and
allows us to restart the plugin. Also it allows us to create plugins in
different languages if required in the future.

This SDK provides a Go interface which can be implemented so the server may
load the binary.

[go-plugin]: https://github.com/hashicorp/go-plugin

### Screenshot

<img src="/plugin-sdk.jpg"/>
