---
title: "FAQs"
description: "Reference pages are ideal for outlining how things work in terse and clear terms."
summary: ""
date: 2023-09-07T16:13:18+02:00
lastmod: 2023-09-07T16:13:18+02:00
draft: false
weight: 940
toc: true
seo:
  title: "" # custom title (optional)
  description: "" # custom description (recommended)
  canonical: "" # custom canonical URL (optional)
  robots: "" # custom robot tags (optional)
---
## How can I help out the project?

ReflectOS is an open source project and aspires to be community driven.  Contributions of all kinds are most welcome!  Check out our [contribution guide](/docs/getting-started/contributing/)!

## How do I change the display from portrait to landscape?

Unfortunately, we are still working on a way to allow users to change this via the web app.  You can follow
along with [this issue](https://github.com/Reflect-OS/firmware/issues/1) for updates.

For the time being however, you can rotate the orientation of the display opening up the microSD card drive on your computer's file explorer, and locating the `config.txt` file.  Open the `config.txt` file in a text editor such as Notepad or TextEdit.

Toward the bottom, you should see a line that looks like this:

```
display_rotate=3
```

Changing the value from `3` to `0` or `2` (depending on your display) should rotate the display into the correct orientation.  Note that you should also adjust the screen size in system settings, as it defaults to a portrait resolution of 1080x1920 - change it to 1920x1080 or whatever is appropriate for your screen's resolution.

## How do I upgrade to the latest firmware?

Currently, you can just download the latest version of ReflectOS for your Raspberry Pi from the downloads page and flash it on to your microSD card, following the same steps from the [quickstart](/docs/getting-started/quickstart) guide.  However, this will overwrite your data and you'll need to reconfigure your system as re-flashing the OS in this way is basically a fresh install.

This is another area where we are still working to provide some key functionality (i.e. updating the firmware while keeping your configuration) without having to use the commandline.  You can follow along with our progress using this [Github issue](https://github.com/Reflect-OS/firmware/issues/2).

For now, users can upgrade their firmware without losing their data by using the [fwup](https://github.com/fwup-home/fwup?tab=readme-ov-file#installing) tool, a simple command line utility.  Here's how to do it:

* Install the tool by [following the instructions](https://github.com/fwup-home/fwup?tab=readme-ov-file#installing) for your computer's operating system
* Download the latest `.fw` file from the [downloads page](/downloads)
* Put your microSD card into your microSD card reader and plug it into your computer
* From the folder where the `.fw` file downloads, open the command prompt/terminal and run the upgrade command.  For example:

```
fwup ReflectOS-firmware-rpi4.fw -t upgrade
```

Be sure to use the correct filename for your Raspberry Pi system!

This should autodetect your microSD card and update the firmware without overwriting your data.

## How is this different from the  MagicMirror² Project?

This project was heavily inspired by the MagicMirror² Project, and draws on a TON of the good ideas that it has developed.

One key difference is target audience - in [the docs](https://docs.magicmirror.builders/about/manifesto.html), the creator of the MagicMirror² Project Michael Teeuw summarizes his goals as follows:

> I started this project as an ultimate starter project for Raspberry Pi enthusiasts...
>
> Of course, a bundled version can be complimentary to the regular un-bundled version. And I'm sure a lot of (new) users will opt for the bundled version. But this means those users won't be motivated to take a peek under the hood. They will just remain 'users'. They won't become contributors, and worse: they won't be motivated to take their first steps in software development.
>
> And to be honest: motivating curious users to step out of their comfort zone and take those first steps is what drives me in this project. Therefore my ultimate goal is this project is to keep it as accessible as possible.

Here at ReflectOS, we LOVE this perspective and fully support these goals.  If you are interested in tinkering with using the command line and software development, we highly recommend building your own ReflectOS extensions or checking out the MagicMirror² Project.  It has an incredibly rich ecosystem of community modules, and because customization is via config files in the code, the modules tend to have a lot more configuration options.

ReflectOS is designed to allow makers and users a way to quickly and easily get started building
(or even selling) smart mirrors and displays.  It has fewer modules (called "sections"), but offers
a way to make a fully customized system without having to "peek under the hood" (though we do highly encourage that if you are interested!).

On the technical side, another key difference is that ReflectOS use native C library based rending
instead of browser based rendering.  While this is a bit tricker to build and develop, it tends to
work a little more smoothly on devices with more limited CPU and memory available.

Lastly, by building the system on the Elixir ecosystem, ReflectOS has a high degree of fault-tolerance and reliability.  Individual parts of the system as well as the OS itself will
automatically restart if there is an issue.  For a device that is intended to be running 24/7 for
months and years on end, this helps ensure that your system is always there and ready when you need it.

All that said, ReflectOS also strives to be community driven and we welcome all contributions to make the ecosystem better for everyone!
