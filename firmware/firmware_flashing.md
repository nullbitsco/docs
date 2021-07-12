# QMK Flashing Instructions
Follow these instructions to flash your Pro Micro or Bit-C microcontroller:
1. Download the firmware for your device. If using [VIA](https://caniusevia.com) to configure, download the VIA version:
    * For Nibble - [Default](https://github.com/nullbitsco/nibble/releases/download/v1.3/nullbitsco_nibble_default.hex) | [VIA](https://github.com/nullbitsco/nibble/releases/download/v1.3/nullbitsco_nibble_via.hex)
    * For Tidbit - [Default](https://github.com/nullbitsco/tidbit/releases/download/v1.4/nullbitsco_tidbit_default.hex)  |  [VIA](https://github.com/nullbitsco/tidbit/releases/download/v1.4/nullbitsco_tidbit_via.hex)
    * For Scramble - [Default](https://github.com/nullbitsco/docs/raw/main/firmware/default_firmware/nullbitsco_scramble_default.hex)
2. Download and install [QMK Toolbox](https://github.com/qmk/qmk_toolbox/releases). If on Windows, also install device drivers when prompted. 
4. Connect your Pro-Micro MCU in DFU Mode. If using a new Bit-C, it will be in DFU mode by default (LED will glow white).
6. Open QMK Toolbox and select the firmware file you downloaded earlier.
7. Click flash and wait for it to complete.
8. Disconnect and reconnect the Pro-Micro or Bit-C. On the Bit-C, the LED light will stop glowing indicating that the board has loaded the firmware. 

# Setting up VIA
1. Flash VIA compatible firmware for your device, as described above. 
2. Download and install [VIA](https://caniusevia.com).
3. Download the VIA keymap file for your device - [Nibble](https://github.com/nullbitsco/nibble/blob/master/keymaps/via/nibble.json) | [Tidbit](https://github.com/nullbitsco/tidbit/blob/master/keymaps/via/tidbit.json).
4. Connect your device and open VIA.
5. If your device is not detected, go to Settings > Enable "Show Design Tab".
6. Go to the Design tab.
7. Click "Load Draft Definition" and upload the VIA keymap file you downloaded in step 3.
8. Go to the Configure tab. Your device should now be detected and ready to configure. 

## <a name="helpful_links"></a> Helpful links
Check out these awesome resources before diving into firmware customizations.
* [QMK Tutorial: QMK Toolbox (Flashing Firmware On Your Keyboard)](https://youtu.be/fuBJbdCFF0Q)
* [QMK Tutorial: How to get VIA on your board](https://youtu.be/lyvf7Yp1z5g)
* [How to Install/Use VIA Configurator (Tutorial)](https://youtu.be/78zVepszCmE)

## [TODO] <a name="proton_c"></a> Proton-C conversion
https://github.com/jaygreco/qmk_firmware/tree/proton_c_conversion

## [TODO] Firmware Building Instructions
