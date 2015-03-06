Known issues:

When we compile get the error: 'ArduinoDmxN' was not Declared In This scope:

Check if you have configured the correct type of board in the Arduino IDE, menu tools > board
(with Arduino nano can only use one USART = ArduinoDmx0 = USART0)


Flicker when controlling LEDs:

If we are dealing with LED lights, flicker may appear due to a refresh rate too low, we use fewer channels per universe (eg 200 instead of 512, to increase the frequency) and / or use less universes.

Note about the refresh time:

The Arduino Mega & Nano use an Atmel AVR 8-bit microcontroller running at 16 Mhz which have limited resources.

Forked from - www.deskontrol.net (Toni Merino)