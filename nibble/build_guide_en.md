# NIBBLE

### Customizable 65% Keyboard Kit

![](https://github.com/nullbitsco/docs/raw/main/nibble/build_guide_img/image000.jpg)

### Assembly Instructions

## 1. Thanks for purchasing!

Seriously, thank you! The NIBBLE has been a passion project of mine over the past year. I&#39;ve been using a NIBBLE in its various stages of development and think it&#39;s a great keyboard that you&#39;ll love. I&#39;ve designed and assembled the kits during my free time, and I want to make sure you have a great experience. If at any point you hit a snag or have a question, feel free to let me know via email or Reddit DM. I&#39;ll make sure it&#39;s taken care of.

# 1. Helpful links [TODO!]
* Soldering
* How to use a DMM

# 1. Parts and tools

![](https://github.com/nullbitsco/docs/raw/main/nibble/build_guide_img/image001.jpg)

## 1. Parts included in the kit

### Hardware
| **Item** | **Qty.** | **Image** |
| --- | --- | --- |
| Standoff, M2x3 | 13 | ![](https://github.com/nullbitsco/docs/raw/main/nibble/build_guide_img/image002.jpg) |
| Standoff, M2x3 | 2 | ![](https://github.com/nullbitsco/docs/raw/main/nibble/build_guide_img/image004.jpg) |
| Screw, M2x3 | 26 | ![](https://github.com/nullbitsco/docs/raw/main/nibble/build_guide_img/image006.jpg) |
| Screw, M2x6 | 2 | ![](https://github.com/nullbitsco/docs/raw/main/nibble/build_guide_img/image008.jpg) |
| Screw, M2x10 | 2 | ![](https://github.com/nullbitsco/docs/raw/main/nibble/build_guide_img/image010.jpg) |
| Machined Knob | 1 | ![](https://github.com/nullbitsco/docs/raw/main/nibble/build_guide_img/image046.jpg) |

### Electronics
| **Item** | **Qty.** | **Image** |
| --- | --- | --- |
| 1N4148 Diode | 73 | ![](https://github.com/nullbitsco/docs/raw/main/nibble/build_guide_img/image003.jpg) |
| 0.1μF Capacitor | 2 | ![](https://github.com/nullbitsco/docs/raw/main/nibble/build_guide_img/image005.jpg) |
| 330Ω Resistor | 3 | ![]() |
| IC Socket | 2 | ![](https://github.com/nullbitsco/docs/raw/main/nibble/build_guide_img/image007.jpg) |
| IC (74HC138N) | 2 | ![](https://github.com/nullbitsco/docs/raw/main/nibble/build_guide_img/image009.jpg) |
| Reset Switch | 1 | ![](https://github.com/nullbitsco/docs/raw/main/nibble/build_guide_img/image011.jpg) |
| WS2812B LED | 10 | ![](https://github.com/nullbitsco/docs/raw/main/nibble/build_guide_img/image042.jpg) | 
| TRRS Jack | 1 | ![](https://github.com/nullbitsco/docs/raw/main/nibble/build_guide_img/image043.jpg) |
| Rotary Encoder | 1 | ![](https://github.com/nullbitsco/docs/raw/main/nibble/build_guide_img/image044.jpg) |
| Big RGB LED | 1 | ![](https://github.com/nullbitsco/docs/raw/main/nibble/build_guide_img/image045.jpg) |

### Core

| **Item** | **Qty.** | **Image** |
| --- | --- | --- |
| Top PCB plate | 1 | ![](https://github.com/nullbitsco/docs/raw/main/nibble/build_guide_img/image012.jpg) |
| Bottom PCB plate | 1 | ![](https://github.com/nullbitsco/docs/raw/main/nibble/build_guide_img/image013.jpg) |
| Middle acrylic spacer | 1 | ![](https://github.com/nullbitsco/docs/raw/main/nibble/build_guide_img/image014.jpg) |
| Top acrylic guard | 1 | ![](https://github.com/nullbitsco/docs/raw/main/nibble/build_guide_img/image015.jpg) |

  1.
## Parts you provide

- PCB-mount switches (Cherry MX footprint)
- PCB-mount stabilizers
- Keycaps
- BIT-C or other Pro Micro MCU
- **[Optional]** Qty. 144 Mill-Max 0305 or 7305 hot-swap solder sockets
- **[Optional]** FR4 switch plate

  1.
## Add-ons and extras

- WS2812B RGB LED underglow
- Rotary encoder &amp; knob
- Big RGB LED &amp; required resistors
- SSD1306 OLED display
- TRRS expansion jack for future numpad support

  1.
## Tools required

- Fine-tip soldering iron &amp; solder
- Needle nose pliers
- Phillips #0 screwdriver
- Snips for cutting leads
- Rubbing alcohol

1.
# Assembly Steps

⚠️ **Important!** Notes marked with this icon are crucial, so be sure to read them carefully before moving on.

Steps marked [OPTIONAL] aren&#39;t required for the base kit, but may be needed depending on what you choose to include in your build.

  1.
## [optional] Solder underglow LEDS

Solder the 10x WS2812B underglow LEDs. Start by tacking down one corner, and then soldering the remaining 3 leads. After soldering, clean with rubbing alcohol.

⚠️ **Orientation matters!** These parts have a small angled mark which should match up with the one on the PCB. If you don&#39;t get the orientation right, the LEDs will not work, and your keyboard may not boot up.

![](RackMultipart20210210-4-1pg77zq_html_626e117ff25b07db.jpg)

  1.
## [optional] bend and solder resistors for big LED

This step is only required if using the optional big LED in place of one of the macro keys. Bend and solder R1, R2, and R3.

| ![](RackMultipart20210210-4-1pg77zq_html_afbcddce7a095032.gif) ![](RackMultipart20210210-4-1pg77zq_html_c4f8947a0b66e07d.gif) | ![](RackMultipart20210210-4-1pg77zq_html_707c56cd24c1db62.png) |
| --- | --- |

After soldering, clean with rubbing alcohol and use the snips to clip the leads as close to the PCB as possible.

  1.
## Solder reset switch

Fit and solder the reset switch as shown below.

| ![](RackMultipart20210210-4-1pg77zq_html_afbcddce7a095032.gif) ![](RackMultipart20210210-4-1pg77zq_html_357eecf6ed02b863.gif) | ![](RackMultipart20210210-4-1pg77zq_html_bc5fe8eacf8ff842.jpg) |
| --- | --- |

After soldering, clean with rubbing alcohol.

  1.
## Solder IC sockets

Fit and solder the two IC sockets. Be sure to match the notch in the socket with the one on the PCB. After soldering, clean with rubbing alcohol.

⚠️ **Do not solder the socket with the IC inserted!** The high heat may damage the chip if it is in the socket during soldering.

| ![](RackMultipart20210210-4-1pg77zq_html_a353e99f1e6bf155.gif) ![](RackMultipart20210210-4-1pg77zq_html_3cbc8a5f64e4fb57.gif) | ![](RackMultipart20210210-4-1pg77zq_html_1ef5ac4a1ff1d527.jpg) |
| --- | --- |

  1.
## Solder caps

Fit and solder the two capacitors.

| ![](RackMultipart20210210-4-1pg77zq_html_c3ee71fa1be12ebe.gif) ![](RackMultipart20210210-4-1pg77zq_html_c3ee71fa1be12ebe.gif) ![](RackMultipart20210210-4-1pg77zq_html_3cbc8a5f64e4fb57.gif) | ![](RackMultipart20210210-4-1pg77zq_html_3eb238f0b5a5d65.jpg) |
| --- | --- |

After soldering, clean with rubbing alcohol and use the snips to clip the leads as close to the PCB as possible.

  1.
## Bend and solder diodes

Bend and fit the 1N4148 diodes. In order to get uniform placement of the diodes, I recommend using a diode bending tool. You can buy one or 3D print one. [Here&#39;s a link to my favorite](https://www.thingiverse.com/thing:4332520). Bend the leads inward to hold the diodes in place when the PCB is turned upside down. Begin by soldering one side of the diodes and adjust the diode alignment to your liking before soldering the second lead.

⚠️ **Orientation matters!** Solder the diodes with the black bar **UP** as shown in the images. The keyboard will not work if they are backward.

| ![](RackMultipart20210210-4-1pg77zq_html_c3f49cf624ddc4a7.jpg) | ![](RackMultipart20210210-4-1pg77zq_html_acdab3a0e651fd98.gif) |
| --- | --- |

There is one special case – the second to last diode has a top-mount pad, in order to fit the expansion jack below. Cut one lead as shown below, so that it rests evenly on the PCB fit into the mounting hole.

![](RackMultipart20210210-4-1pg77zq_html_222bdfb1e59c8b2d.png)

Solder the short end of the diode that was just trimmed on the **top** side of the PCB. Once all diodes are soldered, it should be virtually unnoticeable from the rest. After soldering all 72 diodes, clean with rubbing alcohol and use the snips to clip the leads as close to the PCB as possible.

⚠️

# **STOP!**

It&#39;s highly recommended that you flash the MCU (Bit-C or Pro Micro) before soldering it so you can be sure it&#39;s working properly. Jump to step 20 to flash QMK firmware.

  1.
## Solder MCU

Fit and solder the BIT-C or Pro Micro MCU as shown below. After soldering, clean with rubbing alcohol and use the snips to clip the pins as close to the PCB as possible.

![](RackMultipart20210210-4-1pg77zq_html_d0a50e0b682c5cdb.png)

  1.
## [optional] solder rotary encoder, big led, and/or oled

If building with the optional rotary encoder, big LED, or OLED display, in place of the programmable macro keys, fit and solder each in the position each shown. After soldering, clean with rubbing alcohol and use the snips to clip the pins as close to the PCB as possible. Do not clip the large support pins on the encoder.

⚠️ **Compatibility note:** the OLED display and big RGB LED share a signal line. It&#39;s recommended to use either the big LED or the OLED. They can both be used at the same time, but the blue LED will be dimly illuminated when the I2C display is in use.

| ![](RackMultipart20210210-4-1pg77zq_html_4ff125727a51216f.gif) | ![](RackMultipart20210210-4-1pg77zq_html_7628030166b1e8e0.gif) | ![](RackMultipart20210210-4-1pg77zq_html_701062075f5916e4.gif) |
| --- | --- | --- |

After soldering, clean with rubbing alcohol and use the snips to clip the leads as close to PCB as possible.

  1.
## Insert ICs into IC sockets

⚠️ **Orientation matters!** Make sure that the round mark on the IC is aligned with the round mark on the IC socket before inserting.

Carefully bend the IC leads inward so that they are the width of the socket. It helps to set the IC on its side on a flat surface and use a tool to bend all leads at once.

While supporting the back of the PCB with one hand, push on the top of the IC using your thumb until it sits flush in the socket. If you feel leads bending, stop and carefully straighten them before continuing.

![](RackMultipart20210210-4-1pg77zq_html_4d57da390193f807.jpg)

  1.
## Choose key layout and configuration

The NIBBLE includes guide marks for switches and stabilizers to make their placement easier. The center of each switch lines up with a letter for a particular layout. The tables below show which markings to follow based on key configuration. Familiarize yourself with the [standard layout](https://nullbits.co/nibble/layout.html) and the [function row options](https://nullbits.co/nibble/layout_fn.html).

⚠️ **Compatibility note:** Not all combinations are compatible with each other. See the compatibility notes in the table. Double-check that the chosen configuration matches your keycaps before soldering.

⚠️

# **STOP!**

It&#39;s highly recommended that you test each key at this point before continuing. If you haven&#39;t already, jump to step 20 to flash QMK firmware. Use a keyboard tester ([this one](https://www.keyboardtester.com/) works) and short the switch pads for each switch using tweezers, a clipped lead from earlier, or something else conductive. If there is an issue, it will be much easier to debug now before everything has been soldered and assembled.

**Caps lock**** Left modifiers**

| **Guide Mark** | **Layout Option** |
 | **Guide Mark** | **Layout Option** |
| --- | --- | --- | --- | --- |
| A | Stepped 1.75U Caps Key |
 | C | 3x 1.25U Modifiers |
| B | Standard 1.75U Caps Key |
 | D | 2x 1.5U Modifiers |

**Spacebar**** Right modifiers**

| **Guide Mark** | **Layout Option** |
 | **Guide Mark** | **Layout Option** |
| --- | --- | --- | --- | --- |
| E | 6.25U spacebar _ **Only compatible with &quot;C&quot;** _ |
 | H | 3x 1U Modifiers |
| F | 7U spacebar_ **Only compatible with &quot;D&quot;** _ |
 | I | 2x 1.5U Modifiers_ **Recommended when using &quot;G&quot;** _ |
| G | 2.75U + 1U + 2.25 split spacebar _ **Only compatible with &quot;C&quot;** _ |
 |
 |
 |

**Left Shift (Rev2 Only)****Enter Key (Rev2 Only)**

| **Guide Mark** | **Layout Option** |
 | **Guide Mark** | **Layout Option** |
| --- | --- | --- | --- | --- |
| J | 2.25U ANSI |
 | L | 2.25U ANSI |
| K | 1.25U + 1U ISO |
 | M | 1.25U + 1U ISO |

![](RackMultipart20210210-4-1pg77zq_html_bc33fb3f4b0a2a35.jpg)

  1.
## Screw together M2x3 standoffs using M2x3 screws

In the locations shown, screw the M2x3 standoffs into the **TOP** PCB plate. Fasten using 13 M2x3 screws. Use pliers to hold the standoff steady while tightening the screw. **Do not overtighten!**

![](RackMultipart20210210-4-1pg77zq_html_6f121cb6d989458a.gif) ![](RackMultipart20210210-4-1pg77zq_html_c7b64e8fc4a2814f.gif) ![](RackMultipart20210210-4-1pg77zq_html_c7b64e8fc4a2814f.gif) ![](RackMultipart20210210-4-1pg77zq_html_6f121cb6d989458a.gif) ![](RackMultipart20210210-4-1pg77zq_html_6f121cb6d989458a.gif) ![](RackMultipart20210210-4-1pg77zq_html_c7b64e8fc4a2814f.gif) ![](RackMultipart20210210-4-1pg77zq_html_c7b64e8fc4a2814f.gif) ![](RackMultipart20210210-4-1pg77zq_html_c7b64e8fc4a2814f.gif) ![](RackMultipart20210210-4-1pg77zq_html_6f121cb6d989458a.gif) ![](RackMultipart20210210-4-1pg77zq_html_6f121cb6d989458a.gif) ![](RackMultipart20210210-4-1pg77zq_html_c7b64e8fc4a2814f.gif) ![](RackMultipart20210210-4-1pg77zq_html_6f121cb6d989458a.gif) ![](RackMultipart20210210-4-1pg77zq_html_6f121cb6d989458a.gif) ![](RackMultipart20210210-4-1pg77zq_html_467e8e9dd76c1446.jpg)

  1.
## Snap in stabilizers

Snap in the PCB-mount stabilizers as shown below. The tab goes in the big hole, and the retaining clips go in the small holes. The stabilizers will only snap in one way. Make sure the stabilizer is fully seated, or the keycap won&#39;t move properly once it&#39;s installed.

![](RackMultipart20210210-4-1pg77zq_html_54067db1e191a056.jpg)

  1.
## [optional] Insert hot-swap sockets

If building with hotswap sockets, drop one into each plated lead hole. Alternatively, insert them onto each lead of the PCB mount switch before proceeding.

  1.
## Snap in switches

⚠️ **Stop!** Test fit your keycaps to make sure that the switch spacings are correct before soldering, especially the bottom row.

If you are using 5-pin PCB mount switches, they may take some force to insert. This is by design. For PCB mount switches, a tight fit makes the switches more stable. Snap in by supporting the back of the PCB, and then pushing hard on the top of the switch. It helps to use a spare keycap on the switch to take some of the pressure off your thumb. After snapping the switch in, make sure it&#39;s sitting flush against the PCB.

![](RackMultipart20210210-4-1pg77zq_html_6fbe29b2eee1b271.jpg)

  1.
## Solder switches or hot-swap sockets

⚠️ **Stop!** If you are building with a switch plate, make sure that you have installed and tightened the mounting hardware ( **Step 2.11** ) and installed the stabilizers ( **Step 2.12** ) before continuing! Once the switches are installed on the plate, access to the items below is difficult.

Make sure each switch pin has enough solder to form a nice solid joint.

  1.
## Slide the acrylic spacer onto the standoffs

Make sure the acrylic spacer sits flat against the PCB plate. Check for interreferences due to leads or solder joints. Trim if needed.

![](RackMultipart20210210-4-1pg77zq_html_661bac1ddd37a5c2.jpg)

  1.
## Fasten the bottom with M2x3 screws

Place the bottom PCB plate on top of the acrylic spacer. In the same locations where the 13 standoffs were installed, fasten with 13 M2x3 screws. **Do not overtighten!**

![](RackMultipart20210210-4-1pg77zq_html_2ca7e3d879c21466.jpg)

  1.
## Fasten M2x10 standoffs from bottom using M2x10 screws

Fasten using 2 M2x10 screws. Use pliers to hold the standoff steady while tightening the screw.

![](RackMultipart20210210-4-1pg77zq_html_8e6fbbece5b06f53.jpg)

  1.
## Attach the top guard using M2x6 screws

Fasten using 2 M2x6 screws. Don&#39;t overtighten these, as it can crack the top guard.

![](RackMultipart20210210-4-1pg77zq_html_d2ff77e9f97b4246.jpg)

  1.
## Flash firmware using QMK toolbox

Download either a precompiled binary (only if using a Pro Micro or BIT-C) or the QMK source files from [GitHub](https://github.com/nullbitsco/nibble). Using [QMK Toolbox](https://qmk.fm/toolbox/), flash the firmware onto the keyboard.

  1.
## Enjoy!

![](RackMultipart20210210-4-1pg77zq_html_f5f3023eec63b11c.jpg)

1.
# Troubleshooting

**None of the keys are working**

- Is the firmware loaded?
- Check the direction of the diodes. The back bar should be facing upwards.
- Check the direction of the ICs. The keyboard will not work if they are in the socket backward.
- Check that there are no shorts and that the keyboard is powering up properly.

**A single key is not working**

- Check that all of the diodes are soldered properly at both pins.
- Check that the switch is soldered properly at both pins.
- Check that the keymap you are using is defined correctly and matches your keyboard layout.

**A whole row is not working**

- Check that all pins on the MCU are soldered properly.
- Check that the proper rows and columns are set in QMK config.h

**A whole column is not working**

- Check that all pins on the MCU are soldered properly.
- Check that the proper rows and columns are set in QMK config.h
- Check that all pins on the ICs are soldered properly.

**The rotary encoder is not working**

- Check that all pins on the rotary encoder are soldered properly.
- Check that the A and B pins are set in QMK config.h and that ENCODER\_ENABLE = yes in QMK rules.mk.

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

- See the QMK docs, or make a post on r/olkb for help.
- Send me a PM on Reddit or an email, and I&#39;ll try to help.

**Something else?**

- Visit [nullbits.co/support/](https://nullbits.co/support/)
- Reach out at [help@nullbits.co](mailto:help@nullbits.co)
- Message [u/jaygreco](https://www.reddit.com/user/Jaygreco) on Reddit
- Join our [Discord](https://discord.gg/eSegJcY)!

NIBBLE 0x3 Assembly Instructions Rev03 10.22.20
