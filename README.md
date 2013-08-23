SmartTemp
=========

Tmp36/ATtiny85

Sources:

1)  Uber fridge:
    The filtering code is directly from this project and works great
    
        http://www.elcojacobs.com/eleminating-noise-from-sensor-readings-on-arduino-with-digital-filtering

2)  Attiny85 Programing with Arduino 

        http://hlt.media.mit.edu/?p=1695
     
3) Sensor Calibration:

      V_calib = V_base * ((T_ref + 50) / (T_base + 50))
      V_base = 1100
      T_ref = temperature as measured by reliable source
      T_base = temperature as measured on ATtiny85
      http://mchr3k-arduino.blogspot.com/2012/02/wireless-sensor-node-part-9.html
      
   Very important becasue the ATtiny85 internal reference is not consistent across chips 
   
 
   
4) TinyWire I2C for the ATtiny85/84:

    http://playground.arduino.cc/Code/USIi2c


This code is for an ATtiny85. The ATtiny85 reads sensor data from am TMP36 then filters and sends the data back to an Arduino UNO using I2C. These slaves will placed througout my house using unused ethernet ports to connect to the I2C  lines. 

I will eventually display the temps on 7 segment displays in a central location. I will also be controlling a blower fan to boost my air flow from my HVAC system to upstairs.  
