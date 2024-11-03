---
title: "Sections"
description: "Reference pages are ideal for outlining how things work in terse and clear terms."
summary: ""
date: 2023-09-07T16:13:18+02:00
lastmod: 2023-09-07T16:13:18+02:00
draft: false
weight: 910
toc: true
seo:
  title: "" # custom title (optional)
  description: "" # custom description (recommended)
  canonical: "" # custom canonical URL (optional)
  robots: "" # custom robot tags (optional)
---

In ReflectOS, the visual elements which display on the dashboard are called "Sections", and they are the primary
building blocks of the system.  When creating a new section, you first select the "Section Type" from the
pre-installed available options.

After selecting the type, you can name and configure the section.  Most section types offer several configuration options which allow customization of what information is displayed.

{{< callout context="tip" title="Pro Tip" icon="outline/circle-check" >}}
You can create multiple sections of the same type and configure them differently.  For example, the `Date/Time` section allows you to configure the time zone, so you could have a `Date/Time` section for several locations worldwide on your dashboard.
{{< /callout >}}

The ReflectOS systems on the download page currently come with the following Section Types installed:

## Calendar

The calendar section provides an agenda view of upcoming events - all you need to provide is an iCal calendar link.  There are number of calendar providers which have feeds you can use.  For example, Google allows you
to use a "secret address" for your calendar which works with ReflectOS - check out [the instructions](https://support.google.com/calendar/answer/37648?hl=en#zippy=%2Csecret-address%2Cget-your-calendar-view-only).

Note that system is designed to show all events starting after midnight of the current day.

Here's an example of the section with the US Holiday calendar:

{{< figure
  src="/images/sections/calendar.png"
  alt="RelectOS Calendar Section Example"
  caption="ReflectOS Calendar Section"
>}}

## Countdown

The countdown section is great for getting excited about an upcoming vacation, wedding, or anything else you might be looking forward to.  All you need to do is provide the date and time when it's happening and a brief
description.

{{< figure
  src="/images/sections/countdown.png"
  alt="RelectOS Countdown Section Example"
  caption="ReflectOS Countdown Section"
>}}

## Date/Time

The date/time section is about as straightforward as it gets - just shows a digital clock in either 12 or 24 hour format, and provides a variety of date formats as well.  However, as mentioned in the tip above you can also specify the timezone, and could add multiple date/time sections to your dashboard for different geographic locatons.  Like most sections, you can specify an optional label to help keep things organized.

{{< figure
  src="/images/sections/date-time.png"
  alt="RelectOS Date/Time Section Example"
  caption="ReflectOS Date/Time Section"
>}}

## RSS Feed

RSS (Really Simple Syndication) Feeds are a very common way blogs, news sites, and other organizations distribute streams of information.  This section allows you to display the title and summary for each item in the feed.  You can also select how many items from the feed you'd like to show at once.

Because of the variety of RSS Feeds publicly available, this is a simple but incredibly flexible way to provide at-a-glance headlines and information on your system dashboard.

{{< figure
  src="/images/sections/rss-feed.png"
  alt="RelectOS RSS Feed Section Example"
  caption="ReflectOS Feed Section"
>}}

## Weather

The weather section optionally provides current conditions as well as hourly and daily forecasts for the zipcode
you specify.  If you'd like to be more precise, you can also manually enter a latitude and longitude.  Hourly weather is shown for a configurable number of hours up to midnight of the current day.

By default, weather information is provided by the National Oceanic and Atmospheric Adminstration's free service.  This is super simple to set up as it doesn't require any kind of account to use, but the current weather conditions are not always updated frequently.

For users wanting more up-to-the-minute information, we recommend using the Pirate Weather provider.  It does require creating a free account to obtain an API Key, but tends provide more frequent forecast and conditions updates.  For more details and to create an account, see the [Pirate Weather Website](https://pirate-weather.apiable.io/products/weather-data/Plans).

{{< figure
  src="/images/sections/weather.png"
  alt="RelectOS Weather Section Example"
  caption="ReflectOS Weather Section"
>}}


{{< callout context="note" title="Note" icon="outline/info-circle" >}}
Didn't see something you were looking for?  Check out the [contributing](/docs/getting-started/contributing/) page to learn how to make a feature request or build your own sections to suite your needs!
{{< /callout >}}
