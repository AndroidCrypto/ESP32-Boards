---
layout: page
title: ESP32 ST7789 1.9-inches display
permalink: esp32_st7789_1_9_inches
---

> This is an ESP32 Dev. Board with assembled <b>ST7789 1.9-inches</b> TFT display with <b>SPI</b> interface and a resolution of <b>170 x 320 pixels</b> (no touch)

NOT CORRECT <img class="mx-auto w-1" src="{{site.baseurl}}/assets/img/pinout/esp32_s3_matrix_pinout_800w.png">

## Documentation

There is no documentation available for this board. I saw it is often advertised as part of the ESP32 Cheap Yellow Display (CYD) family, but has a total different breadboard pin layout.

## Libraries

The following libraries and version numbers are tested with this board:

- **TFT_eSPI** by Bodmer, version 2.5.43, [https://github.com/Bodmer/TFT_eSPI](https://github.com/Bodmer/TFT_eSPI)
- **LovyanGFX** by Lovyan03, version 1.2.7, [https://github.com/lovyan03/LovyanGFX](https://github.com/lovyan03/LovyanGFX)

## Development board profile

| Position | Characteristics | 
|----------------------------------------|--|
| Processor: | ESP32 module with dual-core Xtensa LX7, Flash 4 MB, no PSRAM |
| CPU Frequencies | 160/160/80 MHz (for WiFi), 40/20/10 MHz (no WiFi) |
| Pins available on Breadboard | 0, 4, 5, 12, 16, 17, 18, 19, 21, 22, 23, 25, 26, 27, 32, 33, input only: 34, 35, 36, 39 (total 20), 3.3V, 5V, GND |
| Pins available on solder pads | NO |
| Pins available internally | 0 (BOOT button) and display (see below |
| Pins for ST7789 | BL:21, MISO: n/c, MOSI: 13, SCLK: 14, CS: 15, DC: 2, RST -1, HSPI-port, 80 MHz |
| Pins safe to use | 4, 5, 12, 16, 17, 18, 19, 22, 23, 25, 26, 27, 32, 33, input only: 34, 35, 36, 39 |
| Display | YES, ST7789 1.9-inches display, SPI interface, 170x320 pixels, no touch controller |
| Interfaces | 1x I2C, 2x SPI, 2x UART, 11x GPI0 (PWM), 4x ADC |
| Onboard Power LED | NO |
| Onboard GPIO LED | NO |
| USB-Connection | USB-C, Controller: CH340 |
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
