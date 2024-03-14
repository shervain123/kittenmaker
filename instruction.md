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

This is the pinout for my display please check with your display first
![wirings](https://github.com/shervain123/kittenmaker/blob/main/images/display%20wiring.png)

## Building instructions
Not yet finished building but i can add some first

tbh this is all over the place so you should just use this as a guide for what parts goes where (I have no idea what im doing)
1. Cut a piece of aluminum tape and stick it on the build plate
2. Use aluminum tape to cover the inside light tunnel to help the light disperse better
	 ![Both build plate and light tunnel](https://github.com/shervain123/kittenmaker/blob/main/images/light%20tunnel%20and%20build%20plate.jpg)
3. Cut out both of the tabs in front (I broke the type c port)
	 ![highlight of the tabs needs to be cut](https://github.com/shervain123/kittenmaker/blob/main/images/before.jpeg)
	 ![after cutting](https://github.com/shervain123/kittenmaker/blob/main/images/cutted%20off%20plastic%20pegs.jpeg)
4. Place your fan and drill a hole for wire and additional holes if necessary
5. Screw your esp32 into the holder using m2x5 and nut
 	![mounted wemos?](https://github.com/shervain123/kittenmaker/blob/main/images/wemos%20with%20holder.jpg)
7. Align in the case and mark the bottom screw hole and drill it out
	![image of me trying to align lol](https://github.com/shervain123/kittenmaker/blob/main/images/1710408055937.jpg)
8. Next screw in your fan and pass the wire through the hole
9. Remove the lcd from the frame, the metal backing can be removed using a flat head screwdriver then gently bend the plastic part backwards to loosen the glue and slow the display will pop out
10. make sure you remove all the backlight component from the display and you should be left with a lcd that is see through dimly
    ![Naked display](https://github.com/shervain123/kittenmaker/blob/main/images/seperated%20display.jpg)
12. pass all the wires and ribbon into the hold on the top case and place the display in it's place DO NOT FORCE IT IN IF IT DOESN'T FIT take it out and cut the edges of the top half NOT THE DISPLAY  
13. Screw in the motor and the micro switch as well (use m2x10 for the switch)
14. Your finished top half should look something like this
	![Top half](https://github.com/shervain123/kittenmaker/blob/main/images/1710408309012.jpg)
15. Then finished the bottom half by soldering the leds, motor controller and fan
16. Then you should solder both the lcd and sd card wires (based on the wiring diagram
17. After checking your connection plug it in  and test is everything worked
18. Screw the board to the bottom case and glue the sd card to the back
	![inside](https://github.com/shervain123/kittenmaker/blob/main/images/inside.jpg) 
19. Then screw in the top case with m2x4 screw
	![completed bottom part](https://github.com/shervain123/kittenmaker/blob/main/images/screws.jpg)
20. Glue the feet to the bottom of the case and put coupler onto the motor
21. add glue to your bic pen and shove it in the hexagon shaped hole on the bottom and insert your lead screw into the coupler
	 ![pencile](https://github.com/shervain123/kittenmaker/blob/main/images/bottom%20completed%20half.jpg)
22. Take the top part and insert your lead screw nut you will need to drill the hole for it 
	![top part](https://github.com/shervain123/kittenmaker/blob/main/images/lead%20screw%20thing.jpg) 
23. Put the 6 bearing in place and use M3 screw to secure it in place (I run out of shorter screw)
	![now with bearings!](https://github.com/shervain123/kittenmaker/blob/main/images/with%20bearings.jpg)
24. Place 4 M3 nut in place and find the longest M3 screw you have to screw it in
	![now with nuts!](https://github.com/shervain123/kittenmaker/blob/main/images/carrage%20with%20screw%20and%20nuts.jpg) 
25. Screw the plastic peg into the screw
	![Pegs](https://github.com/shervain123/kittenmaker/blob/main/images/carrage%20with%20plastic%20thingy.jpg)
26. place the magnet in all the places needs it (vat,case top, build plate and the just fron just now)
27. stick the FEP film on the vat
28. i think that's about it
29. idk still waiting for my magnets


