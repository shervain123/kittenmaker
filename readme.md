
# kittenmaker

*kittenmaker* - an ESP32 based msla 3d printer

*originally created by [NyaCat42](https://github.com/NyanCat42/kittenmaker)*

# Work in progress
Parts list and instruction may be inaccurate and will be change

~ As of currently I'm still waiting for all the parts to arrive ~

~ Parts have arrived and just notice some problems<br> fortunately it's just wrong size of magnet which I have reorder ~

Wiring and pins are based off of online resources and codes

## Features 

- Web interface
- g-code parsing
- mid-print parameter updating
- magnetic, easily removable vat and printbed

## Hardware

 1. 3D printed parts in the [3D models folder](https://github.com/shervain123/kittenmaker/tree/main/3d%20models)
 2.  A Bic Crystal pen or something similar (I used a pencil)
 3. T5 lead screw and nut (the nut needs to be in a rectangle shaped instead of circular shaped)
 4. M2 & M3 screws
 5. 3w UV led 405nm wavelength
 6. A 5v fan with heat sink
 7. FEP film
 8. Bearings (683ZZ or 3x7x3mm) x6
 9. Esp32 S2 mini
 10. 2.4inch tft SPI ILI9341 display (no touch and no adapter board)
 11. Parts for driving the led (can be modified with whatever parts you have like relay)
	 -	IRFZ44N mosfet
	 -	2.2 Ohm 5W resistor
12. ~4x3mm~ 5x2mm magnets x16
13. 28byj-48-5v stepper motor with uln2003 driver
14. Micro switch
15. SD Card reader (NOT DFPlayer)

## 3D models
it is recommended to print with PETG as it is much more UV resistance than PLA but you could try and use UV protective coating on the  parts that are more likely exposed to the UV light

 ~~You will also need to print the legs.3mf and post.3mf 4 times~~ Designed a new feet / fan cover.
 
 Also for some odd reason the original does not include any way to connect the motor to the lead screw but I did find a model in older version of it which I included in the 3D models folder 

Bottom was redesigned to move the SD card and Wemos to a different location to free up some space and included screw points for the bottom feet.

## Instructions
I have decided to split them out you can find them [here](https://github.com/shervain123/kittenmaker/blob/main/instruction.md)

## Known Issue / WIP issue
Faced an issue where ESP32S2 failed to initialized and bootlooping. ~~Issue was caused by a cheap unbranded SD card that does not support SPI~~ (The SD card worked at a later date)(seems like wiring issue on the sd reader) 

Used paint primer to smooth out the resin tray, turns out primer is not resin safe. oops.

Magnet protruding from the bottom of the resin tray caused the FEP film to not seal properly and caused leaks. Might need to edit the model depending on how well your printer prints.

FEP film does NOT stick to any adhesive (tried super glue, hot glue, liquid nail(?) ), only solution that worked is sticking it with double sided tape and sealing around the tray with packing tape. 

Aluminum tape on build plate has a lot of creases, and apparently the adhesive melts in resin. Replaced with flatten soda can cut to size and superglued onto the build plate.

Z axis wobbles left to right while raising / lowering the build plate, not currently fixed and is still a work in progress. 

Benchy was printed as [Bchy](https://github.com/shervain123/kittenmaker/blob/main/images/bchy.jpg) :D


## Software

Slicer [Chitubox](https://www.chitubox.com/en/download/chitubox-free)<br>
[Chitubox v1.8.1](https://sac.chitubox.com/software/download.do?softwareId=17839&softwareVersionId=v1.8.1&fileName=CHITUBOX64Install_V1.8.1.exe)
(Honestly I don't really like it but I don't know any better alternative so I'm stuck with this one)
<br>also if you are using newer version you will need software like uvtools to convert the ctb file to a zip. Older version can save as zip files 









