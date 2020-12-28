---
layout: page
title: Getting Started
permalink: /getting-started/
---

## Buy a license

First, buy a license key from the [Instant Rails website](https://www.instantrails.app/).
As of this writing there are licensing options ranging from $19 to $499.

## Generate your app

Once you have your license, you're ready to generate your Dockerized Rails app.
The Instant Rails app generation command is as follows.

```
$ curl get.instantrails.app|sh -s <app name> <license key>
```

If for example your license key was `8d103360d1c68a5d4fb398b15d3d8a60` and you wanted to create an app
called `hello_world`, you would run the following command.

```
$ curl get.instantrails.app|sh -s hello_world 8d103360d1c68a5d4fb398b15d3d8a60
```
