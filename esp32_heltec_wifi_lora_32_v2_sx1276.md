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
- [Heltec Community](http://community.heltec.cn/): http://community.heltec.cn/

## ESP32 Heltec WiFi LoRa 32 V2 pin mapping and schematic

As there is a V2 and V2.1 variant, all data is available for both variants:

### ESP32 Heltec WiFi LoRa 32 V2 variant

- <img class="mx-auto w-1" src="{{site.baseurl}}/assets/img/pinout/esp32_heltec_wifi_lora_32_v2_868-915_pinout_800w.png"> or as [PDF](https://resource.heltec.cn/download/WiFi_LoRa_32/WIFI_LoRa_32_V2.pdf)
- [Schematic V2](/assets/pdf/schematic/esp32_heltec_wifi_lora_32_v2_868-915_schematic.pdf)

### ESP32 Heltec WiFi LoRa 32 V2.1 variant

- <img class="mx-auto w-1" src="{{site.baseurl}}/assets/img/pinout/esp32_heltec_wifi_lora_32_v2_1_868-915_pinout_800w.png"> or as [PDF](https://resource.heltec.cn/download/WiFi_LoRa_32/WIFI_LoRa_32_V2.1.pdf)
- [Schematic V2.1](/assets/pdf/schematic/esp32_heltec_wifi_lora_32_v2_1_868-915_schematic.pdf)

## Libraries

The following libraries and version numbers are tested with this board:

- OLED: [esp8266-oled-ssd1306](https://github.com/ThingPulse/esp8266-oled-ssd1306) by ThingPulse version 4.6.1: https://github.com/ThingPulse/esp8266-oled-ssd1306
- LoRa: [SX12XX-LoRa](https://github.com/StuartsProjects/SX12XX-LoRa) by Stuart Projects version Oct 24, 2024: https://github.com/StuartsProjects/SX12XX-LoRa

## Development board profile

| Position | Characteristics | 
|----------------------------------------|--|
| Processor: | ESP32 module with dual-core Xtensa LX7 (ESP32-D0), Flash 4 MB, no PSRAM |
| CPU Frequencies | 240/160/80 MHz (for WiFi), 40/20/10 MHz (no WiFi) |
| Pins available on Breadboard | 0, 1, 2, 3, 4, 5, 12, 13, 14, 15, 16, 17, 21, 22, 23, 25, 26, 32, 33, input only: 34, 35, 36, 37, 38, 39 (total 28), RST, 3.3V 2*, 5V, 3.3V Vext 2*, GND 2* |
| Pins available on solder pads | NO |
| Pins available internally | 0 (BOOT button), LoRa module and display (see below) |
| Pins safe to use | ??? 12, [13 not on V2], 17, 18, 19, 22, 27, 32, 33, input only: 36, 39 |
| Display | YES, SSD1336 0.96-inches display, I2C interface, 128x64 pixels, no touch controller |
| Interfaces | 2x I2C, 2x SPI, 2x UART, 11x GPI0 (PWM), 4x ADC |
| Onboard Power LED | YES (battery load control) |
| Onboard GPIO LED | YES |
| USB-Connection | Micro-USB, Controller: CP2102 |
| Wi-Fi connector | Spiral antenna |
| Wi-Fi | YES, 802.11 b/g/n (2.4 GHz), STA/AP/Mixed |
| Bluetooth Classic | YES, 5.0 |
| Bluetooth Low Energy (BLE) | YES, Bluetooth 5.0 LE protocols |
| Battery connector | YES |
| Battery loading | YES |
| Battery voltage measure | YES |
| Battery voltage measure control | YES |
| Extern voltage control | YES ("Vext") |
| Restart button | YES |
| BOOT button | YES, GPIO 0 |
| On-/Off Switch | NO |
| SD card reader | NO |
| Breadboard pins | 2 * 18 pins |
| QWIIC connector | NO |
| Internal temperature sensor | YES |
| Low Dropout Voltage Regulator (LDO) | CE6260 (500 mA) |
| Breadboard pins distance (width) | 2,3 cm (1 pin on each side available on a breadboard) |
| Security features | Encryption hardware accelerators that support AES-128/256, hashing, RSA, HMAC, digital signatures, and secure startup |
| Expansion board | NO |
| Arduino board selection | Heltec WiFi LoRa 32 (V2) |

### Display pin profile (I2C interface)

| Position | GPIO | 
|----------------------------------------|--|
| SDA | 4 |
| SCL | 15 |
| RST | 16 |

### LoRa module pin profile (SPI interface)

| Position | GPIO | 
|----------------------------------------|--|
| SS (CS) | 18 |
| MOSI | 27 |
| MISO | 19 |
| SCK | 5 |
| DIO0 | 26 |
| DIO1 | 35 |
| DIO1 | 34 |
| RST_LoRa | 14 |

### LED pin profile

| Position | GPIO | 
|----------------------------------------|--|
| LED | 25 |

### Vext control

| Position | GPIO | Comment | 
|----------------------------------------|--|--|
| Vext | 21 (LOW-ON,HIGH-OFF) | same as VBAT ctrl |

### Battery control

| Position | GPIO | Comment | 
|----------------------------------------|--|--|
| VBAT_CTRL | 21 | same as Vext ctrl |
| VBAT_ADC| 13 | Version 2 |
| VBAT_ADC| 37 | Version 2.1 |
