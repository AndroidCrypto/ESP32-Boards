---
layout: page
title: ESP32 T-Display ST7789 1.14-inches display
permalink: esp32_t_display_st7789_1_14_inches
---

> This is a LilyGo ESP32 Dev. Board with assembled <b>ST7789 1.14-inches</b> TFT display with <b>SPI</b> interface and a resolution of <b>135 x 240 pixels</b> (no touch).

## Documentation

- [Inofficial board overview](https://done.land/components/microcontroller/families/esp/esp32/developmentboards/esp32s/t-display/)
- [LilyGo shop](https://lilygo.cc/products/t-display?_pos=1&_psq=t-display&_ss=e&_v=1.0)
- [LilyGo GitHub repository](https://github.com/Xinyuan-LilyGO/TTGO-T-Display)

## ESP32 T-Display pin mapping and schematic
- <img class="mx-auto w-1" src="{{site.baseurl}}/assets/img/pinout/esp32_lilygo_t_display_pinout_800w.png">
- [Schematic](/assets/pdf/schematic/esp32_lilygo_t_display_schematic.pdf) or [online](https://github.com/Xinyuan-LilyGO/TTGO-T-Display/blob/master/schematic/ESP32-TFT(6-26).pdf)

## Libraries

The following libraries and version numbers are tested with this board:

- Adafruit ST7735 & ST7789 by Adafruit, version 1.11.0, https://github.com/adafruit/Adafruit-ST7735-Library
- TFT_eSPI by Bodmer, version 2.5.43, https://github.com/Bodmer/TFT_eSPI
- LovyanGFX by Lovyan03, version 1.2.7, https://github.com/lovyan03/LovyanGFX

## Development board profile

| Position | Characteristics | 
|----------------------------------------|--|
| Processor: | ESP32 processor with dual-core Xtensa LX6, Flash 4/16 MB, 0 MB PSRAM |
| CPU Frequencies | 240/160/80 MHz (for WiFi), 40/20/10 MHz (no WiFi) |
| Pins available on Breadboard | 2, 12, 13, 15, 17, 21, 22, 25, 26, 27, 32, 33, 36 (I), 37 (I), 38 (I), 39 (I) (total 16), 3.3V 2*, 5V, GND 5* |
| Pins available on solder pads | NO |
| Pins available internally | 0 (BOOT button), 14 (second button) and display (see below) |
| Pins for ST7789 | BL:4, display pins see below, 80 MHz |
| Pins safe to use | ??? |
| Display | YES, ST7789 1.14-inches display, SPI interface, 135x240 pixels, no touch controller |
| Interfaces | ?? 2x I2C, 2x SPI, 2x UART, 12x GPI0 (PWM), 11x ADC |
| Onboard Power LED | YES (battery load control) blue |
| Onboard GPIO LED | NO |
| USB-Connection | USB-C, CH9102 |
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
| Second button | YES, GPIO 35 |
| On-/Off Switch | NO |
| SD card reader | NO |
| Breadboard pins | 2 * 12 pins |
| QWIIC connector | NO |
| Internal temperature sensor | YES |
| Low Dropout Voltage Regulator (LDO) | AP2112K-3.3V( RT9013) (500 mA) |
| Breadboard pins distance (width) | 2,3 cm (1 pin on each side available on a breadboard) |
| Security features | Encryption hardware accelerators that support AES-128/256, hashing, RSA, HMAC, digital signatures, and secure startup |
| Expansion board | NO |
| Arduino board selection | ESP32 Dev Module |

### Display pin profile

| Position | GPIO | 
|----------------------------------------|--|
| BL | 4 |
| MOSI | 19 |
| SCLK | 18 |
| DC | 16 |
| CS | 05|
| RES | 23 |

### Battery pin

| Position | GPIO | 
|----------------------------------------|--|
| Batt.Power | 34 |
