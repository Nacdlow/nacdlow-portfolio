---
title: Dev DNS
description: "A custom Domain Name Server which returns a custom response for our domain, used for testing PWAs with HTTPS support (required by service workers)."
repository: dev-dns
weight: 40
---

This is a DNS which resolves local.nacdlow.com to your local computer's IP
address. This allows testing PWAs.

This uses Miek Gieben's DNS library for both resolving and serving.
### Screenshot
![A screenshot of the development DNS server running](/devdns.jpg)
