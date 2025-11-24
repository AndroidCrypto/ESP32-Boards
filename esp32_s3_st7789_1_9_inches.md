---
layout: page
title: ESP32-S3 ST7789 1.9-inches display
permalink: esp32_s3_st7789_1_9_inches
---

> This is an ESP32-S3 Dev. Board with assembled <b>ST7789 1.9-inches</b> TFT display with <b>SPI</b> interface and a resolution of <b>170 x 320 pixels</b> (no touch).

## Documentation

There is no documentation available for this board. I tried to get the schematic or pinout of the TFT display but no success. In the end, it is just an ESP32-S3 board without any chance to use the display.

## Libraries

n/a

## Development board profile

<b>Please note: the following data are not correct !!</b>

| Position | Characteristics | 
|----------------------------------------|--|
| Processor: | ESP32-S3 processor with dual-core Xtensa LX7 (ESP32-D0WD-V3 (revision v3.1)), Flash 16 MB, 8 MB PSRAM |
| CPU Frequencies | 240/160/80 MHz (for WiFi), 40/20/10 MHz (no WiFi) |
| Pins available on Breadboard | 0, 4, 5, 12, 16, 17, 18, 19, 21, 22, 23, 25, 26, 27, 32, 33, input only: 34, 35, 36, 39 (total 20), 3.3V, 5V, GND |
| Pins available on solder pads | NO |
| Pins available internally | 0 (BOOT button) and display (see below) |
| Pins for ST7789 | BL:21, MISO: n/c, MOSI: 13, SCLK: 14, CS: 15, DC: 2, RST -1, HSPI-port, 80 MHz |
| Pins safe to use | 4, 5, 12, 16, 17, 18, 19, 22, 23, 25, 26, 27, 32, 33, input only: 34, 35, 36, 39 |
| Display | YES, ST7789 1.9-inches display, SPI interface, 170x320 pixels, no touch controller |
| Interfaces | 1x I2C, 2x SPI, 2x UART, 11x GPI0 (PWM), 4x ADC |
| Onboard Power LED | YES, blue |
| Onboard GPIO LED | NO |
| USB-Connection | USB-C, no controller |
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
| Second button | YES, GPIO 14 |
| On-/Off Switch | NO |
| SD card reader | NO |
| Breadboard pins | 2 * 12 pins |
| QWIIC connector | NO |
| Internal temperature sensor | YES |
| Low Dropout Voltage Regulator (LDO) | LTH7 ( ??? mA) |
| Breadboard pins distance (width) | 3,0 cm (does not fit on one breadboard) |
| Security features | Encryption hardware accelerators that support AES-128/256, hashing, RSA, HMAC, digital signatures, and secure startup |
| Expansion board | NO |
| Arduino board selection | ESP32 Dev Module |
