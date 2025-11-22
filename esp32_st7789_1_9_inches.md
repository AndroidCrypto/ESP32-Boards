---
layout: page
title: ESP32 ST7789 1.9-inches display
permalink: esp32_st7789_1_9_inches
---

> This is an ESP32 Dev. Board with assembled <b>ST7789 1.9-inches</b> TFT display with <b>SPI</b> interface

NOT CORRECT <img class="mx-auto w-1" src="{{site.baseurl}}/assets/img/pinout/esp32_s3_matrix_pinout_800w.png">

## Documentation


NOT CORRECT
- Official documentation: [https://www.waveshare.com/wiki/ESP32-S3-Matrix](https://www.waveshare.com/wiki/ESP32-S3-Matrix) 
- [Schematic](/assets/pdf/schematic/esp32_s3_matrix_schematic.pdf)

<font color="red">Please note that the LED brightness should not be set too high, it will cause a rapid temperature increase, which can result in damage to the board.</font>

## Libraries

The following libraries and version numbers are tested with this board:

- **Adafruit NEO Pixel** by Adafruit, version 1.15.2, [https://github.com/adafruit/Adafruit_NeoPixel](https://github.com/adafruit/Adafruit_NeoPixel)
- **Adafruit NEO Matrix** by Adafruit, version 1.3.3, [https://github.com/adafruit/Adafruit_NeoMatrix](https://github.com/adafruit/Adafruit_NeoMatrix)
- **SensorLib** by Lewis He, version 0.2.1 , [https://github.com/lewisxhe/SensorLib](https://github.com/lewisxhe/SensorLib)

## Development board profile

| Position | Characteristics | 
|----------------------------------------|--|
| Processor: | ESP32 module with dual-core Xtensa LX7, Flash 4 MB, no PSRAM |
| CPU Frequencies | 160/160/80 MHz (for WiFi), 40/20/10 MHz (no WiFi) |
| Pins available on Breadboard | 0, 4, 5, 12, 16, 17, 18, 19, 21, 22, 23, 25, 26, 27, 32, 33, 34, 35, 36, 39 (total 20), 3.3V, 5V, GND |
| Pins available on solder pads | NO |
| Pins available internally | 0 (BOOT button), ### display |
| Pins safe to use | ### 1, 2, 4, 5, 6, 7, 33, 34, 35, 36, 37, 38, 39, 40 |
| Display | YES, ST7789 1.9-inches display, SPI interface |
| Interfaces | 1x I2C, 2x SPI, 2x UART, 11x GPI0 (PWM), 4x ADC |
| Onboard Power LED | NO |
| Onboard GPIO LED | NO |
| USB-Connection |USB-C, Controller: CH340 |
| Wi-Fi connector | PCB antenna |
| Wi-Fi | YES, 802.11 b/g/n (2.4 GHz), STA/AP/Mixed |
| Bluetooth Classic | YES, 5.0 |
| Bluetooth Low Energy (BLE) | YES, Bluetooth 5.0 LE protocols |
| Battery connector | NO |
| Battery loading | NO |
| Battery voltage measure | NO |
| Battery voltage measure control | NO |
| Extern voltage control | NO |
| Restart button | YES |
| BOOT button | YES, GPIO 0 |
| On-/Off Switch | NO |
| SD card reader | NO |
| Breadboard pins | 2 * 12 pins |
| QWIIC connector | NO |
| Internal temperature sensor | ### YES |
| Low Dropout Voltage Regulator (LDO) | AMS1117 (1000 mA) |
| Breadboard pins distance (width) | 3,0 cm (does not fit on one breadboard) |
| Security features | Encryption hardware accelerators that support AES-128/256, hashing, RSA, HMAC, digital signatures, and secure startup |
| Expansion board | NO |
| Arduino board selection | ESP32 Dev Module |
