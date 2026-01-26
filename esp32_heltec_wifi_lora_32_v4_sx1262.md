---
layout: page
title: ESP32 Heltec Wifi LoRa 32 V4 SX1262
permalink: esp32_heltec_wifi_lora_32_v4_sx1262
---

> This is a Heltec ESP32 Dev. Board with assembled <b>SX1262 LoRa module</b> and <b>0.96-inches</b> OLED display with <b>I2C</b> interface and a resolution of <b>128 x 64 pixels</b> (no touch).

<b>Please note: as I'm located in Europe, the board needs to use the 868 MHz variant of the board !</b>

## Documentation

- [Heltec official manufacturer information](https://heltec.org/project/wifi-lora-32-v4/): https://heltec.org/project/wifi-lora-32-v4/
- [Arduino Heltec Boards](https://resource.heltec.cn/download/package_heltec_esp32_index.json): https://resource.heltec.cn/download/package_heltec_esp32_index.json (Version 3.0.3)
- [Quick start](https://wiki.heltec.org/docs/devices/open-source-hardware/esp32-series/esp32-quick-start?esp32=esp32): https://wiki.heltec.org/docs/devices/open-source-hardware/esp32-series/esp32-quick-start?esp32=esp32
- [GitHub](https://github.com/Heltec-Aaron-Lee/WiFi_Kit_series): https://github.com/Heltec-Aaron-Lee/WiFi_Kit_series
- [GitHub releases](https://github.com/Heltec-Aaron-Lee/WiFi_Kit_series/releases): https://github.com/Heltec-Aaron-Lee/WiFi_Kit_series/releases
- [Heltec library](https://github.com/HelTecAutomation/Heltec_ESP32): https://github.com/HelTecAutomation/Heltec_ESP32 version 2.1.5
- [Heltec Resources](https://resource.heltec.cn/download/WiFi_LoRa_32_V4/): https://resource.heltec.cn/download/WiFi_LoRa_32_V4/
- [Heltec Firmware (Meshtastic & more)](https://resource.heltec.cn/download/WiFi_LoRa_32_V4/firmware)
- [Heltec Community](http://community.heltec.cn/): http://community.heltec.cn/

## ESP32 Heltec WiFi LoRa 32 V4 pin mapping and schematic

- <img class="mx-auto w-1" src="{{site.baseurl}}/assets/img/pinout/esp32_s3_heltec_wifi_lora_32_v4_pinout_800w.png">
- [Schematic V4](/assets/pdf/schematic/esp32_s3_heltec_wifi_lora_32_v4_2_schematic.pdf) or [online](https://resource.heltec.cn/download/WiFi_LoRa_32_V4/Schematic)

## Libraries

The following libraries and version numbers are tested with this board:

- OLED: [esp8266-oled-ssd1306](https://github.com/ThingPulse/esp8266-oled-ssd1306) by ThingPulse version 4.6.1: https://github.com/ThingPulse/esp8266-oled-ssd1306
- LoRa: [SX12XX-LoRa](https://github.com/StuartsProjects/SX12XX-LoRa) by Stuart Projects version Oct 24, 2024: https://github.com/StuartsProjects/SX12XX-LoRa

## Development board profile

| Position | Characteristics | 
|----------------------------------------|--|
| Processor: | ESP32-S3R2 (Xtensa®32-bit lx7 dual core processor), Flash 16 MB, 2 MB PSRAM |
| CPU Frequencies | 240/160/80 MHz (for WiFi), 40/20/10 MHz (no WiFi) |
| Pins available on Breadboard | 0, 1, 2, 3, 4, 5, 6, 7, 19, 20, 21, 26, 33, 34, 35, 36, 37, 38, 39, 40, 41, 42, 43, 44, 45, 46, 47, 48  (total 28), RST, 3.3V 2*, 5V, 3.3V Vext 2*, GND 2* |
| Pins available on solder pads | 15, 16, 17, 18 |
| Pins available internally | 0 (BOOT button), LoRa module and display (see below) |
| Pins safe to use | ???  |
| Display | YES, SSD1336 0.96-inches display, I2C interface, 128x64 pixels, no touch controller |
| Interfaces | 2x I2C, 2x SPI, 3x UART, ??? 11x GPI0 (PWM), ??? 4x ADC |
| Onboard Power LED | YES (battery load control) |
| Onboard GPIO LED | YES |
| USB-Connection | USB-C, Controller: no |
| Wi-Fi connector | FPC antenna, alternative Ipex |
| Wi-Fi | YES, 802.11 b/g/n (2.4 GHz), STA/AP/Mixed |
| Bluetooth Classic | ??? YES, 5.0 |
| Bluetooth Low Energy (BLE) | YES, Bluetooth 5.0 LE protocols |
| LoRa antenna connector | Ipex |
| Battery connector | YES SH 1.25 2-pol |
| Battery loading | YES |
| Battery voltage measure | YES |
| Battery voltage measure control | YES |
| Extern voltage control | YES ("Vext") |
| Solar connector | YES SH 1.25 2-pol |
| Restart button | YES |
| BOOT button | YES, GPIO 0 |
| On-/Off Switch | NO |
| SD card reader | NO |
| Breadboard pins | 2 * 18 pins |
| QWIIC connector | NO |
| GNSS connector | YES, SH 1.25 8 pins |
| Internal temperature sensor | YES |
| Low Dropout Voltage Regulator (LDO) | CE6260 B33M (500 mA) |
| Breadboard pins distance (width) | ??? 2,3 cm (1 pin on each side available on a breadboard) |
| Security features | Encryption hardware accelerators that support AES-128/256, hashing, RSA, HMAC, digital signatures, and secure startup |
| Expansion board | NO |
| Arduino board selection | Heltec WiFi LoRa 32 (V2) |

### Display pin profile (I2C interface)

| Position | GPIO | 
|----------------------------------------|--|
| SDA | 17 |
| SCL | 18 |
| RST | 21 |

### LoRa module pin profile (SPI interface)

| Position | GPIO | 
|----------------------------------------|--|
| SS (CS) | 08 |
| MOSI | 10 |
| MISO | 11 |
| SCK | 09 |
| DIO0 | - |
| DIO1 | 14 |
| DIO2 | - |
| RST_LoRa | 12 |
| BUSY_LoRa | 13 |

### LED pin profile

| Position | GPIO | 
|----------------------------------------|--|
| LED | 35 |

### Vext control

| Position | GPIO | Comment | 
|----------------------------------------|--|--|
| Vext | 36 (LOW-ON,HIGH-OFF) | same as VBAT ctrl |

### Battery control

| Position | GPIO | Comment | 
|----------------------------------------|--|--|
| VBAT_CTRL | 37 |  |
| VBAT_ADC| 1 | |

#### GNSS / GPS control
| Position | GPIO | Comment | 
|----------------------------------------|--|--|
| VGNSS_Ctrl | 34 | |
| GNSS_TX | 39 | |
| GNSS_RX | 38 | |
| GNSS_WAKE | 40 | |
| GNSS_PPS | 41 | |
| GNSS_RST | 42 | |
