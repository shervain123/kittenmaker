[here](https://github.com)

## Wiring

### !!! WARNING ALWAYS DOUBLE CHECK WIRING BEFORE PLUGGING IN POWER AND MAKE SURE TO TEST IT BEFORE SOLDERING INTO THE BOARDS AND DISPLAY

### THE DISPLAY WIRE IS VERY CLOSE TO EACH OTHER PAY ATTENTION DURING SOLDERING AND CHECK WITH MULTIMETER THERE IS NO SHORT

The wiring is based on the code and my testing

| Item                              | ESP32   |
| --------------------------------- | ------- |
| UV LED                            | GPIO 37 |
| Home switch `<br>`(low trigger) | GPIO 39 |
| **Stepper motor**           |         |
| Pin 1                             | GPIO 35 |
| Pin 2                             | GPIO 33 |
| Pin 3                             | GPIO 18 |
| Pin 4                             | GPIO 16 |
| **SD CARD**                 |         |
| CS                                | GPIO 1  |
| MOSI                              | GPIO 11 |
| CLK                               | GPIO 7  |
| MISO                              | GPIO 9  |
| 3v3                               | 3v3     |
| **TFT DISPLAY**             |         |
| MISO(SDO)                         | GPIO 9  |
| MOSI(SDI)                         | GPIO 11 |
| SCLK(SCL)                         | GPIO 7  |
| CS(CSX)                           | GPIO 12 |
| DC                                | GPIO 5  |
| RST                               | GPIO3   |

If there is any problem feel free to let me know

This is the pinout for my display please check with your display first
![wirings](https://github.com/shervain123/kittenmaker/blob/main/images/display%20wiring.png)

## Building instructions

This instructions is for the new bottom which I have modified from the original and with the help of tormenmashi_

If you want to follow with the original instruction, it can be found [here](https://github.com/shervain123/kittenmaker/blob/main/instruction%20old.md).

tbh this is all over the place so you should just use this as a guide for what parts goes where (I have no idea what im doing)

1. Cut a piece of aluminum tape and stick it on the build plate
2. Use aluminum tape to cover the inside light tunnel to help the light disperse better
   ![Both build plate and light tunnel](https://github.com/shervain123/kittenmaker/blob/main/images/light%20tunnel%20and%20build%20plate.jpg)
3. Screw the bottom to the bottom case using 3 M3 screw and nuts
4. Solder wires to the sdcard board and screw it into the bottom case using 2 M2 screw and nuts
   ![SD screw in](https://github.com/shervain123/kittenmaker/blob/main/images/new%20sd.jpg)
5. Screw the wemos s2 mini with the spacer
   ![wemos screw in](https://github.com/shervain123/kittenmaker/blob/main/images/new%20s2.jpg)
6. Next screw in your fan and pass the wire through the hole
7. Remove the lcd from the frame, the metal backing can be removed using a flat head screwdriver then gently bend the plastic part backwards to loosen the glue and slow the display will pop out
8. make sure you remove all the backlight component from the display and you should be left with a lcd that is see through dimly
   ![Naked display](https://github.com/shervain123/kittenmaker/blob/main/images/seperated%20display.jpg)
9. pass all the wires and ribbon into the hold on the top case and place the display in it's place DO NOT FORCE IT IN IF IT DOESN'T FIT take it out and cut the edges of the top half NOT THE DISPLAY
10. Screw in the motor and the micro switch as well (use m2x10 for the switch)
11. Your finished top half should look something like this
    ![Top half](https://github.com/shervain123/kittenmaker/blob/main/images/1710408309012.jpg)
12. Then finished the bottom half by soldering the leds, motor controller and fan
13. Then you should solder both the lcd and sd card wires (based on the wiring diagram
14. After checking your connection plug it in  and test is everything worked
15. Screw the board to the bottom case and glue the sd card to the back
    ![inside](https://github.com/shervain123/kittenmaker/blob/main/images/inside.jpg)
16. Then screw in the top case with m2x4 screw
    ![completed bottom part](https://github.com/shervain123/kittenmaker/blob/main/images/screws.jpg)
17. Glue the feet to the bottom of the case and put coupler onto the motor
18. add glue to your bic pen and shove it in the hexagon shaped hole on the bottom and insert your lead screw into the coupler
    ![pencile](https://github.com/shervain123/kittenmaker/blob/main/images/bottom%20completed%20half.jpg)
19. Take the top part and insert your lead screw nut you will need to drill the hole for it
    ![top part](https://github.com/shervain123/kittenmaker/blob/main/images/lead%20screw%20thing.jpg)
20. Put the 6 bearing in place and use M3 screw to secure it in place (I run out of shorter screw)
    ![now with bearings!](https://github.com/shervain123/kittenmaker/blob/main/images/with%20bearings.jpg)
21. Place 4 M3 nut in place and find the longest M3 screw you have to screw it in
    ![now with nuts!](https://github.com/shervain123/kittenmaker/blob/main/images/carrage%20with%20screw%20and%20nuts.jpg)
22. Screw the plastic peg into the screw
    ![Pegs](https://github.com/shervain123/kittenmaker/blob/main/images/carrage%20with%20plastic%20thingy.jpg)
23. add the longest m2 screw you have to the small part at the bearing side (this function as a home switch adjuster thingy)
24. place the magnet in all the places needs it (vat,case top, build plate and the just fron just now)
25. stick the FEP film on the vat
26. i think that's about it
27. idk still waiting for my magnets
