This project was designed to control a HVAC blower fan to blow cool air from my basement up to my bedroom during the warm summer month. I use four TMP36 temperature sensors each controlled by an Attiny85. The Attiny85 filters the analog data and then communicates back to an Arduino Uno via i2c. I also use an Attiny85 to control a relay that controls the blower fan this allows it to communicate over i2c. I use an Adafruit 16x2 LCD shield with buttons to display the temperatures and adjust menu settings. The LCD and buttons are controlled via i2c. This means the whole system only uses two wires for communication.  The Arduino Uno acts as the i2c master parsing the incoming data and changing the necessary variables. 

This is a video of the project in action: http://youtu.be/glCS1Rm0Yho

Works Cited

1. Mchr3k. Mchr3k - Arduino. [Online] July 2013.                                                                             http://mchr3k-arduino.blogspot.com/2012/02/wireless-sensor-node-part-9.html.

2. Media, M.I.T. High-Low Tech. [Online] http://hlt.media.mit.edu/?p=1695.

3. BroHogan. Arduino Playground. I2C (master and slave) on the ATtiny85. [Online] July 2013.                                 http://playground.arduino.cc/Code/USIi2c.

4. Jacobs, Elco. Eleminating noise from sensor readings on Arduino with digital filtering. [Online] July 2013.               http://www.elcojacobs.com/eleminating-noise-from-sensor-readings-on-arduino-with-digital-filtering.

5. Adafruit Industries . Adafruit Learning System. RGB LCD Shield. [Online] July 2013.                                       http://learn.adafruit.com/rgb-lcd-shield.

6. Margolis, Michael. Arduino Cookbook 2nd Edition. [ed.] Teresa Elsey. Sebastopol : O'reilly, 2012. 978-1-44931387-6.

