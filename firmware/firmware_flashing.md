# Firmware Flashing

## Building and flashing QMK firmware 

# Contents
[Helpful Links](#helpful_links)  
[NIBBLE](#nibble)  
[TIDBIT](#tidbit)  
[SCRAMBLE](#scramble)  
[Proton-C conversion](#proton_c)  
[Flashing Instructions and Firmware Binaries](#releases)  


# <a name="helpful_links"></a> Helpful links
Check out these awesome resources before diving into firmware customizations.
* [QMK Tutorial: QMK Toolbox (Flashing Firmware On Your Keyboard)](https://youtu.be/fuBJbdCFF0Q)
* [QMK Tutorial: How to get VIA on your board](https://youtu.be/lyvf7Yp1z5g)
* [How to Install/Use VIA Configurator (Tutorial)](https://youtu.be/78zVepszCmE)

## [TODO] <a name="proton_c"></a> Proton-C conversion
https://github.com/jaygreco/qmk_firmware/tree/proton_c_conversion

## [TODO] <a name="nibble"></a> NIBBLE

## [TODO] <a name="tidbit"></a> TIDBIT

## [TODO] <a name="scramble"></a> SCRAMBLE

## <a name="releases"></a> Flashing Instructions and Firmware Binaries

Follow these instructions to flash your Pro Micro or Bit-C microcontroller:
1. Download the firmware for your device:
    * [NIBBLE default firmware](https://github.com/nullbitsco/docs/raw/main/firmware/default_firmware/nullbitsco_nibble_default.hex)
    * [TIDBIT default firmware](https://github.com/nullbitsco/docs/raw/main/firmware/default_firmware/nullbitsco_tidbit_default.hex)
    * [SCRAMBLE default firmware](https://github.com/nullbitsco/docs/raw/main/firmware/default_firmware/nullbitsco_scramble_default.hex)

2. Download [QMK Toolbox](https://github.com/qmk/qmk_toolbox/releases).
3. Connect your Pro-Micro in DFU mode. If using a new Bit-C, it will be in DFU mode already as indicated by the glowing white LED.
4. Open QMK Toolbox and select the firmware file.
5. Click flash and wait for it to complete.
6. Disconnect and reconnect the Pro-Micro or Bit-C. On the Bit-C, the LED light will stop glowing indicating that the board has loaded the firmware. 
