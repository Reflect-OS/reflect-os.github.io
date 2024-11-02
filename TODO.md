## ReflectOS - TODO

### Open Source Plan

[x] Support multiple Raspberry Pis
    [x] Zero 2 W
    [x] Zero W
    [x] Raspberry Pi 3a
    [x] Raspberry Pi 3 B / B+
    [x] Raspberry Pi 4 B [untested]
    [x] Raspberry Pi 5 [untested]
[x] Publish Firmware
    [x] Readme
    [x] Build firmware for all supported Raspberry PIs
    [x] Fix bug for bottom left layout
[] Public Website
    [x] Homepage
    [] Getting Started
        [] Flashing Firmware
        [] Connecting to the Network
        [] Configuring your system
    [] Core Extensions
        [] Sections
        [] Layouts
        [] Layout Managers
    [] Advanced
        [] Basic workflow for working locally
        [] Change splash screen
        [] Add an extension library
    [] Contributing
    [] FAQ
        * How is this different from MagicMirror2
        *


### System
[x] Fix splash screen delay
[x] Boot splash screen
    [x] Update reflect_os_rpi0 to use custom build root package, instead of hacking the downloaded buildroot to pull the FBV from a different location
[x] Fix overscan
[x] Set up a "branded" hostname
[x] Enable bcm_host.h on reflect_os_rpi0 to allow use of Scenic 0.11
[x] Enable using Raspberry Pi Zero W 2

#### Settings
[x] Update screens and sections to respect viewport Size
[x] Update scenes to respect Default Timezone
[x] Update scenes to respect Default Time format
[x] Trigger pub/sub event when system configs change

### Console
[x] Allow changing system settings

### Layouts UI
[x] Allow multiple configurable layouts with unique section options
[] Allow setting a daily schedule determining which layout to show
[x] Allow different layouts
    [] Top Left / Top Right / Full width bottom

### Network Config Workflow
[x] Network Setup - Welcome
[x] Network Setup - Configure
[x] Network Setup - Error
[x] Network Setup - Success
[x] Network error screen

### DateTime
[x] Handle pub/sub message when default timezone changes

### Calendar
[x] Basic functionality
[x] Handle pub/sub message when default timezone changes
[x] Global time format
[x] Handle pub/sub message when default timezone changes
[] Error handling for request errors

### RSS Feed
[] Error handling for request errors

### Notification Section
[x] Show message when there are no notifications to display

### Weather Section
[x] Current weather section
[x] Today weather section
[x] Create daily weather section
[x] Pirate Weather Provider
~~[] Create notifications from weather alerts weather alerts~~
[] Error handling for request errors
[] Show error if lat/long are not provided

~~[] Respect time format~~

### Sports Score Section [as a seperate package]
[] Create basic sports score section, allowing selection of teams and displaying the scores
[] Show game status
[] Handle pub/sub message when default timezone changes
