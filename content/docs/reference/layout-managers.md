---
title: "Layout Managers"
description: "Reference pages are ideal for outlining how things work in terse and clear terms."
summary: ""
date: 2023-09-07T16:13:18+02:00
lastmod: 2023-09-07T16:13:18+02:00
draft: false
weight: 930
toc: true
seo:
  title: "" # custom title (optional)
  description: "" # custom description (recommended)
  canonical: "" # custom canonical URL (optional)
  robots: "" # custom robot tags (optional)
---

Layout Managers are a unique feature of ReflectOS - as their name implies, they manage
which layout should be diplayed on your system's screen.  These are designed to allow your
system's screen to change in response to events in the outside world, such as a schedule or
a person arriving home.

Just like Sections and Layouts, you can create multiple Layout Managers of the same type with different configurations.  However, only one Layout Manager may be active at a given time.  You can select the active layout manager on the Settings page of the web app.

## Static

The static layout manager is the system default, and allows you to select a single layout which is always active.

## Web Condition

The Web Condition layout manager allows your system to change the active layout based
on any publicly available web page.  For example, you could use a weather page to change
the layout based on whether the page contains the word "rain".  Additionally, you could use
a service like [ITTT](https://ifttt.com/explore) (If This Then That)
to update web content (such as a Google Sheet) based on any one of the hundreds of integrations it provides.
