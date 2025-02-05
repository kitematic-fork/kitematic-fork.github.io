---
layout: docs
title: Known Issues
permalink: /docs/known-issues/
published: true
---

## Known Issues

---

Kitematic is in beta, and we're still working out the kinks. The most common errors occur at the setup stage since creating a VM reliably with VirtualBox can be tricky.

In the meantime, below are a list of common errors and solutions that work for most people.

### Setup Error or Hanging at 99%

Sometimes Kitematic doesn't set up VirtualBox properly. Retrying the setup usually works (via one of the two retry buttons). If not, try the following commands on the command line:

- `docker-machine rm -f dev`
- `docker-machine create -d virtualbox dev`

Then re-open Kitematic. This usually fixes the issue, but if it persists, feel free to view our [existing GitHub issues](https://github.com/kitematic-fork/kitematic/issues?q=is%3Aopen+is%3Aissue+label%3Abug).

### Contributing Fixes

We're always looking for help to make Kitematic better and more reliable! Visit [our GitHub page](https://github.com/kitematic-fork/kitematic) for docs on how to contribute.

Under the hood, Kitematic uses [Docker Machine](https://github.com/docker/machine) to provision Docker-enabled VMs via VirtualBox. We're still working on a stronger integration with this project. Their [GitHub repo](https://github.com/docker/machine) is a great place to start if you're looking to help fix specific issues around VM provisioning.

### View All Issues

For a full list of Kitematic bugs or issues see our [GitHub issues](https://github.com/kitematic-fork/kitematic/issues?q=is%3Aopen+is%3Aissue+label%3Abug) labelled as `bug`.
