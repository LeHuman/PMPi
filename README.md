# PMPi

Wireless PM2813 GPIB Controller using a Raspberry Pi Pico W.

This project hardware should be adaptable to other GPIB interfaces in a one to one configuration,
as communication still occurs through the same hardware. However, larger networks with more than two nodes are untested and might run into current capacity issues,
where this device cannot output much current compared to what standard IEEE-488 transceivers can, such as with the SN7516x chips. This, again, is untested.

## Key Features

- Wireless
  - Wireless capability is enabled by using a Raspberry Pi Pico W
  - Web interface exposed on local network powered by [mongoose](https://mongoose.ws/)
- Open Source
  - You are reading the open sourcedness of all this
- Obsolete on Arrival $-$ *new*⭐
  - I only know one other person that *might* use this

## Mechanical

<!-- case construction and mounting -->

## Electrical

<!-- schematics and routing -->

## Firmware

<!-- programming the Pico W and the Web UI -->
