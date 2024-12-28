## https://docs.m5stack.com/en/core/m5stickc


## Description
M5StickC is a mini M5Stack, powered by ESP32. It is a portable, easy-to-use, open source, IoT development board. What it can do? This tiny block is able to realize your idea, enlighten your creativity, and help with your IoT prototyping in a very short time. It will take away a lot of pains from the development process.M5stickC is one of the core devices in M5Stack product series.

It is built in a continually growing hardware and software ecosystem. It has a lot of compatible modules and units, as well as the open source code & engineering communities that will help you maximize your benefits in every step of the developing process.

Power switch operation:

Power on :Press power button for 2 seconds

Power off :Press power button for 6 seconds

The input range of VBUS_VIN and VBUS_USB is limited to 4.8-5.5V, and the internal battery will be charged through AXP192 power management when VBUS is powered.

Notice:

Baud rate supported by M5StickC: 1200 ~115200, 250K, 500K, 750K, 1500K

### Features
* ESP32-based
* Built-in 6-Axis IMU
* Red LED
* IR transmitter
* Microphone
* Buttons, LCD(0.96 inch)
* Built-in Lithium Polymer Battery
* Extendable Socket
* Wearable & Wall mounted
* Compatible with multi-platform development:
    * UIFlow
    * MicroPython
    * Arduino
    * .NET nanoFramework

## Specifications

| Resources | Parameter |
| --- | --- |
| ESP32 |	240MHz dual core, 600 DMIPS, 520KB SRAM, Wi-Fi
| Flash Memory | 4MB |
| Power Input | 5V @ 500mA |
| Port	| TypeC x 1, GROVE(I2C+I/0+UART) x 1 |
| LCD screen | 0.96 inch, 80*160 Colorful TFT LCD, ST7735S |
| Button | Custom button x 2 |
| LED	| RED LED |
| MEMS	| MPU6886 |
| IR	| Infrared transmission |
| MIC	| SPM1423 |
| RTC	| BM8563 |
| PMU	| AXP192 |
| Battery	| 95 mAh @ 3.7V |
| Antenna	| 2.4G 3D Antenna |
| PIN port	|G0, G26, G36 |

## Pin Map

**RED LED & IR Transmitter & BUTTON A & BUTTON B**

| ESP32 | GPIO10 | GPIO9 | GPIO37 | GPIO39 |
| --- | --- | --- | --- | --- |
| RED LED | LED Pin |  |  |  |
| IR Transmitter |  | Transmitter Pin |  |  |
| BUTTON A |  |  | Button Pin |  |
| BUTTON B |  |  |  | Button Pin |

**TFT LCD**

Driver IC:ST7735S

Resolution:80 \* 160

| ESP32 | GPIO15 | GPIO13 | GPIO23 | GPIO18 | GPIO5 |
| --- | --- | --- | --- | --- | --- |
| TFT LCD | TFT\_MOSI | TFT\_CLK | TFT\_DC | TFT\_RST | TFT\_CS |

**GROVE PORT**

| ESP32 | GPIO33 | GPIO32 | 5V | GND |
| --- | --- | --- | --- | --- |
| GROVE port | SCL | SDA | 5V | GND |

**MIC (SPM1423)**

| ESP32 | GPIO0 | GPIO34 |
| --- | --- | --- |
| MICPHONE | CLK | DATA |

**6-Axis posture sensor (SH200Q/MPU6886) & power management IC (AXP192) & RTC (BM8563)**

| ESP32 | G21 | G22 | G35 |
| --- | --- | --- | --- |
| AXP192 | SDA | SCL | IRQ |
| MPU6886 | SDA | SCL | IRQ |
| BM8563 | SDA | SCL | IRQ |

**AXP192**

| Microphone | RTC | TFT backlight | TFT IC | ESP32/3.3V MPU6886/SH200Q | 5V GROVE |
| --- | --- | --- | --- | --- | --- |
| LDOio0 | LDO1 | LDO2 | LDO3 | DC-DC1 | IPSOUT |

**Charging current measured value**

| charging current | Fully charged current(Power OFF) | Fully charged current(Power ON） |
| --- | --- | --- |
| 0.488A | 0.066A | 0.181A |