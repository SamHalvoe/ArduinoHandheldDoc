---
created: 2024-01-02T23:28:58+01:00
modified: 2024-01-02T23:36:29+01:00
---

# Notes - Software

## General DevNotes

* ~~replace BlockNot with elapsedMillis/elapsedMicros: https://www.pjrc.com/teensy/td_timing_elaspedMillis.html~~
* consider to create classes (e.g. WireController) for each I2C bus and their setup methods in Arduino#setup
* log also uptime of handheld with sd logger, and log 'real' time only if available
* use 8 bit colors with custom palette (256 colors, maybe 28 * 9 ramps (252) + black & white (254) + grey33 & grey66 (256))

## Unplanned Features

* consider to use ChaiScript/AngelScript to enable post build program logic modification (scripting) and moving of program logic from Teensy flash memory to SD card memory and (PS)RAM
