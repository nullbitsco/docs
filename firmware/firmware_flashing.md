# QMK Flashing Instructions

Follow these instructions to flash your Pro Micro or Bit-C microcontroller:

1. Download the firmware for your device. If using [VIA](https://caniusevia.com) to configure, download the VIA version:
   - For Snap - [Default](https://github.com/nullbitsco/firmware/releases/download/latest/nullbitsco_snap_default.hex) | [VIA](https://github.com/nullbitsco/firmware/releases/download/latest/nullbitsco_snap_via.hex)
   - For Nibble - [Default](https://github.com/nullbitsco/firmware/releases/download/latest/nullbitsco_nibble_default.hex) | [VIA](https://github.com/nullbitsco/firmware/releases/download/latest/nullbitsco_nibble_via.hex)
   - For Tidbit - [Default](https://github.com/nullbitsco/firmware/releases/download/latest/nullbitsco_tidbit_default.hex) | [VIA](https://github.com/nullbitsco/firmware/releases/download/latest/nullbitsco_tidbit_via.hex)
   - For Scramble - [VIA](https://github.com/nullbitsco/firmware/releases/download/latest/nullbitsco_scramble_via.hex)
1. Download and install [QMK Toolbox](https://github.com/qmk/qmk_toolbox/releases). If on Windows, also install device drivers when prompted.
1. Connect your Pro-Micro MCU in DFU Mode. If using a new Bit-C, it will be in DFU mode by default (LED will glow white).
   - To enter DFU mode, press the reset switch, or short the RST pin to GND with a wire or some tweezers.
1. Open QMK Toolbox and select the firmware file you downloaded earlier.
1. Click flash and wait for it to complete. QMK Toolbox will tell you how many bytes were written and a percentage (for example: `0x3F80 bytes written into 0x7000 bytes memory (56.70%)`); this is normal, and means that everything worked properly.
1. Disconnect and reconnect the Pro-Micro or Bit-C. On the Bit-C, the LED light will stop glowing indicating that the board has loaded the firmware. Note that it will no longer show up in QMK Toolbox! That is expected. If you want to flash again, you need to enter DFU mode (see step 3 above)

# Setting up VIA

1. Flash VIA compatible firmware for your device, as described above.
1. Download and install [VIA](https://caniusevia.com).
1. Download the VIA keymap file for your device. NOTE: ONLY REQUIRED FOR TIDBIT AND SNAP.
   - [Snap](https://raw.githubusercontent.com/nullbitsco/snap/main/keymaps/via/snap.json)
   - [Tidbit](https://raw.githubusercontent.com/nullbitsco/tidbit/master/keymaps/via/tidbit.json)
3. Connect your device and open VIA.
4. If your device is not detected, go to Settings > Enable "Show Design Tab".
5. Go to the Design tab.
6. Click "Load Draft Definition" and upload the VIA keymap file you downloaded in step 3.
7. Go to the Configure tab. Your device should now be detected and ready to configure.

## <a name="troubleshooting"></a> Troubleshooting

If you are having issues flashing your firmware, check these things first:
| **Issue** | **Thing to check** |
| --- | --- |
| VIA won't detect my TIDBIT | Reflash your TIDBIT with the VIA firmware (this is important!) and follow the "Setting up VIA" section above. |
| I connect my MCU but nothing happens | Change USB ports, cables, and PCs if possible. You'd be surprised by how many times one of these items fixes it. |
| MCU is in DFU, but QMK Toolbox won't detect it or won't flash | Right click in the window and select Install Drivers. Please refer to [this](https://docs.qmk.fm/#/driver_installation_zadig?id=list-of-known-bootloaders) page for the correct driver for your particular bootloader. |
I flashed my MCU once, and now it's not working | Are you sure it's not working? It's more than likely just not showing up in Toolbox, which is normal. You need to press the reset button or short RST to GND in order for it to show up again. |

## <a name="helpful_links"></a> Helpful links

Check out these awesome resources before diving into firmware customizations.

- [QMK Tutorial: QMK Toolbox (Flashing Firmware On Your Keyboard)](https://youtu.be/fuBJbdCFF0Q)
- [QMK Tutorial: How to get VIA on your board](https://youtu.be/lyvf7Yp1z5g)
- [How to Install/Use VIA Configurator (Tutorial)](https://youtu.be/78zVepszCmE)

## <a name="proton_c"></a> Proton-C conversion

If you want to convert the nibble firmware to Proton-C flavor, the normal build will encounter some issues. Use the following as a starting point.
https://github.com/jaygreco/qmk_firmware/tree/proton_c_conversion

## Firmware Building Instructions

Follow the [QMK Newbs Guide](https://docs.qmk.fm/#/newbs) for a great tutorial on setting up and building QMK firmware
