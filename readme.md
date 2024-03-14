# kittenmaker

*kittenmaker* - an ESP32 based msla 3d printer

*originally created by [NyaCat42](https://github.com/NyanCat42/kittenmaker)*

# Work in progress
Parts list and instruction may be inaccurate and will be change

~As of currently I'm still waiting for all the parts to arrive~

Parts have arrived and just notice some problems<br> fortunately it's just wrong size of magnet which I have reorder 

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

 You will also need to print the legs.3mf and post.3mf 4 times
 
 Also for some odd reason the original does not include any way to connect the motor to the lead screw but I did find a model in older version of it which I included in the 3D models folder 

## Wiring
### !!! WARNING ALWAYS DOUBLE CHECK WIRING BEFORE PLUGGING IN POWER AND MAKE SURE TO TEST IT BEFORE SOLDERING INTO THE BOARDS AND DISPLAY

### THE DISPLAY WIRE IS VERY CLOSE TO EACH OTHER PAY ATTENTION DURING SOLDERING AND CHECK WITH MULTIMETER THERE IS NO SHORT

The wiring is based on the code and my testing

|Item|ESP32  |
|--|--|
|UV LED| GPIO 37 |
|Home switch <br>(low trigger)|GPIO 39|
|**Stepper motor**||
|Pin 1|GPIO 35|
|Pin 2|GPIO 33|
|Pin 3|GPIO 18|
|Pin 4|GPIO 16|
|**SD CARD**||
|CS|GPIO 1|
|MOSI|GPIO 11|
|CLK|GPIO 7|
|MISO|GPIO 9|
|3v3| 3v3|
|**TFT DISPLAY**||
|MISO(SDO)|GPIO 9|
|MOSI(SDI)|GPIO 11|
|SCLK(SCL)|GPIO 7|
|CS(CSX)|GPIO 12|
|DC|GPIO 5|
|RST|GPIO3|

If there is any problem feel free to let me know

## Building instructions
Not yet finished building but i can add some first

tbh this is all over the place so you should just use this as a guide for what parts goes where (I have no idea what im doing)
1. Cut a piece of aluminum tape and stick it on the build plate
2. Use aluminum tape to cover the inside light tunnel to help the light disperse better
	 ![Both build plate and light tunnel](link)
3. Cut out both of the tabs in front (I broke the type c port)
	 ![highlight of the tabs needs to be cut](a)
	 ![after cutting](a)
4. Place your fan and drill a hole for wire and additional holes if necessary
5. Screw your esp32 into the holder using m2x5 and nut
6. Align in the case and mark the bottom screw hole and drill it out
	![image of me trying to align lol](a)
7. Next screw in your fan and pass the wire through the hole
8. Remove the lcd from the frame, the metal backing can be removed using a flat head screwdriver then gently bend the plastic part backwards to loosen the glue and slow the display will pop out
9. make sure you remove all the backlight component from the display and you should be left with a lcd that is see through dimly 
10. pass all the wires and ribbon into the hold on the top case and place the display in it's place DO NOT FORCE IT IN IF IT DOESN'T FIT take it out and cut the edges of the top half NOT THE DISPLAY  
11. Screw in the motor and the micro switch as well (use m2x10 for the switch)
12. Your finished top half should look something like this
	![Top half](a)
13. Then finished the bottom half by soldering the leds, motor controller and fan
14. Then you should solder both the lcd and sd card wires (based on the wiring diagram
15. After checking your connection plug it in  and test is everything worked
16. Screw the board to the bottom case and glue the sd card to the back
	![inside](a) 
17. Then screw in the top case with m2x4 screw
	![completed bottom part](a)
18. Glue the feet to the bottom of the case and put coupler onto the motor
19. add glue to your bic pen and shove it in the hexagon shaped hole on the bottom and insert your lead screw into the coupler
	 ![pencile](a)
20. Take the top part and insert your lead screw nut you will need to drill the hole for it 
	![top part](a) 
21. Put the 6 bearing in place and use M3 screw to secure it in place (I run out of shorter screw)
	![now with bearings!](a)
22. Place 4 M3 nut in place and find the longest M3 screw you have to screw it in
	![now with nuts!](a) 
23. Screw the plastic peg into the screw
	![Pegs](a)
24. place the magnet in all the places needs it (vat,case top, build plate and the just fron just now)
25. stick the FEP film on the vat
26. i think that's about it
27. idk still waiting for my magnets



## Software

Slicer [Chitubox](https://www.chitubox.com/en/download/chitubox-free)<br>
[Chitubox v1.8.1](https://sac.chitubox.com/software/download.do?softwareId=17839&softwareVersionId=v1.8.1&fileName=CHITUBOX64Install_V1.8.1.exe)
(Honestly I don't really like it but I don't know any better alternative so I'm stuck with this one)
<br>also if you are using newer version you will need software like uvtools to convert the ctb file to a zip. Older version can save as zip files









