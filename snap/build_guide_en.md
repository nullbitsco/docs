# SNAP

## 75% Split Keyboard Kit

![](build_guide_img/image000.jpg)

## Build Guide

# Contents

[Helpful Links](#helpful_links)

[Parts and Tools](#parts_and_tools)

[Assembly Steps](#assembly_steps)

[Troubleshooting](#troubleshooting)

## Thanks for purchasing!

We're humbled by how much interest and love the NIBBLE and the TIDBIT have received. After lots of research, iteration, and feedback, we have what we hope is an even more popular follow-on to the two. The SNAP (we hope) takes the best of the two and then some. We hope you love building and using this board as much as we have.

# <a name="helpful_links"></a> 1. Helpful links

- [Default Keymap](http://www.keyboard-layout-editor.com/#/gists/bd48e2fe5b0f571c0034f27cb328d2d7)
- [QMK Firmware](https://github.com/nullbitsco/snap)
- [Basic Skills: Soldering](https://www.youtube.com/watch?v=UpVx4wGukRc) - Make sure you're prepared to solder your keyboard kit!
- [Check the](build_guide_img/image048.png) quality of your [soldering joints!](build_guide_img/image049.png)
- [How to use a DMM](https://www.youtube.com/watch?v=SECWePatYjY) - Important if you need to troubleshoot your build!
- [Firmware Flashing Guide](https://github.com/nullbitsco/docs/blob/main/firmware/firmware_flashing.md)

# <a name="parts_and_tools"></a> 2. Parts and tools

![](build_guide_img/image001.jpg)

## 1. Parts included in the kit

### Hardware

| **Item** | **Qty.** | **Image** |
| --- | --- | --- |
| Standoff, M2x3 | 16 | ![](build_guide_img/image002.jpg) |
| Standoff, M2x10 | 6 | ![](build_guide_img/image004.jpg) |
| Screw, M2x3 | 30 | ![](build_guide_img/image006.jpg) |
| Screw, M2x6 | 6 | ![](build_guide_img/image008.jpg) |
| Screw, M2x10 | 6 | ![](build_guide_img/image010.jpg) |
| Machined Knob | 1 | ![](build_guide_img/image046.jpg) |

### Electronics

| **Item** | **Qty.** | **Image** |
| --- | --- | --- |
| 1N4148 Diode | 100 | ![](build_guide_img/image003.jpg) |
| 0.1μF Capacitor | 2 | ![](build_guide_img/image005.jpg) |
| 10KΩ Resistor | 2 | ![](build_guide_img/image013.jpg) |
| IC Socket | 2 | ![](build_guide_img/image007.jpg) |
| IC (74HC138N) | 2 | ![](build_guide_img/image009.jpg) |
| Reset Switch | 2 | ![](build_guide_img/image011.jpg) |
| WS2812B LED | 10 | ![](build_guide_img/image042.jpg) | 
| TRRS Jack | 4 | ![](build_guide_img/image043.jpg) |
| Rotary Encoder | 1 | ![](build_guide_img/image044.jpg) |
| PTH Buzzer | 1 | ![](build_guide_img/image045.jpg) |
| PTH Pogo Pins (male) | 2 | ![](build_guide_img/image015.jpg) |
| PTH Pogo Pins (female) | 2 | ![](build_guide_img/image014.jpg) |
| 40-pin Breakaway Headers | 2 | ![](build_guide_img/image047.jpg) |

### Core

| **Item** | **Qty.** | **Image** |
| --- | --- | --- |
| Top PCB plate (left) | 1 | ![](build_guide_img/image016.jpg) |
| Top PCB plate (right) | 1 | ![](build_guide_img/image029.jpg) |
| Bottom PCB plate (left) | 1 | ![](build_guide_img/image030.jpg) |
| Bottom PCB plate (right) | 1 | ![](build_guide_img/image031.jpg) |
| Middle acrylic spacer (left) | 1 | ![](build_guide_img/image033.jpg) |
| Middle acrylic spacer (right) | 1 | ![](build_guide_img/image034.jpg) |
| Top acrylic guard (left) | 1 | ![](build_guide_img/image037.jpg) |
| Top acrylic guard (right) | 1 | ![](build_guide_img/image038.jpg) |

### Extras

| **Item** | **Qty.** | **Image** |
| --- | --- | --- |
| TRRS cable | 1 | ![](build_guide_img/image039.jpg) |
| 3x6mm magnets | 6 | ![](build_guide_img/image040.jpg) |
| Magnet stickers | 6 | ![](build_guide_img/image041.jpg) |
| Mini bumpons | 8 | ![](build_guide_img/image012.jpg) |

## 2. Parts you provide

- 2x [BIT-C](https://nullbits.co/bit-c/) or other Pro Micro compatible MCU
- Qty. 92 PCB-mount switches (Cherry MX footprint)
- 5x 2U PCB-mount stabilizers*. Snap-in or screw in both work.
  - 2x 2U stabs - one for each spacebar
  - 3x 2U stabs - for left shift, enter, and backspace
  - *[Optional] - 1x 2U stab if building with a 2.75U right shift
- Keycaps: [(black set pictured in product photos)](https://kbdfans.com/products/pbt-xda-143keys-keycaps-set) [(white set in product photos)](https://kbdfans.com/collections/keycaps/products/dsa-profile-simple-grey-dye-subbed-keycap-set)
- **[OPTIONAL]** [Additional rotary encoder and knob](https://amzn.to/3rOnY2l)
- **[OPTIONAL]** [0.91" 128x32 OLED Display(s)](https://amzn.to/3wjHpmK)
- **[OPTIONAL]** [FR4 switch plate](https://amzn.to/3IozdaE)
- **[OPTIONAL]** Mill-Max 0305 or 7305 hot-swap solder sockets

## 3. Tools required

- Fine-tip soldering iron &amp; solder
- Needle nose pliers
- Fine-point tweezers
- Phillips #0 screwdriver
- Snips for cutting leads
- Rubbing alcohol
- **[Recommended]** DMM/Multimeter
- **[Recommended]** USB Current Meter

# <a name="assembly_steps"></a> 3. Assembly Steps

⚠️ **Important!** Notes marked with this icon are crucial, so be sure to read them carefully before moving on.

⚠️ **Stop!** If at any point during your build you find yourself confused, stuck, not sure whether something you're doing is right, or not sure what to do next, stop and ask! On average, questions are answered on Discord or via email in less than a few hours. Better to ask questions that might feel silly than to make a mistake!


Steps marked [OPTIONAL] aren&#39;t required for the base kit, but may be needed depending on what you choose to include in your build.

## 1. [OPTIONAL] Solder Underglow LEDS

[Recommended resource: soldering 5050 SMT LEDs](https://electronics.stackexchange.com/questions/482626/how-to-solder-ws2812b-ledsindividual-not-a-strip-to-a-pcb)

Solder the 10x WS2812B underglow LEDs, 5x on each keyboard half. Start by tacking down one corner, and then soldering the remaining 3 leads. After soldering, clean with rubbing alcohol.

⚠️ **Orientation matters!** These parts have a small angled mark which should match up with the one on the PCB. If you don&#39;t get the orientation right, the LEDs will not work, and your keyboard may not boot up.

⚠️ **LED Issues** If you have soldered the LEDs, but are encountering issues (no underglow, random colors, flickering, or only some LEDs working), please follow the LEDs section in [troubleshooting](#troubleshooting), or take a look at the [LED debugging guide](../accessories/ws2812b_led_debug_docs.md).

| ![](build_guide_img/image081.jpg) | ![](build_guide_img/image080.jpg) |
| --- | --- |

## 2. Bend and solder resistors

Bend and solder R1 on each keyboard half.

| ![](build_guide_img/image017.jpg) | ![](build_guide_img/image018.jpg) |
| --- | --- |

After soldering, clean with rubbing alcohol and use the snips to clip the leads as close to the PCB as possible.

## 3. Solder reset switches

Fit and solder the reset switch on each keyboard half as shown below.

| ![](build_guide_img/image019.jpg) | ![](build_guide_img/image020.jpg) |
| --- | --- |

After soldering, clean with rubbing alcohol.

## 4. Solder IC sockets

Fit and solder the two IC sockets; one on each keyboard half. Match the notch in the socket with the one on the PCB. After soldering, clean with rubbing alcohol. **Note: if you accidentally solder one or both sockets backward, don't panic! The sockets are passive components and will work in either orientation. The direction of the ICs themselves is what really matters, so just make sure to insert the IC in the correct direction later on in the build!**

⚠️ **Do not solder the socket with the IC inserted!** The heat may damage the chip if it is in the socket during soldering.

| ![](build_guide_img/image021.jpg) | ![](build_guide_img/image022.jpg) |
| --- | --- |

## 5. Solder capacitors

Fit and solder the two capacitors; one on each keyboard half.

| ![](build_guide_img/image023.jpg) | ![](build_guide_img/image024.jpg) |
| --- | --- |

After soldering, clean with rubbing alcohol and use the snips to clip the leads as close to the PCB as possible.

## 6a. Bend and solder under-key diodes

There are a number of diodes that aren't in the main group on the top of the keyboard: **13** on the left half, and **11** on the right half. Bend and fit the 1N4148 diodes. Bend the leads inward to hold the diodes in place when the PCB is turned upside down. Begin by soldering one side of the diodes and adjust the diode alignment to your liking before soldering the second lead.

⚠️ **Orientation matters!** These go on the **TOP** side of the PCB! Solder the diodes with the black bar **UP** as shown in the images. The keyboard will not work if they are backward.

| ![](build_guide_img/image025.jpg) | ![](build_guide_img/image026.jpg) |
| --- | --- |

## 6b. Bend and solder top row of diodes

Bend and fit the remaining 1N4148 diodes for the top row. Bend the leads inward to hold the diodes in place when the PCB is turned upside down. Begin by soldering one side of the diodes and adjust the diode alignment to your liking before soldering the second lead.

⚠️ **Orientation matters!** These go on the **TOP** side of the PCB! Solder the diodes with the black bar **UP** as shown in the images. The keyboard will not work if they are backward.

| ![](build_guide_img/image027.jpg) | ![](build_guide_img/image028.jpg) |
| --- | --- |

After soldering all diodes, clean with rubbing alcohol and use the snips to clip the leads as close to the PCB as possible.

## 7. Solder TRRS Jacks

Solder all 4 TRRS jacks (two  keyboard side) in the locations shown. After soldering, clean with rubbing alcohol.

| ![](build_guide_img/image051.jpg) | ![](build_guide_img/image050.jpg) |
| --- | --- |

## 8. Solder Pogo Pins

**Pay close attention!** The pogo pins go on the bottom side of the PCBs! Look closely at the images below. Don't accidentally solder them on the wrong side of the PCB! In addition, the pogo pins are gendered. The male pogo pins mate with the female pogo pins, so double check that you have them on the correct sides before soldering.

| ![](build_guide_img/image055.jpg) | ![](build_guide_img/image054.jpg) |
| --- | --- |
| ![](build_guide_img/image053.jpg) | ![](build_guide_img/image052.jpg) |

Solder the included pogo pins on the **Bottom Side** of the PCB (same side as the optional LEDs). The male pogo pins go on the **left** half of the keyboard, and the female pins go on the **right** half.

# ⚠️ **STOP** ⚠️

It&#39;s highly recommended that you flash the MCU (Bit-C or Pro Micro) before soldering it so you can be sure it&#39;s working properly. [Jump to step](#firmware_flashing) 22 to flash QMK firmware.

## 9. Solder MCU

Use header pins to solder the MCUs to the keyboard. Fit and solder the BIT-C or Pro Micro MCU as shown below using 0.1" male header pins. After soldering, clean with rubbing alcohol and use the snips to clip the pins as close to the PCB as possible.

| ![](build_guide_img/image056.jpg) | ![](build_guide_img/image057.jpg) |
| --- | --- |

## 10a. [OPTIONAL] Solder rotary encoder(s)

If building with the optional rotary encoders, fit and solder one in each desired position(s) shown. One rotary encoder can be installed directly below the MCU on each side of the board. After soldering, clean with rubbing alcohol and use the snips to clip the pins as close to the PCB as possible. Note that it is **not** necessary to solder the large side support pins on the rotary encoder. **Do not clip the large support pins on the encoder.**

| ![](build_guide_img/image058.jpg) | ![](build_guide_img/image059.jpg) |
| --- | --- |

## 10b. [OPTIONAL] Solder speaker

If building with the optional speaker, fit and solder it in the position shown. The speaker is installed on the left side of the board.  After soldering, clean with rubbing alcohol and use the snips to clip the pins as close to the PCB as possible.

![](build_guide_img/image060.jpg)

## 10c. [OPTIONAL] Solder OLED(s)

If building with the optional OLED displays, fit and solder each in the position each shown. One OLED can be installed on each side of the board above the diodes. After soldering, clean with rubbing alcohol and use the snips to clip the pins as close to the PCB as possible.

| ![](build_guide_img/image061.jpg) | ![](build_guide_img/image062.jpg) |
| --- | --- |

## 11. Insert ICs into IC sockets

⚠️ **Orientation matters!** Make sure that the side of the IC with the round mark is closest to the Bit-C on the left half and furthest from the Bit-C on the right half (both facing left) before inserting. Double check the images below before inserting if you're not sure! The  orientation should match the silkscreen.

![](build_guide_img/image032.jpg)

Carefully bend the IC leads inward so that they are the width of the socket. It helps to set the IC on its side on a flat surface and use a tool to bend all leads at once.

While supporting the back of the PCB with one hand, push on the top of the IC using your thumb until it sits flush in the socket. If you feel leads bending, stop and carefully straighten them before continuing.

| ![](build_guide_img/image063.jpg) | ![](build_guide_img/image064.jpg) |
| --- | --- |

## 12. Choose key layout and configuration

The SNAP PCB includes guide marks for the switches and stabilizers to make their placement easier. The center of each switch lines up with a letter for a particular layout. The tables below show which markings to follow based on key configuration. Familiarize yourself with the [standard layout](http://www.keyboard-layout-editor.com/#/gists/bd48e2fe5b0f571c0034f27cb328d2d7) before soldering. The color coding and markings in the link above match the table below, so refer back to that if needed.

⚠️ **Compatibility note:** Not all combinations are compatible with each other! See the compatibility notes in the table. Double-check that the chosen configuration matches your keycaps before soldering.

![](build_guide_img/image066.jpg)

**Caps lock (light yellow)**
| **Guide Mark** | **Layout Option** |
| --- | --- |
| A | Stepped 1.75U caps lock |
| B | Standard 1.75U caps lock |

**Left shift (dark yellow)**
| **Guide Mark** | **Layout Option** |
| --- | --- |
| C | 2.25U left shift + stab |
| D | 1.25U/1U (ISO) left shift |

**Spacebar (light green)**
| **Guide Mark** | **Layout Option** |
| --- | --- |
| E | 1.25U Fn, 2.25U spacebar + stab |
| F | 2.25U spacebar + stab, 1.25U Fn |

**Right modifiers (purple)**
| **Guide Mark** | **Layout Option** |
| --- | --- |
| G | 5x 1U modifiers + arrows |
| H | 4x 1.25U modifiers and no arrows |

**Right shift (dark green)**
| **Guide Mark** | **Layout Option** |
| --- | --- |
| I | 1.75U + 1U shift + up arrow |
| J | 2.75U shift + stab |

**Enter key**
| **Guide Mark** | **Layout Option** |
| --- | --- |
| K | 1.25U + 1U ISO + stab |
| L | 2.25U ANSI + stab |

**Backspace**
| **Guide Mark** | **Layout Option** |
| --- | --- |
| M | 2U + stab |
| N | 1U + 1U split backspace |

![](build_guide_img/image065.jpg)

# ⚠️ **STOP** ⚠️

It&#39;s highly recommended that you test each key at this point before continuing. If you haven&#39;t already, [Jump to step](#firmware_flashing) 22 to flash QMK firmware. Use a keyboard tester ([this one](https://www.keyboardtester.com/) works) and short the switch pads for each switch using tweezers, a clipped lead from earlier, or something else conductive. If there is an issue, it will be much easier to debug now before everything has been soldered and assembled.

## 13. Screw together M2x3 standoffs using M2x3 screws

In the locations shown, screw the M2x3 standoffs into the bottom side of the **TOP** PCB plate. Fasten using 14 M2x3 screws (7 on each half). Use pliers to hold the standoff steady while tightening the screw. **Do not overtighten!** This step is extra important if you are building with a plate, since it's more difficult to access the screws with the plate in place, so double check this! The standoffs go on the bottom side of the board.

| ![](build_guide_img/image068.jpg) | ![](build_guide_img/image067.jpg) |
| --- | --- |

## 14. Snap in stabilizers

Snap in the PCB-mount stabilizers as shown below. The tab goes in the big hole, and the retaining clips go in the small holes. The stabilizers will only snap in one way. Make sure the stabilizer is fully seated, or the keycap won&#39;t move properly once it&#39;s installed. If using screw-in stabilizers, do **not** use the included washer between the screw and the PCB. The acrylic will not seat properly on top of the washer.

![](build_guide_img/image035.jpg)

## 15. [OPTIONAL] Insert hot-swap sockets

If building with hotswap sockets, drop one into each plated lead hole and affix with tape (masking or electrical tape works well). Alternatively, insert them onto each lead of the PCB mount switch before proceeding.

## 16. Snap in switches

⚠️ **Stop!** Test fit your keycaps to make sure that the switch spacings are correct before soldering, especially the bottom row.

![](build_guide_img/image036.jpg)

If you are using 5-pin PCB mount switches, they may take some force to insert. This is by design. For PCB mount switches, a tight fit makes the switches more stable. Snap in by supporting the back of the PCB, and then pushing hard on the top of the switch. It helps to use a spare keycap on the switch to take some of the pressure off your thumb. After snapping the switch in, make sure it&#39;s sitting flush against the PCB.

Note that some of the switches go in "sideways" and "upside down". This is by design! T, Y, \\, Enter, Backspace, and Caps Lock are all switches that might be installed in different orientations.

If building with hotswap sockets and a switch plate, you will need to remove the switches from the sockets after soldering in order to fit them into the plate for final assembly.

## 17. Solder switches or hot-swap sockets

⚠️ **Stop!** If you are building with a switch plate, make sure that you have installed and tightened the mounting hardware ( **Step 3.13** ) and installed the stabilizers ( **Step 3.14** ) before continuing! Once the switches are installed on the plate, access to the items below is difficult.

Make sure each switch pin has enough solder to form a nice solid joint.

| ![](build_guide_img/image077.jpg) | ![](build_guide_img/image078.jpg) |
| --- | --- |

If building with hotswap sockets and a switch plate, after soldering, insert switches into the switch plate before installing on the PCB. It helps to seat switches in the corner positions on the plate, then insert into the sockets, then insert the remaining switches into the plate and sockets.

## 18. Slide the acrylic spacer onto the standoffs

Peel the backing material off the acrylic spacer. Make sure the acrylic spacer sits flat against the PCB plate. Check for interferences due to leads or solder joints. Trim if needed.

| ![](build_guide_img/image070.jpg) | ![](build_guide_img/image069.jpg) |
| --- | --- |

## 19. Fasten the bottom with M2x3 screws

Place the bottom PCB plate on top of the acrylic spacer. In the same locations where the 14 standoffs were installed, fasten with 14 M2x3 screws (7 on each half). **Do not overtighten!**

| ![](build_guide_img/image072.jpg) | ![](build_guide_img/image071.jpg) |
| --- | --- |

## 20. Fasten M2x10 standoffs from bottom using M2x10 screws

Fasten using 2 M2x10 screws. Use pliers to hold the standoff steady while tightening the screw.

| ![](build_guide_img/image074.jpg) | ![](build_guide_img/image073.jpg) |
| --- | --- |

## 21. Attach the top guard using M2x6 screws

Fasten using 2 M2x6 screws. Don&#39;t overtighten these, as it can crack the top guard.

| ![](build_guide_img/image076.jpg) | ![](build_guide_img/image075.jpg) |
| --- | --- |

## 22. <a name="firmware_flashing"></a> Flash firmware using QMK toolbox

Download either a precompiled binary (only if using a Pro Micro or BIT-C) or the QMK source files from [GitHub](https://github.com/nullbitsco/snap). Using [QMK Toolbox](https://qmk.fm/toolbox/), flash the firmware onto the keyboard. For more information, follow the [Firmware flashing guide](https://github.com/nullbitsco/docs/blob/main/firmware/firmware_flashing.md)

Heads up: both sides of the keyboard need to be flashed for it to work!

## 23. Install keycaps and enjoy!

![](build_guide_img/image079.jpg)

# <a name="troubleshooting"></a> 4. Troubleshooting

Helpful reference pinouts:  
[MCU Pinout (Left)](build_guide_img/image082.jpg)  
[MCU Pinout (Right)](build_guide_img/image083.jpg)  
[OLED Pinout](build_guide_img/image084.jpg)

**None of the keys are working**

- Is the firmware loaded?
- Try with a different USB cable, USB port, and PC.
- If you soldered the LEDs, check that none have been soldered backward. The keyboard will not work if an LED was mistakenly soldered backward.
- Check the direction of the diodes. The back bar should be facing upwards.
- Check the direction of the ICs. The keyboard will not work if they are in the socket backward.
- Check that there are no shorts and that the keyboard is powering up properly. None of the solder joints should be touching each other.

**A single key is not working**

- Check that the switch is soldered properly at both pins.
- Bypass the switch by shorting the two pads with tweezers. If that works, the switch is to blame and should be replaced. If it does not, the diode soldering is likely the issue. You can use the [diode key](https://nullbits.co/static/file/SNAP_diode_key.pdf) to match diodes with a switch!
- Check that all of the diodes are soldered properly at both pins.
- Check that the keymap you are using is defined correctly and matches your keyboard layout.

**A whole row is not working**

- This is usually caused by a cold solder joint at the MCU. Check that all pins on the MCU are soldered properly.
- Check that the proper rows and columns are set in QMK config.h

**A whole column is not working**

- Check that all pins on the MCU are soldered properly.
- Check that the proper rows and columns are set in QMK config.h
- Check that all pins on the ICs are soldered properly.

**The rotary encoder is not working**

- Check that all pins on the rotary encoder are soldered properly.
- Check that the A and B pins are set in QMK config.h and that ENCODER\_ENABLE = yes in QMK rules.mk.

**The OLED is not working**

- Check that all pins on the OLED are soldered properly.
- The OLED is not enabled in the default firmware. Load the 'oled' firmware, available on the QMK repo.

**Two or more keys are swapped**

- Check that the keymap you are using is defined correctly and matches your keyboard layout.

**The underglow LEDs are not working**

- Check that the RGB\_DI\_PIN pin is set in QMK config.h and that RGBLIGHT\_ENABLE = yes in QMK rules.mk.
- Check that all LEDs are soldered in the proper orientation.

**There&#39;s no power**

- Check that all LEDs are soldered in the proper orientation.
- Check the direction of the ICs.
- Check for other shorts – solder blobs, leads that were not clipped all the way, etc.

**How to I do X in firmware?**

- See the QMK docs, or make a post on [r/olkb](https://www.reddit.com/r/olkb/) for help.
- Make a post on the [r/nullbits](https://www.reddit.com/r/nullbits/) subreddit, or join the #firmware channel in the [nullbits discord server](https://discord.gg/eSegJcY).

**Something else?**

- Visit [nullbits.co/support/](https://nullbits.co/support/)
- Reach out at [help@nullbits.co](mailto:help@nullbits.co)
- Join our [Discord](https://discord.gg/eSegJcY)!
