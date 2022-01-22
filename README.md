# RATMIPAD

Ratmi is multi layout macropad supports six analog potentiometer, two rotary encoders, 3.5mm TRS socket for sending out serial data like midi output and more. The firmware is fully QMK, see [build environment setup](https://docs.qmk.fm/#/getting_started_build_tools) then the [make instructions](https://docs.qmk.fm/#/getting_started_make_guide) for more information. 
The analog potentiometer outputs a midi signal which can be recognized by any software reads midi input. For hardware midi controller the PCB has 3.5mm TRS female socket footprint ( 3.5mm TRS male jack to 5-pin midi midi cable as connector required ), for this specific purpose the programaing code can be done with arduinoIDE.

Designer and maintainer: [sandipratama/nendezkombet](https://github.com/nendezkombet) 


![DSC04817](https://user-images.githubusercontent.com/82454371/150630727-42b04696-4c57-4079-88c4-db2a9ac5d35e.jpg)

![DSC04809](https://user-images.githubusercontent.com/82454371/150630732-6e4a5c95-a508-4664-8c4d-1ff9fe7a1c56.jpg)


## Table of contents

- [Features](#features)
- [Default Layout](#default-layout)
- [Optional Layout](#optional-layout)
- [PCB](#pcb)
- [BOM](#bom)
- [Case](#case)
- [Assembly Guide](#assembly-guide)
- [Firmware](#firmware)


## Features


- Cheap to build.
- Multi layout support.
- Easy to source components.
- Easy to build.
- MX style switch and Kailh low profile V2 switch compatible
- Arduino Pro Micro powered.
- QMK compatible.
- RGB backlighting support (optional).
- Up to two rotary encoder support.
- Hardware midi controller support.
- Battery powered support ( as portable controller ).
- Completely open-source.


## Default Layout


![Screenshot 2022-01-22 171054](https://user-images.githubusercontent.com/82454371/150634974-43f5ce20-520c-4ecf-b685-a5e6a9a79136.png)


## Optional Layout 


![Screenshot 2022-01-22 172756](https://user-images.githubusercontent.com/82454371/150634990-3c94788f-6693-495a-a578-00850d2df288.png)

From left to right layout configuration :

1. 1x big encoder knob with 6x key switch.
2. 9x key switch.
3. 2x small encoder knob with 7x key switch.
4. 1x big encoder knob with 6x analog potentiometer.


## PCB


Top view


![upper](https://user-images.githubusercontent.com/82454371/150636799-4c5a5ed7-6855-46f0-90fe-4ed2c280f6ce.png)


Bottom view


![bottom](https://user-images.githubusercontent.com/82454371/150636808-75d68e0a-db87-46cb-b2ee-3d14b719f42a.png)


## BOM

|Parts|Footprint|Quantity|
|:---|:---|:---|
|WS2812B RGB LED |5050|8|
|100nF capacitor|0805|8|
|MX switch or Kailh low V2 switch |3 or 5 pin|9|
|Rotary encoder|EC11|2|
|Arduino Promicro |32u4|1|
|10K pullup resistor (optional)|0805 or axial|9|
|220ohm resistor|0805 or axial|3|
|Reset button switch |6mm*2.5mm|1|
|B10K Analog potentiometer (optional) | RV09 or RK09|6|
|3.5mm TRS female socket (optional) |PJ313|1|
|Micro slide switch (optional)|MSS22D18 |1|
|9V battery (optional) ||1|
|10mm M2 "MALE TO FEMALE" brass standoff|round knurled|4|
|10mm M2 "FEMALE TO FEMALE" brass standoff|round knurled|4|
|5mm M2 screw|-|8|
|3.5mm TRS jack to 5-pin midi din male socket (optional) |see detail below|1|


![51kXivjBTuL _AC_SX425_](https://user-images.githubusercontent.com/82454371/150636116-4ee8e17d-2fe3-4c75-84c9-792c8be12903.jpg)


you can build by your self, wiring instruction can by found in the google search engine.


## Case

Stacked acrylic case 


![DSC04837](https://user-images.githubusercontent.com/82454371/150636476-ca4dd9e8-aa27-4ff9-9fa8-5f2157010b53.jpg)


![DSC04840](https://user-images.githubusercontent.com/82454371/150636525-73c4b8e4-4978-475d-8bf5-532a54f16a95.jpg)


## Assembly Guide

Will be update soon !!!


## Firmware

Firmware flashing :

Open QMK Toolbox and locate The .hex file you compiled before or use ready flash default keymap

Enter the bootloader :

Briefly press the button twice on the small hole located in the top of the encoder with simcard ejector pin than hit flash 

