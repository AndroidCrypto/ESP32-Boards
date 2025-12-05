---
layout: page
title: ESP32-S3 T-Display-S3 ST7789 1.9-inches display
permalink: esp32_s3_t_display_s3_st7789_1_9_inches
---

> This is a LilyGo ESP32-S3 Dev. Board with assembled <b>ST7789 1.9-inches</b> TFT display with <b>8-Bit Parallel</b> interface and a resolution of <b>170 x 320 pixels</b> (no touch).

## Documentation

- [LilyGo shop](https://lilygo.cc/products/t-display-s3)
- [LilyGo GitHub repository](https://github.com/Xinyuan-LilyGO/T-Display-S3)

## ESP32-S3 T-Display S3 pin mapping overview
<img class="mx-auto w-1" src="{{site.baseurl}}/assets/img/pinout/esp32_s3_t_display_s3_pinout_800w.png">

## Libraries

The following libraries and version numbers are tested with this board:

- TFT_eSPI by Bodmer, version 2.5.43, https://github.com/Bodmer/TFT_eSPI
- LovyanGFX by Lovyan03, version 1.2.7, https://github.com/lovyan03/LovyanGFX

## Development board profile

| Position | Characteristics | 
|----------------------------------------|--|
| Processor: | ESP32-S3 processor with dual-core Xtensa LX7 (QFN56, revision v0.2, Flash 16 MB, 8 MB PSRAM |
| CPU Frequencies | 240/160/80 MHz (for WiFi), 40/20/10 MHz (no WiFi) |
| Pins available on Breadboard | 1, 2, 3, 10, 11, 12, 13, 16, 17, 18, 43, 44 (total 12), 3.3V, 5V, GND |
| Pins available on solder pads | NO |
| Pins available internally | 0 (BOOT button), 14 (second button) and display (see below) |
| Pins for ST7789 | BL:38, powered by battery: set GPIO 15 to HIGH,  display pins see below, 80 MHz |
| Pins safe to use | ??? |
| Display | YES, ST7789 1.9-inches display, 8_Bit Parallel interface, 170x320 pixels, no touch controller |
| Interfaces | ?? 2x I2C, 2x SPI, 2x UART, 11x GPI0 (PWM), 4x ADC |
| Onboard Power LED | YES, green |
| Onboard GPIO LED | NO |
| USB-Connection | USB-C, no controller |
| Wi-Fi connector | PCB antenna |
| Wi-Fi | YES, 802.11 b/g/n (2.4 GHz), STA/AP/Mixed |
| Bluetooth Classic | YES, 5.0 |
| Bluetooth Low Energy (BLE) | YES, Bluetooth 5.0 LE protocols |
| Battery connector | YES JST 1.25 2P |
| Battery loading | YES |
| Battery voltage measure | YES GPIO 4 |
| Battery voltage measure control | NO |
| Extern voltage control | NO |
| Restart button | YES |
| BOOT button | YES, GPIO 0 |
| Second button | YES, GPIO 14 |
| On-/Off Switch | NO |
| SD card reader | NO |
| Breadboard pins | 2 * 12 pins |
| QWIIC connector | YES JST 1.00 4P, GND, 3.3V, GPIOs 43 + 44 |
| Internal temperature sensor | YES |
| Low Dropout Voltage Regulator (LDO) | LTH7 ( ??? mA) |
| Breadboard pins distance (width) | 2,3 cm (1 pin on each side available on a breadboard) |
| Security features | Encryption hardware accelerators that support AES-128/256, hashing, RSA, HMAC, digital signatures, and secure startup |
| Expansion board | NO |
| Arduino board selection | ESP32-S3 Dev Module |

### Display pin  profile

| Position | GPIO | 
|----------------------------------------|--|
| BL | 38 |
| Batt.Power | 15 |
| D0 | 39 |
| D1 | 40 |
| D2 | 41 |
| D3 | 42 |
| D4 | 45 |
| D5 | 46 |
| D6 | 47 |
| D7 | 48 |
| WR | 08 |
| RD | 09 |
| DC | 07 |
| CS | 06|
| RES | 05 |
