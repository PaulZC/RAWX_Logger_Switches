# RAWX_Logger_Switches

A switch PCB for the [ZED-F9P_FeatherWing](https://github.com/PaulZC/ZED-F9P_FeatherWing) and
[ZED-F9P_FeatherWing_USB](https://github.com/PaulZC/ZED-F9P_FeatherWing_USB)

![Switches](https://github.com/PaulZC/RAWX_Logger_Switches/blob/master/img/Switches.JPG)

![PCBs](https://github.com/PaulZC/RAWX_Logger_Switches/blob/master/img/PCBs.JPG)

Contains:

### Three slide switches:
- ON/OFF power control (pulls the EN line low to disable the 3.3V regulators on the FeatherWing and the Adalogger)
- Base/Rover mode (pulls A0 low for Base mode, leaves it floating for Rover mode)
- Survey_In mode (pulls A3 low to enable Survey_In (RTCM) mode when in Base mode)

### Two push button switches:
- EVENT (pulls A2 (ZED-F9P EXTINT) pin low to create a TIM_TM2 event message)
- STOP (pulls A1 low to stop logging and close the log file)

### NeoPixel:
- Indicates the status of the Logger

![Dimensions](https://github.com/PaulZC/RAWX_Logger_Switches/blob/master/img/Dimensions.PNG)

![Top](https://github.com/PaulZC/RAWX_Logger_Switches/blob/master/img/Top.JPG)

![Bottom](https://github.com/PaulZC/RAWX_Logger_Switches/blob/master/img/Bottom.JPG)

Based extensively on the Adafruit Feather(Wing) product range

The Eagle files are available in the [Eagle folder](https://github.com/PaulZC/RAWX_Logger_Switches/tree/master/Eagle)

The schematic is available [here](https://github.com/PaulZC/RAWX_Logger_Switches/blob/master/img/Schematic.PNG)

## BOM

- The ON/OFF, BASE/ROVER and SURVEY_IN slide switches are: E-Switch part EG1218 (Farnell / Element14 part 2787232)
- The EVENT and STOP push switches are: e.g. Multicomp MCDTS6-1N 160gf (Farnell / Element14 part 9471685)
- LED1 is a Sparkfun / Worldsemi WS2812B NeoPixel (Mouser part 474-COM-13667)
- LED2 is an 0805 (2.0x1.25mm) red LED: e.g. Wurth Electronik 150080RS75000 (Farnell / Element14 part 2322077)
- R1 is a generic 0805 or 0603 1K resistor: e.g. Multicomp MCWR06X1001FTL (Farnell / Element14 part 2447272)
- C1 and C2 are generic 0603 0.1uF (100nF) ceramic capacitors: e.g. Murata GRM188R71H104JA93D (Farnell / Element14 part 2688523)

LED2 and R1 are optional if you are using the NeoPixel

## Acknowledgements

This project would not have been possible without the open source designs kindly provided by Adafruit.

Adafruit invests time and resources providing this open source design, please support Adafruit and open-source hardware by purchasing products from Adafruit!

## Licence

This project is distributed under a Creative Commons Attribution + Share-alike (BY-SA) licence.
Please refer to section 5 of the licence for the "Disclaimer of Warranties and Limitation of Liability".

Enjoy!

**_Paul_**

