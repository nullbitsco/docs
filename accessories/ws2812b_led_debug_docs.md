# Troubleshooting WS2812B Underglow LEDs

If one or more LEDs on your device are not lighting up or having other issues, follow the steps in this guide to troubleshoot the issue.

## Step 1: Reflow Solder

The most common cause of LEDs not glowing is because the LED pins aren't connected properly with solder. In this case reflowing solder to the pins
usually fixes the connection. Please note you will have to reflow solder both on the LED that is not working and the one preceeding it on the LED 
order diagram as shown below. This is because the LEDs are linked in a chain, so if an LED is not glowing that could mean it isn't connected to the previous one.

![image](https://user-images.githubusercontent.com/6137765/129141693-ae71cea2-8081-4782-a9dc-843990ce4ad9.png)
![image](https://user-images.githubusercontent.com/6137765/129141684-d81d16da-379f-41e7-ab3c-63f960b789c4.png)

## Step 2: Check Connections with Multimeter

If you aren't familiar with using a multimeter, [watch this](https://www.youtube.com/watch?v=SECWePatYjY) to learn the basics.

Here are the pin diagrams for the MCU and LEDs. We'll be using these to identify what pins to check. 

![image](https://user-images.githubusercontent.com/6137765/129142514-3b07697e-9229-491a-b1fb-a5cdc2bd6641.png)

**UNPLUG** your board and follow these steps to check your pin connections.

1. Check that the LED's VDD pin has continuity to the MCU's +5V pin as show in the pin diagram above.
    * REMINDER: The pins readout for the MCU will be “flipped” since the diagram shows the top view but you'll be looking at the bottom of the MCU.
2. Check continuity of the LED's VSS pin to the ground pin (GND0 or GND1) on the MCU.
3. Check continuity of the first not-glowing LED's DI pin to the previous LED's DO pin. 
If this is very first LED in the chain then check continuity between the LED's DI pin and the MCU's RGB_2812 pin.

If any of the pins are not connected, resolder them and check your LEDs again. 

## Connections are fine but LEDs still don't glow?
This might occur if had previously flashed a firmware that disabled the LEDs on your device. MCUs persist certain settings across firmware flashes and underglow LED state is one of them. Use the "Clear EEPROM" option in QMK Toolbox and reflash your device. If your LEDs still do not glow, it you might have a defective LED on your hands. 

At this point we recommend you hop into our [Discord](https://discord.gg/eSegJcY) for additional troubleshooting support.
