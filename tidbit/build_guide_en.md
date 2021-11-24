# TIDBIT

### Customizable 19-Key Numpad Kit

![](https://github.com/nullbitsco/docs/raw/main/tidbit/build_guide_img/image018.jpg)

### Build Guide

# Contents

[Helpful Links](#helpful_links)

[Parts and Tools](#parts_and_tools)

[Assembly Steps](#assembly_steps)

[Troubleshooting](#troubleshooting)

# <a name="helpful_links"></a> 1. Helpful links

- [Default Keymap](http://www.keyboard-layout-editor.com/#/gists/a1aedbf7a153c6ec3295f0ea32b6ad5b)
- [TIDBIT Diode Key (AKA which diode connects to which switch)](https://nullbits.co/static/file/TIDBIT_diode_key.pdf)
- [QMK Firmware](https://github.com/nullbitsco/tidbit)
- [Basic Skills: Soldering](https://www.youtube.com/watch?v=UpVx4wGukRc) - Make sure you're prepared to solder your keyboard kit!
- [Another Great Soldering Guide](https://mightyohm.com/files/soldercomic/FullSolderComic_EN.pdf)
- [Check the](https://github.com/nullbitsco/docs/raw/main/nibble/build_guide_img/image048.png) quality of your [soldering joints!](https://github.com/nullbitsco/docs/raw/main/nibble/build_guide_img/image049.png)
- [How to use a DMM](https://www.youtube.com/watch?v=SECWePatYjY) - Important if you need to troubleshoot your build!
- [Firmware Flashing Guide](https://github.com/nullbitsco/docs/blob/main/firmware/firmware_flashing.md)

## Thanks for purchasing!

Seriously, thank you! The TIDBIT has been a passion project of mine over the past year. I've been using a TIDBIT in its various stages of development and think it's a great keyboard that you'll love. I've designed and assembled the kits during my free time, and I want to make sure you have a great experience. If at any point you hit a snag or have a question, feel free to let us know.

# <a name="parts_and_tools"></a> 2. Parts and tools

![](https://github.com/nullbitsco/docs/raw/main/tidbit/build_guide_img/image003.jpg)

### Hardware

| **Item**        | **Qty.** | **Image**                                                                            |
| --------------- | -------- | ------------------------------------------------------------------------------------ |
| Standoff, M2x3  | 6        | ![](https://github.com/nullbitsco/docs/raw/main/tidbit/build_guide_img/image028.jpg) |
| Standoff, M2x10 | 2        | ![](https://github.com/nullbitsco/docs/raw/main/tidbit/build_guide_img/image026.jpg) |
| Screw, M2x3     | 12       | ![](https://github.com/nullbitsco/docs/raw/main/tidbit/build_guide_img/image030.jpg) |
| Screw, M2x6     | 2        | ![](https://github.com/nullbitsco/docs/raw/main/tidbit/build_guide_img/image033.jpg) |
| Screw, M2x10    | 2        | ![](https://github.com/nullbitsco/docs/raw/main/tidbit/build_guide_img/image032.jpg) |
| Machined Knob   | 1        | ![](https://github.com/nullbitsco/docs/raw/main/tidbit/build_guide_img/image034.jpg) |

### Electronics

| **Item**              | **Qty.** | **Image**                                                                            |
| --------------------- | -------- | ------------------------------------------------------------------------------------ |
| 1N4148 Diode          | 19       | ![](https://github.com/nullbitsco/docs/raw/main/tidbit/build_guide_img/image031.jpg) |
| Reset Switch          | 1        | ![](https://github.com/nullbitsco/docs/raw/main/tidbit/build_guide_img/image027.jpg) |
| WS2812B LED           | 8        | ![](https://github.com/nullbitsco/docs/raw/main/tidbit/build_guide_img/image023.jpg) |
| TRRS Jack             | 1        | ![](https://github.com/nullbitsco/docs/raw/main/tidbit/build_guide_img/image024.jpg) |
| Rotary Encoder        | 1        | ![](https://github.com/nullbitsco/docs/raw/main/tidbit/build_guide_img/image029.jpg) |
| Breakaway Header Pins | 40       | ![](https://github.com/nullbitsco/docs/raw/main/tidbit/build_guide_img/image035.jpg) |

### Core

| **Item**              | **Qty.** | **Image**                                                                            |
| --------------------- | -------- | ------------------------------------------------------------------------------------ |
| Top PCB plate         | 1        | ![](https://github.com/nullbitsco/docs/raw/main/tidbit/build_guide_img/image020.jpg) |
| Bottom PCB plate      | 1        | ![](https://github.com/nullbitsco/docs/raw/main/tidbit/build_guide_img/image022.jpg) |
| Middle acrylic spacer | 1        | ![](https://github.com/nullbitsco/docs/raw/main/tidbit/build_guide_img/image019.jpg) |
| Top acrylic guard     | 1        | ![](https://github.com/nullbitsco/docs/raw/main/tidbit/build_guide_img/image025.jpg) |

## 1. Parts you provide

- PCB-mount switches (Cherry MX footprint)
- [Keycaps. Recommended set (pictured in product photos)](https://drop.com/buy/dsa-dolch-key-set)
- [BIT-C](https://nullbits.co/bit-c/) or other Pro Micro compatible MCU
- **[OPTIONAL]** [0.91" 128x32 OLED Display](https://www.amazon.com/dp/B08KL8YKVW)
- **[OPTIONAL]** [FR4 switch plate](http://www.amazon.com/dp/B08M9RM8YQ)
- **[OPTIONAL]** [Extra encoder & knob](http://www.amazon.com/dp/B08NH53BMJ)
- **[OPTIONAL]** Qty. 40 Mill-Max 0305 or 7305 hot-swap solder sockets

## 2. Optional Add-ons and extras [not included]

- [**Adafruit Mini 8x8 LED Matrix w/I2C Backpack**](https://www.adafruit.com/product/1080)
- [**16x8 1.2&quot; LED Matrix w/I2C Backpack**](https://www.adafruit.com/product/2038)
- [**Quad Alphanumeric Display - 0.54 w/I2C Backpack**](https://www.adafruit.com/product/2157)

## 3. Tools required

- Fine-tip soldering iron &amp; solder
- Needle nose pliers
- Phillips #0 screwdriver
- Snips for cutting leads
- Rubbing alcohol
- **[Recommended]** DMM/Multimeter
- **[Recommended]** USB Current Meter

# <a name="assembly_steps"></a> 3. Assembly Steps

⚠️ **Important!** Notes marked with this icon are crucial, so be sure to read them carefully before moving on.

⚠️ **Stop!** If at any point during your build you find yourself confused, stuck, not sure whether something you're doing is right, or not sure what to do next, stop and ask! On average, questions are answered on Discord or via email in less than a few hours. Better to ask questions that might feel silly than to make a mistake!

Steps marked [OPTIONAL] aren&#39;t required for the base kit, but may be needed depending on what you choose to include in your build.

## 1. Solder reset switch

Fit and solder the reset switch as shown below.

![](https://github.com/nullbitsco/docs/raw/main/tidbit/build_guide_img/image005.jpg)

After soldering, clean with rubbing alcohol.

## 2. [OPTIONAL] Solder underglow LEDS

[Recommended resource: soldering 5050 SMT LEDs](https://electronics.stackexchange.com/questions/482626/how-to-solder-ws2812b-ledsindividual-not-a-strip-to-a-pcb)

Solder the 8x WS2812B underglow LEDs. Start by tacking down one corner, and then soldering the remaining 3 leads. After soldering, clean with rubbing alcohol.

⚠️ **Orientation matters!** These parts have a small angled mark which should match up with the one on the PCB. If you don&#39;t get the orientation right, the LEDs will not work, and your keyboard may not boot up.

![](https://github.com/nullbitsco/docs/raw/main/tidbit/build_guide_img/image006.jpg)

## 3. Bend and solder diodes

Bend and fit the 1N4148 diodes. In order to get uniform placement of the diodes, I recommend using a diode bending tool. You can buy one or 3D print one. [Here&#39;s a link to my favorite](https://www.thingiverse.com/thing:4332520). Bend the leads inward to hold the diodes in place when the PCB is turned upside down. Begin by soldering one side of the diodes and adjust the diode alignment to your liking before soldering the second lead.

⚠️ **Orientation matters!** Solder the diodes with the black bar **UP** as shown in the images. The keyboard will not work if they are backward.

![](https://github.com/nullbitsco/docs/raw/main/tidbit/build_guide_img/image015.jpg)

After soldering all diodes, clean with rubbing alcohol and use the snips to clip the leads as close to the PCB as possible.

## 4. [OPTIONAL] Solder TRRS expansion jack

Fit and solder the 4-pin TRRS expansion jack as shown below. After soldering, clean with rubbing alcohol.

![](https://github.com/nullbitsco/docs/raw/main/tidbit/build_guide_img/image001.jpg)

# ⚠️ **STOP** ⚠️

It&#39;s highly recommended that you flash the MCU (Bit-C or Pro Micro) before soldering it so you can be sure it&#39;s working properly. [Jump to](#firmware_flashing) step 16 QMK firmware.

## 5. Solder MCU

Use header pins to solder the MCU to the keybpard. Fit and solder the BIT-C or Pro Micro MCU using 0.1" male header pins as shown below. After soldering, clean with rubbing alcohol and use the snips to clip the pins as close to the PCB as possible.

![](https://github.com/nullbitsco/docs/raw/main/tidbit/build_guide_img/image013.jpg)

## 6. [OPTIONAL] Solder rotary encoder, LED matrix, and/or OLED display

If building with the optional rotary encoder, alphanumeric display or LED matrix, or OLED display in place of the programmable macro keys, fit and solder each in the position each shown. After soldering, clean with rubbing alcohol and use the snips to clip the pins as close to the PCB as possible. Note that it is **not** necessary to solder the large side support pins on the rotary encoder. **Do not clip the large support pins on the encoder.**

![](https://github.com/nullbitsco/docs/raw/main/tidbit/build_guide_img/image002.png)

⚠️ **Compatibility note:** the top-left and top-right encoder (encoder 1) footprints share the same signals. An encoder should only be installed in one of the footprints.

⚠️ **Compatibility note:** encoder 3 shares the drive signals with the I2C bus. It can not be used at the same time as the OLED, alphanumeric display, or LED matrix options.

⚠️ **Compatibility note:** encoder 4 shares the drive signals with the UART bus. It can not be used at the same time as the expansion port.

**Placement guide (see image below):**

![](https://github.com/nullbitsco/docs/raw/main/tidbit/build_guide_img/image000.png)

![](https://github.com/nullbitsco/docs/raw/main/tidbit/build_guide_img/image021.png)

## 7. Choose key layout and configuration

The TIDBIT supports a standard numpad layout as well as a more dense 19-key layout option. Each is compatible with the various rotary encoder options.

| ![](https://github.com/nullbitsco/docs/raw/main/tidbit/build_guide_img/image009.jpg) | ![](https://github.com/nullbitsco/docs/raw/main/tidbit/build_guide_img/image011.jpg) |
| ------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------ |

# ⚠️ **STOP** ⚠️

It&#39;s highly recommended that you test each key at this point before continuing. Jump to step 16 to flash QMK firmware. Use a keyboard tester ([this one](https://www.keyboardtester.com/) works) and short the switch pads for each switch using tweezers, a clipped lead from earlier, or something else conductive. If there is an issue, it will be much easier to debug now before everything has been soldered and assembled.

## 8. Screw together M2x3 standoffs using M2x3 screws

In the locations shown, screw the M2x3 standoffs into the **TOP** PCB plate. Fasten using 6 M2x3 screws. Use pliers to hold the standoff steady while tightening the screw. **Do not overtighten!**

⚠️ This step is extra important if you are building with a plate, since it's more difficult to access the screws with the plate in place.

![](https://github.com/nullbitsco/docs/raw/main/tidbit/build_guide_img/image007.jpg)

## 9. [OPTIONAL] Insert hot-swap sockets

If building with hotswap sockets, drop one into each plated lead hole. Alternatively, insert them onto each lead of the PCB mount switch before proceeding.

## 10. Snap in switches

⚠️ **Stop!** Test fit your keycaps to make sure that the switch spacings are correct before soldering, especially the bottom row.

The switches will take some force to insert. This is by design. The TIDBIT doesn&#39;t have a plate mount, so the tight fit makes in the PCB the switches more stable. Snap in by supporting the back of the PCB, and then pushing hard on the top of the switch. It helps to use a spare keycap on the switch to take some of the pressure off your thumb. After snapping the switch in, make sure it&#39;s sitting flush against the PCB.

![](https://github.com/nullbitsco/docs/raw/main/tidbit/build_guide_img/image016.jpg)

## 11. Solder switches or hot-swap sockets

Make sure each switch pin has enough solder to form a nice solid joint.

## 12. Slide the acrylic spacer onto the standoffs

Make sure the acrylic spacer sits flat against the PCB plate. Check for interreferences due to leads or solder joints. Trim if needed. If using the TRRS expansion jack, snap out the acrylic piece to fit it.

![](https://github.com/nullbitsco/docs/raw/main/tidbit/build_guide_img/image004.jpg)

## 13. Fasten the bottom with M2x3 screws

Place the bottom PCB plate on top of the acrylic spacer. In the same locations where the 6 standoffs were installed, fasten with 6 M2x3 screws. **Do not overtighten!**

![](https://github.com/nullbitsco/docs/raw/main/tidbit/build_guide_img/image017.jpg)

## 14. Fasten M2x10 standoffs from bottom using M2x10 screws

Fasten using 2 M2x10 screws. Use pliers to hold the standoff steady while tightening the screw.

![](https://github.com/nullbitsco/docs/raw/main/tidbit/build_guide_img/image012.jpg)

## 15. Attach the top guard using M2x6 screws

Fasten using 2 M2x6 screws. Don&#39;t overtighten these, as it can crack the top guard.

![](https://github.com/nullbitsco/docs/raw/main/tidbit/build_guide_img/image014.jpg)

## 16. <a name="firmware_flashing"></a> Flash firmware using QMK toolbox

Download either a precompiled binary (only if using a Pro Micro or BIT-C) or the QMK source files from [GitHub](https://github.com/nullbitsco/tidbit). Using [QMK Toolbox](https://qmk.fm/toolbox/), flash the firmware onto the keyboard. For more information, follow the [Firmware flashing guide](https://github.com/nullbitsco/docs/blob/main/firmware/firmware_flashing.md)

If using VIA, download the json file [here](https://github.com/nullbitsco/tidbit/blob/master/keymaps/via/tidbit.json). Click "Raw." Download the file by right clicking and selecing "Save as..."

## 17. Enjoy!

![](https://github.com/nullbitsco/docs/raw/main/tidbit/build_guide_img/image008.jpg)

# 4. <a name="troubleshooting"></a> Troubleshooting

**None of the keys are working**

- Is the firmware loaded?
- Check the direction of the diodes. The back bar should be facing upwards.
- Check that there are no shorts and that the keyboard is powering up properly.

**A single key is not working**

- Check that all of the diodes are soldered properly at both pins.
- Bypass the switch by shorting the two pads with tweezers. If that works, the switch is to blame and should be replaced. If it does not, the diode soldering is likely the issue. You can use the [diode key](https://nullbits.co/static/file/TIDBIT_diode_key.pdf) to match diodes with a switch!
- Check that the switch is soldered properly at both pins.
- Check that the keymap you are using is defined correctly and matches your keyboard layout.

**A whole row is not working**

- Check that all pins on the MCU are soldered properly.
- Check that the proper rows and columns are set in QMK config.h

**A whole column is not working**

- Check that all pins on the MCU are soldered properly.
- Check that the proper rows and columns are set in QMK config.h

**The rotary encoder is not working**

- Check that all pins on the rotary encoder are soldered properly.
- Check that the A and B pins are set in QMK config.h and that ENCODER_ENABLE = yes in QMK rules.mk.

**Two or more keys are swapped**

- Check that the keymap you are using is defined correctly and matches your keyboard layout.

**The underglow LEDs are not working**

- The LED underglow is on and set to red by default. If all of the LEDs are not on, soldering is almost always the culprit! The LEDs are in a series "chain". Symptoms can include: LEDs not turning on after a specific LED, LEDs flickering, LEDs changing themselves to random colors, or LEDs behaving differently each time you power cycle the keyboard.
- Carefully reflow (remelt) the each solder joint on the last LED that is working properly, along with the first one that isn't, and then power cycle the keyboard. It might take a few tries, and you might have multiple LEDs that need to be touched up.
- The LEDs "snake" downward, and the very first LED is the one just below the Bit-C.
- Check that the RGB_DI_PIN pin is set in QMK config.h and that RGBLIGHT_ENABLE = yes in QMK rules.mk.
- Check that all LEDs are soldered in the proper orientation.

**There&#39;s no power**

- Check that all LEDs are soldered in the proper orientation.
- Check for other shorts – solder blobs, leads that were not clipped all the way, etc.

**How to I do X in firmware?**

- See the QMK docs, or make a post on r/olkb for help.
- Make a post on the [r/nullbits](https://www.reddit.com/r/nullbits/) subreddit, or join the #firmware channel in the [nullbits discord server](https://discord.gg/eSegJcY).

**Something else?**

- Visit [nullbits.co/support/](https://nullbits.co/support/)
- Reach out at [help@nullbits.co](mailto:help@nullbits.co)
- Join our [Discord](https://discord.gg/eSegJcY)!

TIDBIT 0x1 Assembly Instructions Rev03 03.25.21
