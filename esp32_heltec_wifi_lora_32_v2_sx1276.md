---
layout: page
title: ESP32 Heltec Wifi LoRa 32 V2 SX1276
permalink: esp32_heltec_wifi_lora_32_v2_sx1276
---

> This is a Heltec ESP32 Dev. Board with assembled <b>SX1276 LoRa module</b> and <b>0.96-inches</b> OLED display with <b>I2C</b> interface and a resolution of <b>128 x 64 pixels</b> (no touch).

<b>Please note: as I'm located in Europe, the board needs to use the 868 MHz variant of the board !</b>

## Documentation

- The official documentation is no longer available as the product is outphased
- [Arduino Heltec Boards](https://resource.heltec.cn/download/package_heltec_esp32_index.json): https://resource.heltec.cn/download/package_heltec_esp32_index.json (Version 3.0.3)
- [Quick start](https://wiki.heltec.org/docs/devices/open-source-hardware/esp32-series/esp32-quick-start?esp32=esp32): https://wiki.heltec.org/docs/devices/open-source-hardware/esp32-series/esp32-quick-start?esp32=esp32
- [GitHub](https://github.com/Heltec-Aaron-Lee/WiFi_Kit_series): https://github.com/Heltec-Aaron-Lee/WiFi_Kit_series
- [GitHub releases](https://github.com/Heltec-Aaron-Lee/WiFi_Kit_series/releases): https://github.com/Heltec-Aaron-Lee/WiFi_Kit_series/releases
- [Heltec library](https://github.com/HelTecAutomation/Heltec_ESP32): https://github.com/HelTecAutomation/Heltec_ESP32 version 2.1.5
- [Heltec Resources](https://resource.heltec.cn/download/WiFi_LoRa_32/V2): https://resource.heltec.cn/download/WiFi_LoRa_32/V2

## ESP32 Heltec WiFi LoRa 32 V2 pin mapping and schematic
- <img class="mx-auto w-1" src="{{site.baseurl}}/assets/img/pinout/heltec_wireless_stick_v3_lora_pinout_600w.png">
- [Schematic](/assets/pdf/schematic/esp32_heltec_wifi_lora_32_v2_868-915_schematic.pdf)

## Libraries

The following libraries and version numbers are tested with this board:


## Development board profile

| Position | Characteristics | 
|----------------------------------------|--|
| Processor: | ESP32-S3 processor with dual-core Xtensa LX7 (ESP32-S3FN8, Flash 8 MB, NO PSRAM |
| CPU Frequencies | 240/160/80 MHz (for WiFi), 40/20/10 MHz (no WiFi) |
| Pins available on Breadboard | 1, 2, 3, 10, 11, 12, 13, 16, 17, 18, 43, 44 (total 12), 3.3V, 5V, GND |
| Pins available on solder pads | NO |
| Pins available internally | 0 (BOOT button), 14 (second button) and display (see below) |
| Pins for ??ST7789 | BL:38, powered by battery: set GPIO 15 to HIGH,  display pins see below, 80 MHz |
| Pins safe to use | ??? |
| Display | YES, ST7789 1.9-inches display, 8_Bit Parallel interface, 170x320 pixels, no touch controller |
| Interfaces | ?? 2x I2C, 2x SPI, 2x UART, 11x GPI0 (PWM), 4x ADC |
| Onboard Power LED | YES, white |
| Onboard GPIO LED | YES, Orange |
| USB-Connection | USB-C, CP2102 USB controller |
| Wi-Fi connector | PCB antenna |
| Wi-Fi | YES, 802.11 b/g/n (2.4 GHz), STA/AP/Mixed |
| Bluetooth Classic | YES, 5.0 |
| Bluetooth Low Energy (BLE) | YES, Bluetooth 5.0 LE protocols |
| Battery connector | YES JST 1.25 2P |
| Battery loading | YES |
| Battery voltage measure | YES GPIO 1 |
| Battery voltage measure control | YES GPIO 37 |
| Extern voltage control | YES GPIO 36 |
| Restart button | YES |
| BOOT button | YES, GPIO 0 |
| On-/Off Switch | NO |
| SD card reader | NO |
| Breadboard pins | 2 * 17 pins |
| QWIIC connector | NO |
| Internal temperature sensor | YES |
| Low Dropout Voltage Regulator (LDO) | LTH7 ( ??? 500 mA) |
| Breadboard pins distance (width) | 2,8 cm (1 pin on each side available on a breadboard) |
| Security features | Encryption hardware accelerators that support AES-128/256, hashing, RSA, HMAC, digital signatures, and secure startup |
| Expansion board | NO |
| Arduino board selection | ESP32-S3 Dev Module |

### Display pin profile (I2C interface)

| Position | GPIO | 
|----------------------------------------|--|
| SDA | 18 |
| SCL | 18 |
| RST | 21 |

### LoRa module pin profile (SPI interface)

| Position | GPIO | 
|----------------------------------------|--|
| SS (CS) | 8 |
| MOSI | 10 |
| MISO | 11 |
| SCK | 9 |
| DIO1 | 14 |
| RST_LoRa | 12 |
| BUSY_LoRa | 13 |

### LED pin profile

| Position | GPIO | 
|----------------------------------------|--|
| LED | 35 |

### Vext control

| Position | GPIO | 
|----------------------------------------|--|
| Vext | 36 |

### Battery control

| Position | GPIO | 
|----------------------------------------|--|
| VBAT_CTRL | 37 |
| VBAT_ADC| 1 |
