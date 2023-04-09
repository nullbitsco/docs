# QMK Flashing Instructions

Follow these instructions to flash your Pro Micro, Bit-C, or Bit-C PRO microcontroller:

1. Determine which MCU you are using: 
   1. If you are using a Pro Micro or Bit-C AVR (with ATmega32U4), your MCU uses `.hex` files and is flashed using QMK Toolbox.
   1. If you are using a Bit-C PRO (RP2040), your MCU uses `.uf2` files and is flashed by dragging and dropping the firmware to the RPI-RP2 USB device. [Read more here](https://github.com/nullbitsco/docs/blob/main/bit-c-pro/user_guide_en.md).
   1. If you have purchased a SCRAMBLE before January 2023, it likely a V1, and uses `.hex` files and is flashed using QMK Toolbox.
   1. If you have purchased a SCRAMBLE after January 2023, it is likely a V2, which uses `.uf2` files and is flashed by dragging and dropping the firmware to the RPI-RP2 USB device, just like the Bit-C PRO.
1. Download the firmware for your device. All firmwares are compatible with [VIA](https://caniusevia.com), which can be used to configure keybinds, underglow, and more!
   - For Snap - [Pro Micro & Bit-C (AVR)](https://github.com/nullbitsco/firmware/releases/download/latest/nullbitsco_snap_via.hex) | [Bit-C PRO (RP2040)](https://github.com/nullbitsco/firmware/releases/download/nightly-rp2040/nullbitsco_snap_rp2040_via.uf2)
   - For Nibble - [Pro Micro & Bit-C (AVR)](https://github.com/nullbitsco/firmware/releases/download/latest/nullbitsco_nibble_via.hex) | [Bit-C PRO (RP2040)](https://github.com/nullbitsco/firmware/releases/download/nightly-rp2040/nullbitsco_nibble_rp2040_via.uf2)
   - For Tidbit - [Pro Micro & Bit-C (AVR)](https://github.com/nullbitsco/firmware/releases/download/latest/nullbitsco_tidbit_via.hex) | [Bit-C PRO (RP2040)](https://github.com/nullbitsco/firmware/releases/download/nightly-rp2040/nullbitsco_tidbit_rp2040_via.uf2)
   - For Scramble - [V1 (AVR)](https://github.com/nullbitsco/firmware/releases/download/latest/nullbitsco_scramble_via.hex) | [V2 (RP2040)](https://github.com/nullbitsco/firmware/releases/download/nightly-rp2040/nullbitsco_scramble_v2_via.uf2)
1. For Pro Micro, Bit-C (AVR) and SCRAMBLE V1, download and install [QMK Toolbox](https://github.com/qmk/qmk_toolbox/releases). If on Windows, also install device drivers when prompted. Bit-C PRO (RP2040) and SCRAMBLE V2 don't require QMK Toolbox or any additional drivers.
1. For Bit-C PRO (RP2040) and SCRAMBLE V2, follow the [firmware flashing guide](https://github.com/nullbitsco/docs/blob/main/bit-c-pro/user_guide_en.md#loading-new-firmware) and you're done! For Pro Micro, Bit-C (AVR) and SCRAMBLE V1, continue below.
1. Connect your MCU in DFU Mode. If using a new Bit-C, it will be in DFU mode by default (LED will glow white).
   - To enter DFU mode, press the reset switch, or short the RST pin to GND with a wire or some tweezers.
1. Open QMK Toolbox and select the firmware file you downloaded earlier.
1. Click flash and wait for it to complete. QMK Toolbox will tell you how many bytes were written and a percentage (for example: `0x3F80 bytes written into 0x7000 bytes memory (56.70%)`); this is normal, and means that everything worked properly.
1. Disconnect and reconnect the Pro-Micro or Bit-C. On the Bit-C, the LED light will stop glowing indicating that the board has loaded the firmware. Note that it will no longer show up in QMK Toolbox! That is expected. If you want to flash again, you need to enter DFU mode (see step 3 above)

# Setting up VIA

1. Flash VIA compatible firmware for your device, as described above.
1. Connect your device and open VIA using the [webapp](https://usevia.app/).
1. Go to the Configure tab. Your device should now be detected and ready to configure.

## <a name="troubleshooting"></a> Troubleshooting

If you are having issues flashing your firmware, check these things first:
| **Issue** | **Thing to check** |
| --- | --- |
| VIA won't detect my TIDBIT | Reflash your TIDBIT with the VIA firmware (this is important!) and follow the "Setting up VIA" section above. |
| I connect my MCU but nothing happens | Change USB ports, cables, and PCs if possible. You'd be surprised by how many times one of these items fixes it. |
| QMK Toolbox can see my Bit-C PRO (RP2040) in programming mode, but I can't flash it! | The RP2040 isn't flashed with Toolbox! [Follow these steps instead](https://github.com/nullbitsco/docs/blob/main/bit-c-pro/user_guide_en.md). |
| MCU is in DFU, but QMK Toolbox won't detect it or won't flash | Right click in the window and select Install Drivers. Please refer to [this](https://docs.qmk.fm/#/driver_installation_zadig?id=list-of-known-bootloaders) page for the correct driver for your particular bootloader. |
I flashed my MCU once, and now it's not working | Are you sure it's not working? It's more than likely just not showing up in Toolbox, which is normal. You need to press the reset button or short RST to GND in order for it to show up again. |

## <a name="helpful_links"></a> Helpful links

Check out these awesome resources before diving into firmware customizations.

- [QMK Tutorial: QMK Toolbox (Flashing Firmware On Your Keyboard)](https://youtu.be/fuBJbdCFF0Q)
- [QMK Tutorial: How to get VIA on your board](https://youtu.be/lyvf7Yp1z5g)
- [How to Install/Use VIA Configurator (Tutorial)](https://youtu.be/78zVepszCmE)

## Firmware Building Instructions

Follow the [QMK Newbs Guide](https://docs.qmk.fm/#/newbs) for a great tutorial on setting up and building QMK firmware.
