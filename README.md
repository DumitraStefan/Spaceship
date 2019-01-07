# Spaceship

Main idea:
  This is a classic arcade game. The main thing you have to do is to survive for as long as possible, destroying the meteors with rockets  before they touch the spaceship.

Implementation:
  The game will start with the message: "START NEW GAME" and will be displayed until one of the buttons is pushed. The code:
  - checks if you can move, or fire
  - creates meteors on a random position
  - clears the led matrix
  - draws the spaceship, meteors and rockets
  - checks if the meteor touched the spaceship - the function that ends and resets the game - or the spaceship went into a meteor
  
Demo Video: https://photos.app.goo.gl/NUAnD6Geg3Hok1xL6
  
Requirements:
 - library <LedControl.h>
 
 Components you will need:
 - breadboard
 - arduino UNO
 - 8x8 LED matrix 
 - driver MAX7219
 - 4 Buttons
 - four 470 Ohm resistors (buttons)
 - one 10 kOhm resistor (driver ISet pin)
 
Connections:
For the connections between led matrix and driver:
  check if youre led matrix is column cathode on column anode; either way, DIG0 TO DIG7 should be connected to cathodes and SEG0 to SEG7   to anodes (fore more info: http://wayoda.github.io/LedControl/pages/hardware)
  
  

Four buttons are connected to the Analog Input PINs from A0 to A3.
- A0 - Connects to the button that shoots from the right side of the spaceship
- A1 - Connects to the button that shoots from the left side of the spaceship
- A2 - Connects to the button that moves spaceship to the left
- A3 - Connects to the button that moves spaceship to the right
Three wires are connected to PINs 10, 11 and 12.
- PIN 12 - DATA IN-pin
- PIN 11 - CLK-pin
- PIN 10 - LOAD(/CS)-pin
