<!-- PROJECT: PMPi -->
<!-- TITLE: PMPi -->
<!-- FONT: IBM Plex -->
<!-- KEYWORDS: Controller, Raspberry Pi Pico W, Embedded, Hardware, Firmware -->
<!-- LANGUAGES: C, C++, Python -->
<!-- TECHNOLOGY: Mongoose Embedded Web Server, RESTful API, Altium -->
<!-- STATUS: Work In Progress -->

![PMPi-Logo](<PMPi-Logo/PMPi Logo Full.png>)

[About](#about) - [Key Features](#key-features) - [Child Repositories](#child-repositories) - [Related](#related) - [License](#license)

## Status

**`Work In progress`**
> *Focus has mainly been on making hardware - May 2024*

## About
<!-- DESCRIPTION START -->
Wireless PM2813 GPIB Controller using a Raspberry Pi Pico W.

The PM2813 is a 3 channel programmable power supply produced by Phillips/Fluke in the mid to late 90s. Featured on the back side of the device is a IEEE 488 interface, aka a GPIB port. Naturally, this interface is long outdated and I found that there is no easy solution to remotely control this device without multiple bulky translators and unintuitive interfaces.
The goal of this project is to add a non-invasive device to the PM2813 to create an easy to use web interface to interact with it's 3 channel output, completely hiding the underlying legacy communication to the end user.
<!-- DESCRIPTION END -->

This project hardware should be adaptable to other GPIB interfaces in a one to one configuration,
as communication still occurs through the same hardware. However, larger networks with more than two nodes are untested and might run into current capacity issues,
where this device cannot output much current compared to what standard IEEE-488 transceivers can, such as with the SN7516x chips. This, again, is untested.

### Why

This project has mainly served as an exercise in hardware and firmware development, as I don't imagine a product this niche would do all that well. However, a generalized GPIB controller may be more applicable, but that has been done multiple times at this point. The main goal of this project focuses solely on deeply integrating with the PM2813 and potentially the PM28 series as a whole, the only difference being the number of channels.

## Key Features

- Wireless
  - Wireless capability is enabled by using a Raspberry Pi Pico W
  - Web interface exposed on a local network, powered by [mongoose](https://mongoose.ws/)
- Open Source
  - You are reading the open sourcedness of all this
- Obsolete on Arrival $-$ *new*⭐
  - I only know one other person that *might* use this

<!-- ## Mechanical -->

<!-- case construction and mounting -->

<!-- ## Electrical -->

<!-- schematics and routing -->

<!-- ## Firmware -->

<!-- programming the Pico W and the Web UI -->

## Related

- Twilight-Logic/[AR488](https://github.com/Twilight-Logic/AR488)
- pchernikhowsky/[AVR488](https://github.com/pchernikhowsky/AVR488)

## Child Repositories

- [PMPi-Firmware](https://github.com/LeHuman/PMPi-Firmware)
- [PMPi-PCB](https://github.com/LeHuman/PMPi-PCB)

## License

MIT
