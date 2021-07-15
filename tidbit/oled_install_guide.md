# SSD1306 OLED Install Guide

If you purchased the Nullbits OLED, or a SSD1306 OLED, follow this guide to install it on your device.

## For Tidbit
1. Solder 4 header pins with their short ends into the marked sockets on the Tidbit PCB.<br>
_[TODO: Add picture of header pins placed in PCB with a highlight rectangle drawn around them.]_
2. [OPTIONAL] If building with plate, install hotswap / mill-max sockets and install plate before proceeding.<br>
_[TODO: Add picture of plate and switches installed in PCB and OLED header pins sticking out through plate.]_
3. Insert the OLED on the header pins such that the far end rests on the USB-C port. Use tape to hold it in place and ensure it is horizontal.<br>
_[TODO: Insert picture of OLED position after insert through header pins.]_
4. Solder the OLED. Be careful not to damage the display while soldering.
5. Flash the [OLED keymap firmware](https://github.com/nullbitsco/tidbit/releases/download/v1.5/nullbitsco_tidbit_oled.hex) for the Tidbit (flashing instructions can be found [here](https://github.com/nullbitsco/docs/blob/main/firmware/firmware_flashing.md)).

If installed correctly, the OLED will show the Nullbits logo when plugged in.<br>
_[TODO: Insert picture of OLED displaying Nullbits logo]_
