---
title: "Project Ideas"
description: "Some options on how to build your smart mirror system with ReflectOS."
summary: ""
date: 2024-10-26T16:06:50-04:00
lastmod: 2024-10-26T16:06:50-04:00
draft: false
weight: 840
toc: true
seo:
  title: "" # custom title (optional)
  description: "" # custom description (recommended)
  canonical: "" # custom canonical URL (optional)
  robots: "" # custom robot tags (optional)
---

There are lots of ways cool projects you can do with ReflectOS, and we hope this page eventually serves as a showcase.  If you build a project and would like to share it, send us a link to it via our [contact form](/contact) and we might share it here!

## Smart Mirrors

Smart mirrors are the primary use case for ReflectOS, and there's a lots of ways to go about getting started.

The easiest way to is to purchase a [Vilros Magic Mirror v4](https://vilros.com/products/vilros-magic-mirror-v4) - it comes ready to go with everything you need besides a Raspberry Pi and a microSD card.  Just follow the instructions on the [quickstart](/docs/getting-started/quickstart) page and you'll be up and running in minutes.

For those looking to build their own, there are a ton of great resources out there.  One of our favorites is from the offical Raspberry Pi website: https://www.raspberrypi.com/tutorials/how-to-build-a-super-slim-smart-mirror/.  Just note that this tutorial was written for the excellent  MagicMirror project - if you'd like to use ReflectOS, be sure to follow the instructions in these docs for configuring your Raspberry Pi instead of the ones listed.  The hardware steps are the same however, and there are a number of great photos showing the process!

## Refrigerator Display

Using ReflectOS to add a info screen to your fridge works surprisingly well - especially if you have dark colored fridge which allows the screen to blend in a bit more.  The other benefit is that where there is a fridge, there is bound to be a power outlet and it's much easier to hide the wiring.

We've had success with ultra-thin monitors like [this one](https://www.amazon.com/Portable-Monitor-Upgraded-Ultra-Slim-Speakers/dp/B088TLQR3K/ref=asc_df_B088TLQR3K) - the monitor itself is slightly magnetic so it readily holds on a fridge with just a little bit of additional support underneath it.  You can run the wires up to the top of the fridge where you can tuck the Raspberry Pi out of the way.

{{< picture
  src="/images/project-ideas/fridge-display.png"
  alt="RelectOS Fridge Display Example"
>}}
