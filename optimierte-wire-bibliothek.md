# ⛓ Optimierte Wire Bibliothek

Für eine schnellere Kommunikation über I2C wird die optimierte Wire Bibliothek von Richard Gemmell genutzt (siehe [https://github.com/Richard-Gemmell/teensy4\_i2c](https://github.com/Richard-Gemmell/teensy4\_i2c) und [https://www.pjrc.com/teensy/td\_libs\_Wire.html](https://www.pjrc.com/teensy/td\_libs\_Wire.html)).

Im Projekt wird die optimierte Wire Bibliothek eingebunden, indem der Ordner Wire in Teensyduino durch einen Ordner Wire mit Wire.h ersetzt, der folgenden Code enthält:

```arduino
// This header is used to replace the standard Wire implementation with the optimized version for Teensy 4.x.
// Replace the directiory of standard Wire implementation in the Teensy board (directory) with this directory and Wire.h file.

#include <i2c_driver_wire.h>
```
