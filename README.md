## NEO Flight Computer Schematics
These are the schematics for the NEO dual deploy flight computer.

### Features
- IMU For inertial positioning and acceleration data.
- Barometer for barometric altitude.
- 2 Pyrotechnic channels for charge deployment.
- Support for up to 12V Powersupply.
- Intergrated Flash Storage and SD Card for Data logging (optional)
- Battery Voltage Reader
- Almost all components are through-hole soldered for ease of assembly without solder paste.
- Support for various adafruit IMUs or Barometers.
- Small footprint (55x100mm) to keep manufacturing cheap.
- LED/Buzzer for output
- I2C/SPI Expansion Slots

### Main components:
Full BOM is in the repo.
- Arduino NANO processor (widely available and easily programmable, low memory so libraries that can be used are limited (can be used with the Nano Every, which has more memory))
- Adafruit BMP388 breakout board (compatible with almost all adafruit Barometer boards)
- Adafruit ICM20649 IMU (compatible with almost all adafruit IMU boards)
- Micro SD card socket
- W25Q32FV Winbond Flash Storage Chip (compatible with other similar pinout chips like the SST25VF064C from Microchip)

### Firmware
Firmware for the board is a work in progress, but the board is compatible with all main Arduino Libraries for each sensor and the SD and Flash Chip. Writing simple software for launch and apogee detection isn't too difficult.
