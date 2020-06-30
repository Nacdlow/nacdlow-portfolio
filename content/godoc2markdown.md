---
title: godoc2markdown
description: "A tool which converts go doc to Markdown. We needed this tool to generate documentation of private repositories, which wasn't possible - so we built a solution."
repository: godoc2markdown
weight: 30
---

This is a simple Unix-like tool which allows you to pipe the output of go doc
to generate Markdown.

The purpose of this tool is to allow private Go projects generate Markdown
documentation, where websites like [GoDoc] has no access to the repository.

After implementing this, we have created a script to generate our Wiki for the
iglü server repository automatically, including a table-of-contents.

### Screenshots

<img src="/godoc.jpg" width="500"/>
<img src="/godoc2.jpg" width="500"/>

### Usage example

If you want to generate a Markdown of the package in the current directory, and
save it to a file, you can run:

```
$ go doc -all . | godoc2markdown > DOCUMENTATION.md
```

[GoDoc]: https://godoc.org
