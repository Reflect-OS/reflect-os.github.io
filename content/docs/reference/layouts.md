---
title: "Layouts"
description: "Reference pages are ideal for outlining how things work in terse and clear terms."
summary: ""
date: 2023-09-07T16:13:18+02:00
lastmod: 2023-09-07T16:13:18+02:00
draft: false
weight: 920
toc: true
seo:
  title: "" # custom title (optional)
  description: "" # custom description (recommended)
  canonical: "" # custom canonical URL (optional)
  robots: "" # custom robot tags (optional)
---

Layouts represent visual arrangements of the sections on your system's screen.
Layouts will have one or more "locations", which are essentially the slots where you can place a configured section.

Much like sections, each layout also has a "Layout Type" which defines the visual arrangement
and the available configuration options.

Note that you can add multiple sections to the same location, and most layout types offer configuration options which determine how these should be arranged.

The ReflectOS systems on the download page currently come with one layout type, but more are planned.

## Four Corner

Allows placing sections in each of the four corners of the screen, with options for stacking (vertical vs. horizontal) and spacing.

{{< figure
  src="/images/layouts/four-corner.png"
  alt="RelectOS Four Corner Layout Example"
  caption="ReflectOS Four Corner Layout"
>}}
