# BlueMicro Firmware

A Keyboard Firmware for nRF52832 Boards with a pinout compatible with the Arduino Pro Micro

## Build Status
| Branch  | Windows Build  | Docker Build | Adafruit BSP Version  |
|---|---|---|---|
| Master  |  ![Build Status](http://toronto.jpconstantineau.com:8585/buildStatus/icon?job=BlueMicro_BLE%20-%20Push) | ![Build Status](http://toronto.jpconstantineau.com:8585/buildStatus/icon?job=BlueMicro_BLE-master-Docker-nrf52832)  |![Adafruit Library for releases](https://img.shields.io/github/release/adafruit/Adafruit_nRF52_Arduino.svg)  |
| Develop |![Build Status](http://toronto.jpconstantineau.com:8585/buildStatus/icon?job=BlueMicro_BLE-develop) | ![Build Status](http://toronto.jpconstantineau.com:8585/buildStatus/icon?job=BlueMicro_BLE-develop-Docker-nrf52832) | ![Adafruit Library for releases](https://img.shields.io/github/release/adafruit/Adafruit_nRF52_Arduino.svg)   |

[![GitHub license](https://img.shields.io/github/license/jpconstantineau/BlueMicro_BLE.svg)](https://github.com/jpconstantineau/BlueMicro_BLE)
[![Current Version](https://img.shields.io/github/tag/jpconstantineau/BlueMicro_BLE.svg)](https://github.com/jpconstantineau/BlueMicro_BLE/tags)

[![GitHub forks](https://img.shields.io/github/forks/jpconstantineau/BlueMicro_BLE.svg)](https://github.com/jpconstantineau/BlueMicro_BLE/network)
[![GitHub stars](https://img.shields.io/github/stars/jpconstantineau/BlueMicro_BLE.svg)](https://github.com/jpconstantineau/BlueMicro_BLE/stargazers)
[![GitHub contributors](https://img.shields.io/github/contributors/jpconstantineau/BlueMicro_BLE.svg)](https://github.com/jpconstantineau/BlueMicro_BLE/graphs/contributors)

[![Discord](https://img.shields.io/discord/449593318247235589.svg)](https://discord.gg/ecnCR9P)


[![GitHub pull requests](https://img.shields.io/github/issues-pr/jpconstantineau/BlueMicro_BLE.svg)](https://github.com/jpconstantineau/BlueMicro_BLE)

[![GitHub issues](https://img.shields.io/github/issues/jpconstantineau/BlueMicro_BLE.svg)](https://github.com/jpconstantineau/BlueMicro_BLE/issues)


**Compatible Hardware**  

![BlueMicro](/docs/images/BlueMicro_Hardware.jpg)

Top Row: 5x5Backpack, 4x4Backpack

Bottom Row: BlueMicro V2.0,  BlueMicro V1.0, BlueNano V2.0, BlueNano V1.0, Pro Micro (For Reference)



* [Adafruit nRF52 Feather](https://www.adafruit.com/product/3406) (Software compatible - not Pinout compabible)
* [BlueMicro V1.0](https://github.com/jpconstantineau/NRF52-Board/tree/master/EByte_E73)  Serial TX/RX routed through D2 and D3; Designed for the ErgoTravel; Tested and Gerber available
* [BlueMicro V1.1](https://github.com/jpconstantineau/NRF52-Board/tree/master/EByte_E73)  Compatible with more Keyboards - Serial TX/RX are routed separately; Tested and Gerber available
* [BlueMicro V2.0b](https://github.com/jpconstantineau/NRF52-Board/tree/master/EByte_E73_Batt) Compatible with more Keyboards - Serial TX/RX are routed separately, LiPo Charger on board; Tested and Gerber available 
* [BlueMicro V2.0c](https://github.com/jpconstantineau/NRF52-Board/tree/master/EByte_E73_Batt_ErgoTravel) Serial TX/RX routed through D2 and D3; Designed for the ErgoTravel. LiPo Charger on Board with battery connection connected to RAW pin. Tested and Gerber available.
* [BlueNano V1.0](https://github.com/jpconstantineau/NRF52-Board/tree/master/NRF52832-base/NRF52832%20Base) Compatible with even more Keyboards due to its small size 3.3v regulator on board; Tested and Gerber available, not recommended due to the on-board regulator and no LiPo Charger. No longer being developed.
* [BlueNano V2.0](https://github.com/jpconstantineau/NRF52-Board/tree/master/NRF52832-base/NRF52832%20Lipo) Compatible with even more Keyboards due to its small size - Serial USB and PoLi Charger on board. Lots of 0402 components and 2 QFN packages to solder. Under Development.
* [4x4 Backpack](https://github.com/jpconstantineau/NRF52-Board/tree/master/4x4_backpack/4x4_backpack) For use with [40percent.club 4x4 Boards](https://www.40percent.club/2018/01/4x4x4x4x4.html). Uses a CR2032 Battery.
* [5x5 Backpack](https://github.com/jpconstantineau/NRF52-Board/tree/master/5x5_backpack/5x5_backpack) For use with [40percent.club 5x5 Boards](https://www.40percent.club/2018/04/5x5.html). Uses a CR2032 Battery.

* BLE Phage       (Compatible with even more Keyboards due to its small size - Serial USB and PoLi Charger on board)
* [BLE Phage Basic](https://southpawdesign.net/products/blue-phage-basic?variant=8958741545020) (Compatible with even more Keyboards due to its small size - Serial TX/RX are routed separately)


Maintainer: [/u/jpconstantineau](https://github.com/jpconstantineau)  


# Documentation
See the pages [Here](http://bluemicro.jpconstantineau.com/#)

You can contribute to the documentation by editing the markdown files located in the docs folder of the repository.


# Want to help?
Contact /u/jpconstantineau on reddit.


# Credits

The firmware uses the same Arduino Core as the [Adafruit nRF52 Feather Boards](https://github.com/adafruit/Adafruit_nRF52_Arduino)

The Adafruit NRF52 Arduino Core is based on [Arduino-nRF5](https://github.com/sandeepmistry/arduino-nRF5) by Sandeep Mistry, which in turn is based on the [Arduino SAMD Core](https://github.com/arduino/ArduinoCore-samd).

The following tools are used:

- Arduino IDE as the Editing Environment
- GCC ARM Embedded as the compiler
- Nordic's nrfutil 0.5.2 for flashing the firmware by serial interface
- J-Link for flashing the bootloader by SWD interface
