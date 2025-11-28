# ESP32 CYD ST7796 3.5 inches display: Pins

This page talks about the pins on the CYD. (Back to the device overview)[esp32_cyd_st7796_3_5_inches.md]

## Connector types

|Connector|Type    |Note                   |
|---      |---     |----                   |
|[**P1**](#p1)  |4P 1.25mm JST|Serial     |
|[**P3**](#p3)  |4P 1.25mm JST|GPIO       |
|[**P4**](#p4)  |2P 1.25mm JST|Speaker    |
|[**CN1**](#cn1)|4P 1.25mm JST|GPIO (I2C) |
|[**Battery**](#battery)  |2P 1.25mm JST|Battery |

## What pins are available on the CYD?

There are 3 easily accessible GPIO pins

|Pin|Location|Note|
|---|---|----|
|IO35|**P3** JST connector|Input only pin, no internal pull-ups available|
|IO22|**P3** and **CN1** JST connector||
|IO21|**CN1** JST connector||

If you need more than that, you need to start taking them from something else. An SD Card sniffer like mentioned in the [Add-ons](/ADDONS.md) is probably the next easiest.

After that you're probably de-soldering something!

## Broken Out Pins

There are three 4P 1.25mm JST connectors on the board

### P3
|Pin|Use|Note|
|---|---|----|
|GND|||
|IO35||Input only pin, no internal pull-ups available |
|IO22||Also on the **CN1** connector |
|IO21|| Also on the **CN1** connector |

### CN1
This is a great candidate for I2C devices

|Pin|Use|Note|
|---|---|----|
|GND|||
|IO22|| Also on **P3** connector |
|IO21|| Also on **P3** connector |
|3.3V|||

### P1
|Pin|Use|Note|
|---|---|----|
|VIN| 5V ||
|TX| IO1(?) | Maybe possible to use as a GPIO? |
|RX | IO3(?)| Maybe possible to use as a GPIO? |
|GND|||


## Buttons

The CYD has three buttons, reset, boot and switch 1.

|Pin|Use|Note|
|---|---|----|
|IO0|BOOT|Can be used as an input in sketches|

The behavior of switch 1 is unknown.

## Speaker

The speaker connector is a 2P 1.25mm JST connector that is connected to the amplifier, so not usable as GPIO at the speaker connector

|Pin|Use|Note|
|---|---|----|
|IO26|Connected to amp|`i2s_set_dac_mode(I2S_DAC_CHANNEL_LEFT_EN);`|

## Battery

The battery connector is a 2P 1.25mm JST connector that is connected to the LiIon load control.

## RGB LED

If your project requires additional pins to what is available elsewhere, this might be a good candidate to sacrifice.

Note: LEDs are "active low", meaning HIGH == off, LOW == on

|Pin|Use|Note|
|---|---|----|
|IO4|Red LED||
|IO16|Green LED||
|IO17|Blue LED||

## Display
Uses the HSPI

|Pin|Use|Note|
|---|---|----|
|IO2|TFT_RS|AKA: TFT_DC|
|IO12|TFT_SDO|AKA: TFT_MISO|
|IO13|TFT_SDI|AKA: TFT_MOSI|
|IO14|TFT_SCK||
|IO15|TFT_CS||
|IO27|TFT_BL||

## Touch Screen

|Pin|Use|Note|
|---|---|----|
|IO14|XPT2046_CLK||
|IO13|XPT2046_MOSI||
|IO33|XPT2046_CS||
|IO36|XPT2046_IRQ||
|IO12|XPT2046_MISO||

## SD Card
Uses the VSPI
Pin names are predefined in SPI.h

|Pin|Use|Note|
|---|---|----|
|IO5|SS (CS)||
|IO18|SCK||
|IO19|MISO||
|IO23|MOSI||

## LDR (Light Sensor)

|Pin|Use|Note|
|---|---|----|
|IO34|||

(Back to the device overview)[esp32_cyd_st7796_3_5_inches.md]
