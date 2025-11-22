---
layout: page
title: ESP32-S3 Matrix (Waveshare)
permalink: esp32_s3_matrix
---

> This is an ESP32-S3 Dev. Board with assembled 8 x 8 WS2812 LED Matrix Board

<img class="mx-auto w-1" src="{{site.baseurl}}/assets/img/pinout/esp32_s3_matrix_pinout_800w.png">


## Documentation

Official documentation: https://www.waveshare.com/wiki/ESP32-S3-Matrix

## Development board profile

| Position | Characteristics | 
|----------------------------------------|--|
| Processor: | ESP32-S3 (ESP32-S3FH4R2 SoC with dual-core Xtensa LX7), Flash 4 MB, No PSRAM |
| CPU Frequencies | 160/160/80 MHz (for WiFi), 40/20/10 MHz (no WiFi) |
| Pins available on Breadboard | TX, RX, 1, 2, 3, 4, 5, 6, 7, 33, 34, 35, 36, 37, 38, 39, 40 (total 17), 3.3V, 5V, GND |
| Pins available on solder pads | GND, 5V, DOUT (WS2812 LED extension) |
| Pins available internally | 0 (BOOT button), 14 (WS2812 LED |
| Pins safe to use | 1, 2, 4, 5, 6, 7, 8, 15 (S), 16 (S), 17 (S), 18 (S), 21 (S)<br>(S) = soldered |
| Display | NO |
| Interfaces | 1x I2C, 1x SPI, 2x UART, 11x GPI0 (PWM), 4x ADC |
| Onboard Power LED | NO |
| Onboard GPIO LED | NO |
| Onboard GPIO LED-Bead 8x8 LEDs | YES, Color: RGB WS2812, GPIO: 14 |
| USB-Connection |USB-C, Controller: NO (emulated by SoC) |
| Wi-Fi connector | ceramic antenna |
| Wi-Fi | :white_check_mark:, 802.11 b/g/n (2.4 GHz), STA/AP/Mixed |
| Bluetooth Classic | :white_check_mark:, 5.0 |
| Bluetooth Low Energy (BLE) | :white_check_mark:, Bluetooth 5.0 LE protocols |
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
| Expansion board | :white_check_mark: Available, Feature: JT 2.0 Li-Ion Battery connector |
| Arduino board selection | ESP32S3 Dev Module |


