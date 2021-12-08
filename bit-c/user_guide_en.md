# BIT-C

## Pro Micro Compatible MCU with USB-C

![](https://github.com/nullbitsco/docs/raw/main/bit-c/user_guide_img/image000.jpg)

## User Guide

# Contents

[Helpful Links](#helpful_links)  
[Burning the Caterina (Arduino) Bootloader](#burning_bootloader)  
[Building for a Bit-C without flashing a new bootloader](#toolbox_flashing)

# <a name="helpful_links"></a> Helpful links

- [QMK Toolbox](https://github.com/qmk/qmk_toolbox)
- [Bit-C Pinout](https://nullbits.co/static/img/bit-c-legend.png)

## <a name="burning_bootloader"></a> Burning the Caterina (Arduino) bootloader

The Arduino IDE does not support programming the ATmega32U4 via the DFU bootloader, which is the default bootloader on the Bit-C. Fear not, though! Flashing the Caterina bootloader allows the Bit-C to be programmed directly from the Arduino IDE. This process is relatively straightforward and can be done directly from the Arduino IDE.

_Note: this can also be done over the command line, e.g. for Linux users, or using a Raspberry Pi instead of an Arduino, but those are more advanced and won't be covered here directly. [Hit up](https://bfy.tw/S9XQ) [the Googles](https://bfy.tw/S9XS) or pop into our [Discord server](https://discord.gg/eSegJcY) and ask if you're wondering about these or have a different setup._

### You'll need:

- A USB Arduino (Pro Micro, Uno, etc)
- The Arduino IDE, with the Sparkfun AVR board definitions installed

### Steps:

1. Configure the Arduino as an ISP

   An Arduino can be used an an “ISP programmer”. It’s a clever way of reusing an arduino instead of needing to buy or get ahold of a dedicated programmer.

   Sparkfun has a great tutorial on this. It’s a bit wordy, so don’t feel like you need to read the whole thing. The most important part is the one titled [“Option 2: Using the Arduino as a Programmer”](https://learn.sparkfun.com/tutorials/installing-an-arduino-bootloader).

1. Hook the Arduino up to the Bit-C

   The programming pins on the Bit-C are the same as a normal pro micro. Use [this link](https://www.coreforge.com/blog/2014/09/recovering-arduino-pro-micro-atmega32u4/) for reference.

1. Burn the bootloader

   Make sure to select the Sparkfun Pro Micro with ATmega32U4 (5V, 16MHz). Then, use Arduino IDE to [burn the bootloader](https://learn.sparkfun.com/tutorials/installing-an-arduino-bootloader#uploading-code---easy-way).

## <a name="toolbox_flashing"></a> Building for a Bit-C without flashing a new bootloader

It's also possible to build an Arduino sketch and then flash with QMK toolbox. The benefit of this is that the Bit-C doesn't need to be flashed with a new bootloader. Beware, though: complex code might not work as expected when using this method.

The below example shows how to compile a sketch within Arduino, and then flash using QMK Toolbox. It will blink the Bit-C LED at all 3 brightness levels @ 1Hz. The benefit of this is that you don't need to burn the Caterina bootloader.

Compile this with Arduino IDE for a 5V (16MHz) Pro Micro, and then export by choosing 'Sketch --> Export compiled Binary'

Point QMK toolbox to 'test.ino.promicro.hex' (the one WITHOUT the bootloader), reset the Bit-C into the DFU/bootloader mode, and flash.

https://gist.github.com/jaygreco/d82c83a441d5953b4c98d5e1aaebc104
