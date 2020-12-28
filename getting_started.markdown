---
layout: page
title: Getting Started
permalink: /getting-started/
---

## How to generate an app using Instant Rails

Once you've purchased a license from the [Instant Rails website](https://www.instantrails.app/), you're ready to generate your Dockerized Rails app.
The Instant Rails app generation command is as follows.

```
$ curl get.instantrails.app|sh -s <app name> <license key>
```

If for example your license key is `8d103360d1c68a5d4fb398b15d3d8a60` and you wanted to create an app
called `hello_world`, you would run the following command.

```
$ curl get.instantrails.app|sh -s hello_world 8d103360d1c68a5d4fb398b15d3d8a60
```

This command will generate a Rails app for you, download and unzip it, then start a Rails server that you can visit.

When you see `Listening on http://0.0.0.0:3001` on the screen, you know your app is ready to visit at `http://localhost:3001`.
