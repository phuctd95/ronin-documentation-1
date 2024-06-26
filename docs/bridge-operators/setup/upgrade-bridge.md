---
description: Get the latest version of the bridge's software.
title: Upgrade bridge software
---

## Overview

This page describes how to get the latest version of the software for the bridge node.

Upgrades are usually backwards-compatible and can contain performance
improvements, bug fixes or new features. It's recommended that every node is
upgraded as soon as possible.

An upgrade, however, can also be a hardfork, which is usually not
backwards-compatible. If your node fails to upgrade before a hardfork block
occurs, the data on your node can differ from that on the network. Therefore,
it's critical to upgrade your node before a hardfork occurs. All Ronin-planned
hardforks are announced seven days in advance on
our [Discord](https://discord.gg/roninnetwork) server and
the [Ronin Newsletter](https://blog.roninchain.com).

## Upgrade bridge version

Every bridge release is published on
[GitHub](https://github.com/ronin-chain/bridge-v2/releases). To find the Docker
image for each release, visit
[Github Container Registry](https://github.com/ronin-chain/bridge-v2/pkgs/container/bridge).

To download the latest image, follow these steps:

1. In your `.env` file, set `BRIDGE_IMAGE` to the following:

   ```bash
   ghcr.io/ronin-chain/bridge:v0.2.9-61da305
   ```

2. Save the changes.
3. Run `docker-compose up -d`.
