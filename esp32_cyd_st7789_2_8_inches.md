---
layout: page
title: ESP32 CYD ST7789 2.8-inches resistive touch display
permalink: esp32_cyd_st7789_2_8_inches
---

> This is an ESP32 Dev. Board with assembled <b>ST7789 2.8-inches</b> TFT display with <b>SPI</b> interface that has a resolution of <b>240 x 320 pixels</b> and <b>resistive touch surface (driver chip XPT2046)</b>. It is known as <b>Cheap Yellow Display ("CYD")</b> and comes in several variants. Additionally, a Micro-SD-Card reader and a (true) RGB LED is on the backside of the device. There is an LDR Light sensor assembled on the front side, but a lot of people marked them as not working or useless (I did not verify this).

<font color="red">Please note that there are no breadboard pins that expose GPIO pins, instead there are 3 JST 1.25 connectors available.</font>

## Variants of CYD devices

- the first two versions are using a TFT display with driver chip ILI9341 and come with a Micro-USB connector (link to the description)
- the third version (this descriptions) is using the display with attached ST7789 driver chip. These devices do have a Micro-USB and a USB-C connector.

### wrong <img class="mx-auto w-1" src="{{site.baseurl}}/assets/img/pinout/esp32_st7789_1_9_inches_pinout_594w.png">

## Documentation

This board is well documentated by the manufacturer and third party persons:

- Developer website: this specific device has the “device number” “ESP32–2432S028R”, that was developed by a Chinese company. Their website is difficult to find, here is a link to the [folder (containing all models)](http://pan.jczn1688.com/1/ESP32%20module) and the [specific product file](http://pan.jczn1688.com/directlink/1/ESP32%20module/2.8inch_ESP32-2432S028R.rar). You will download a file of about 900 MB size!
- Probably the best website about the CYD is from a hobbyist, “witnessmenow” (Brian Lough), who maintains the GitHub repository “[ESP32-Cheap-Yellow-Display](https://github.com/witnessmenow/ESP32-Cheap-Yellow-Display)” with a lot of FAQs and troubleshooting around CYD
- Another source for examples is “[https://github.com/bitbank2/CYD_Projects](https://github.com/bitbank2/CYD_Projects)”
- Sara and Rui Santos have a phantastic website around ESP32 topics, and they give a lot of information and examples, e.g. “[Getting Started with ESP32 Cheap Yellow Display Board — CYD (ESP32–2432S028R)](https://randomnerdtutorials.com/cheap-yellow-display-esp32-2432s028r/)” and “[ESP32 Cheap Yellow Display (CYD) Pinout (ESP32–2432S028R](https://randomnerdtutorials.com/esp32-cheap-yellow-display-cyd-pinout-esp32-2432s028r/))”. Use their search for more tutorials on this device.

## Own tutorials

I wrote some tutorials regarding this device:

- [Create a colorful digital clock on an ESP32 Cheap Yellow Display (“CYD”)](https://medium.com/@androidcrypto/create-a-colorful-digital-clock-on-an-esp32-cheap-yellow-display-cyd-641db4642e47)
- [Create an Internet Weather Station with 3 days Forecast on an ESP32 Cheap Yellow Display (“CYD”)](https://medium.com/@androidcrypto/create-an-internet-weather-station-with-3-days-forecast-on-an-esp32-cheap-yellow-display-cyd-15eb5c353b1d)
- [How to use Touch and SD Card at the same time on an ESP32 Cheap Yellow Display (“CYD”)](https://medium.com/@androidcrypto/how-to-use-touch-and-sd-card-at-the-same-time-on-an-esp32-cheap-yellow-display-cyd-45fa55d01ffe)
- [Play iconic Arcade Games like Pac-Man or Donkey Kong on ESP32 Cheap Yellow Display (“CYD”) [full guide]](https://medium.com/@androidcrypto/play-iconic-arcade-games-like-pac-man-or-donkey-kong-on-esp32-cheap-yellow-display-cyd-full-899321881f28)
- [Create a digital clock in a Domino style on an ESP32 Cheap Yellow Display (“CYD”)](https://medium.com/@androidcrypto/create-a-digital-clock-in-a-domino-style-on-an-esp32-cheap-yellow-display-cyd-b9e9a784ac21)
- [Playing Othello / Reversi on an ESP32 Cheap Yellow Display with Minimax intelligence for the AI opponent](https://medium.com/@androidcrypto/playing-othello-reversi-on-an-esp32-cheap-yellow-display-with-minimax-intelligence-for-the-ai-07394729e653)
- 

## Libraries

The following libraries and version numbers are tested with this board:

- **TFT_eSPI** by Bodmer, version 2.5.43, [https://github.com/Bodmer/TFT_eSPI](https://github.com/Bodmer/TFT_eSPI)
- **LovyanGFX** by Lovyan03, version 1.2.7, [https://github.com/lovyan03/LovyanGFX](https://github.com/lovyan03/LovyanGFX)

## Development board profile

### wrong

| Position | Characteristics | 
|----------------------------------------|--|
| Processor: | ESP32 module with dual-core Xtensa LX7 (ESP32-D0WD-V3 (revision v3.1)), Flash 4 MB, no PSRAM |
| CPU Frequencies | 160/160/80 MHz (for WiFi), 40/20/10 MHz (no WiFi) |
| Pins available on Breadboard | 0, 4, 5, 12, 16, 17, 18, 19, 21, 22, 23, 25, 26, 27, 32, 33, input only: 34, 35, 36, 39 (total 20), 3.3V, 5V, GND |
| Pins available on solder pads | NO |
| Pins available internally | 0 (BOOT button) and display (see below) |
| Pins for ST7789 | BL: 21, MISO: n/c, MOSI: 13, SCLK: 14, CS: 15, DC: 2, RST -1, HSPI-port, 80 MHz |
| Pins for XPT2046 Touch Controller | MISO: 39, MOSI: 32, SCLK: 25, SS/CS: 33, IRQ: 36 |
| Pins for Micro-SD-Card reader | MISO: 19, MOSI: 23, SCLK: 18, SS/CS: 5 |
| Pins safe to use | 22,27 and 35 (input only) on CN1 |
| Display | YES, ST7789 1.9-inches display, SPI interface, 170x320 pixels, no touch controller |
| Interfaces | 1x I2C, 2x SPI, 2x UART, 11x GPI0 (PWM), 4x ADC |
| Onboard Power LED | NO |
| Onboard GPIO LED | RGB LED, red: 4, green: 16, blue: 17 |
| USB-Connection | USB-C and Micro-USB, Controller: CH340 |
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
| SD card reader | YES |
| Breadboard pins | NO pins but some 1.25 JST connectors |
| QWIIC connector | NO |
| Internal temperature sensor | YES |
| Low Dropout Voltage Regulator (LDO) | AMS1117 (1000 mA) |
| Breadboard pins distance (width) | 3,0 cm (does not fit on one breadboard) |
| Security features | Encryption hardware accelerators that support AES-128/256, hashing, RSA, HMAC, digital signatures, and secure startup |
| Expansion board | NO |
| Arduino board selection | ESP32 Dev Module |
