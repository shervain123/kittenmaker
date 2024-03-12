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
### !!! WARNING WIRING MAY BE INACCURATE AND MAY DAMAGE YOUR HARDWARE PLEASE DOUBLE CHECK BEFORE PLUGGING IN POWER AND MAKE SURE TO TEST IT BEFORE SOLDERING INTO THE BOARDS AND DISPLAY

### THE DISPLAY WIRE IS VERY CLOSE TO EACH OTHER PAY ATTENTION DURING SOLDERING AND CHECK WITH MULTIMETER THERE IS NO SHORT

THIS WIRING LIST IS BASED OFF THE CODE AND EXAMPLE FOUND ONLINE

|Item|ESP32  |
|--|--|
|UV LED| GPIO 37 |
|Home switch|GPIO 39|
|**Stepper motor**||
|Pin 1|GPIO 35|
|Pin 2|GPIO 33|
|Pin 3|GPIO 18|
|Pin 4|GPIO 16|
|**SD CARD**||
|(Again may be inaccurate <br> as all these are based off <br> what I could find online)||
|CS|GPIO 1|
|MOSI|GPIO 11|
|CLK|GPIO 7|
|MISO|GPIO 9|
|3v3| 3v3|
|**TFT DISPLAY**||
|MISO|GPIO 9|
|MOSI|GPIO 11|
|SCLK|GPIO 7|
|CS|GPIO 12|
|DC|GPIO 5|
|RST|GPIO3|
### AGAIN WIRING MAYBE INACCURATE ALWAYS DOUBLE CHECK WITH YOUR OWN HARDWARE PINOUT BEFORE TESTING IT
#### THIS IS ALL BASED ON WHAT I COULD TELL AND I HAVEN'T TEST IT OUT YET
If there is any problem pins feel free to let me know

## Building instructions
Not yet finished building but i can add some first
1. Cut a piece of aluminum tape and stick it on the build plate
2. Use aluminum tape to cover the inside light hood to help the light disperse better
3. idk still waiting on parts



## Software

Slicer [Chitubox](https://www.chitubox.com/en/download/chitubox-free)
(Honestly I don't really like it but I don't know any better alternative so I'm stuck with this one)








