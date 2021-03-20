# SCRAMBLE

## 6-Key Functional Switch Tester
![](https://github.com/nullbitsco/docs/raw/main/scramble/user_guide_img/image000.jpg)
## User Guide

# Contents
[Helpful Links](#helpful_links)  
[Quickstart Guide](#quickstart_guide)  
[Firmware Flashing](#firmware_flashing)  

# <a name="helpful_links"></a> Helpful links
* VIA software download link: https://caniusevia.com
* VIA demo video: https://www.youtube.com/watch?v=WZKf2TvUZ7Q
* VIA guide: https://keyboard.university/guides/using-via-configurator
* SCRAMBLE QMK firmware & source code: https://github.com/qmk/qmk_firmware/tree/master/keyboards/nullbitsco/scramble

# <a name="quickstart_guide"></a> Quickstart Guide

## Plug in SRAMBLE
Plug SCRAMBLE into your computer using the provided USB cable.

Open up a blank Word document and press each key. You should get an output of each switch’s description.

## Customizing your SCRAMBLE
To customize your SCRAMBLE keys, download VIA from https://caniusevia.com/

With your SCRAMBLE plugged into your computer, open VIA. The SCRAMBLE will be recognized. You can now program your SCRAMBLE.

## Default Switch Layout (USB on left)
| | | |
| --- | --- | --- |
| Clear | Red | Black |
| ![](https://github.com/nullbitsco/docs/raw/main/scramble/user_guide_img/image004.jpg) | ![](https://github.com/nullbitsco/docs/raw/main/scramble/user_guide_img/image006.jpg) | ![](https://github.com/nullbitsco/docs/raw/main/scramble/user_guide_img/image001.jpg) |
| Brown | Blue | Green |
| ![](https://github.com/nullbitsco/docs/raw/main/scramble/user_guide_img/image003.jpg) | ![](https://github.com/nullbitsco/docs/raw/main/scramble/user_guide_img/image002.jpg) | ![](https://github.com/nullbitsco/docs/raw/main/scramble/user_guide_img/image005.jpg) |

## Default output of each switch when pressed  
Gateron White: Linear, 35g force  
Gateron White: Linear, 35g force  
Gateron Red: Linear, 45g force  
Gateron Black: Linear, 60g force  
Gateron Brown: Tactile, 55g force  
Gateron Blue: Clicky, 60g force  
Gateron Green: Clicky, 80g force  

# <a name="firmware_flashing"></a> Flashing Firmware
The ATmega328P uses a fork of [USBaspLoader](https://github.com/nullbitsco/USBaspLoader) as the bootloader. The bootloader is in a protected code region so there is a low risk of damaging or overwriting it. You can build firmware using the [QMK Configurator](https://config.qmk.fm/#/nullbitsco/scramble/LAYOUT), but note that it does not support changing encoder or OLED functionality (yet).

## Entering bootloader mode
To enter the bootloader, start with the SCRAMBLE unplugged from USB. With the SCRAMBLE positioned so the USB connector is on the left, hold the green (lower-right) switch and plug into the PC. The LED will stay on, indicating it is in bootloader mode. If it worked, you should see a new USBAsp device in QMK Toolbox. 

![](https://github.com/nullbitsco/docs/raw/main/scramble/user_guide_img/image007.png)

## Flashing new firmware
Before flashing, make sure that "atmega328p" is selected under the "MCU (AVR only)" menu in QMK toolbox! Select a .hex file and press the "Flash" button. After flashing, you must press the green (lower-right) switch to exit the bootloader, or unplug and replug the SCRAMBLE.
