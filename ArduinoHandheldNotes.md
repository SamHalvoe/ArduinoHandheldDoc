---
created: 2024-01-02T22:55:05+01:00
modified: 2024-01-02T22:55:05+01:00
---

# ArduinoHandheld

Hardware
Teensy 4.1 ()
PSRAM for Teensy 4.1 () * 2
Micro SD Card >= 32 GB ()
Teensy Audio Board for Teensy 4.1 ()
Adafruit STEMMA Speaker with Amplifier (Product ID: 3885) * 2
SparkFun Battery Babysitter ()
Polulo Voltage Regulator StepDown to 3.3 V ()
Polulo Voltage Regulator StepUp to 5 V ()
Single Cell Lipo Battery 4000 mAh
SparkFun Qwiic Joystick () * 2
Adafruit LSM6DSOX + LIS3MDL - Gyro/Accel/Compass (Product ID: 4517)
Adafruit Haptic Motor Driver (Product ID: 2305)
Adafruit Haptic Motor (Product ID: 1201)
Resitive Touch Display 2.8" 240x320 ILI9341 ()
SparkFun Qwiic LED Stick ()
Adafruit AirLift WiFi (Product ID: 4201)
Button () * 8
Input Register ()
Cables []
Custom PCB ?!?
Custom 3D Printed Parts []

Libraries
Teensy Core ()


Software
replace BlockNot with elapsedMillis/elapsedMicros: https://www.pjrc.com/teensy/td_timing_elaspedMillis.html
consider to create classes (e.g. WireController) for each I2C bus and their setup methods in Arduino#setup
log also uptime of handheld with sd logger, and log 'real' time only if available
use 8 bit colors with custom palette (256 colors, maybe 28 * 9 ramps (252) + black & white (254) + grey33 & grey66 (256))
consider to use ChaiScript/AngelScript to enable post build program logic modification (scripting) and moving of program logic from Teensy flash memory to SD card memory and (PS)RAM

ArduinoPet – Dumbo Octopus
likings for food, drinks, activities
skin color change for mood
