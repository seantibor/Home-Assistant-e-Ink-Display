# Inkplate 10 Display Home Assistant

An Inkplate 10 (9.7") e-ink display for viewing sensors data from Home Assistant. The firmware is based on ESPHome. I borrowed heavily from I take inspiration **Sainz's** [excellent code](https://github.com/sainz/Home-Assistant-e-Ink-Display) and therefore also from from <b>MaxMac_STN</b>'s work (https://github.com/maxmacstn/HA-ePaper-Display).

![header](https://github.com/sainz/Home-Assistant-e-Ink-Display/blob/master/images/PXL_20220108_093319359.jpg?raw=true)


### Hardware
The unit is an [Inkplate 10 from e-Radionica](https://www.crowdsupply.com/soldered/inkplate-10) with a built-in ESP32 Wifi-chip. I like this board for its built-in ESPHome support and the recycled display. The extra space gives a lot of room for details. 

I printed the frame for the case from the provided designs on the [Inkplate 10 GitHub repo](https://github.com/e-radionicacom/Inkplate-10-hardware/tree/main/3D%20printable%20case/Original%20case) using a roll of [Hatchbox Wood color PLA](https://amzn.to/3jffRJZ). (It's just wood color plastic, so it's not stainable.) I printed on a [Prusa MK3S+](https://www.prusa3d.com/category/original-prusa-i3-mk3s/) and the results were solid.

### Installation
- You need an Home Assistant installation with ESPHome add-on installed;
- I moved around a lot of the text sensors, but some remain from Sainz's code. The sensors.yaml file is linked to configuration.yaml of Home Assistant installation. You must adapt it based on your sensors data;
- Copy fonts folder on your ESPHome folder
- After connect all the hardware together, link it to Home Assistant and flash the firmware (epaper-display.yaml). This is my personal configuration, so you must adaopt based on your Home Assistant configuration and sensors data.
