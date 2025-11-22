---
layout: page
title: ESP32-S3 Matrix (Waveshare)
permalink: esp32_s3_matrix
---

> This is an ESP32-S3 Dev. Board with assembled <b>8 x 8 WS2812 LED Matrix</b> Board and <b>QMI8656 6-axis sensor</b> (3-axis accelerometer and 3-axis gyroscope)

<img class="mx-auto w-1" src="{{site.baseurl}}/assets/img/pinout/esp32_s3_matrix_pinout_800w.png">

## Documentation

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
| Processor: | ESP32-S3 (ESP32-S3FH4R2 SoC with dual-core Xtensa LX7), Flash 4 MB, No PSRAM |
| CPU Frequencies | 160/160/80 MHz (for WiFi), 40/20/10 MHz (no WiFi) |
| Pins available on Breadboard | TX (43), RX (44), 1, 2, 3, 4, 5, 6, 7, 33, 34, 35, 36, 37, 38, 39, 40 (total 17), 3.3V, 5V, GND |
| Pins available on solder pads | GND, 5V, DOUT (WS2812 LED extension) |
| Pins available internally | 0 (BOOT button), 14 (WS2812 LED) |
| Pins safe to use | 1, 2, 4, 5, 6, 7, 33, 34, 35, 36, 37, 38, 39, 40 |
| Display | NO |
| Interfaces | 1x I2C, 1x SPI, 2x UART, 11x GPI0 (PWM), 4x ADC |
| Onboard Power LED | NO |
| Onboard GPIO LED | NO |
| Onboard GPIO LED-Bead 8x8 LEDs | YES, Color: RGB WS2812, **GPIO: 14** |
| QMI8656 6-axis sensor | Interface: **I2C**, **I2C_SDA: 11, I2C_SCL: 12** |
| USB-Connection |USB-C, Controller: NO (emulated by SoC) |
| Wi-Fi connector | ceramic antenna |
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
| Breadboard pins | 2 * 10 pins |
| QWIIC connector | NO |
| Internal temperature sensor | YES |
| Low Dropout Voltage Regulator (LDO) | ME6217 (800 mA) |
| Security features | Encryption hardware accelerators that support AES-128/256, hashing, RSA, HMAC, digital signatures, and secure startup |
| Expansion board | NO |
| Arduino board selection | ESP32S3 Dev Module |


