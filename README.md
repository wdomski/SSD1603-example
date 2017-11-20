# SSD1603-example
Example for STM32 HAL driver for for I2C OLED SSD1603 display with U8glib

This is an example project for I2C OLED SSD1603 display with U8glib.
It includes the driver. The driver itself can be found in [SSD1603](https://github.com/wdomski/SSD1603) 
repository.

The example was prepared under SW4STM32 for STM32F103C8T6 development board 
and can be easily ported to any other device. Also STM32CubeMX configuration 
file is included.

# How to use it

## Prerequisite
You need a board equipped with STM32F103C8T6 MCU and a SSD1603 display with I2C interface.

## Connecting display

The module has to be connected with the MCU board 
with following pins:

| MCU pin | SX1278 pin | Description |
| ------- | ---------- | ----------- |
| PB7     | SDA        | I2C SDA     |
| PB6     | SCL        | I2C SCL     |
| ------- | ---------- | ----------- |
| VDD     | VCC        | +3V3        |
| VSS     | GND        | GND         |

Remember to pull--up the SDA and SCL line. One resistor of value 4k7 Ohm will be sufficient.

## Compilation
You have to compile it under SW4STM32 or import it into i.e. TrueSTUDIO - Atollic.

## Run
The display will show a simple text.

# Final remarks

You can visit [my blog](http://blog.domski.pl) to read more about the SSD1603 display or my other projects.
