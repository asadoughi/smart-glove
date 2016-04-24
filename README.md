# Smart glove

Open hardware wearable glove

![alt First prototype](https://github.com/asadoughi/smart-glove/raw/master/first_prototype.jpg)

# Parts

1. [Golf glove](http://amzn.to/1T7mhV9)
2. Hot glue, hot glue gun
3. Electric tape
4. Solder, soldering gun
5. [Adafruit Flora](https://www.adafruit.com/products/659)
6. Five (5) [Adafruit Flora 9 DOF sensors](https://www.adafruit.com/products/2020)
7. [Adafruit I2C multiplexer](https://www.adafruit.com/products/2717)
8. USB cable
9. [Adafruit Perma-proto quarter-sized (or half-sized) breadboard](https://www.adafruit.com/products/1608)
10. [Adafruit Premium male/male jumper wires](https://www.adafruit.com/products/758)
11. [Hookup wire](http://amzn.to/1raxAVS)

# Instructions

Use a multimeter to test your solder joints along the way. There is a lot of soldering to do.

1. Mount the I2C mux to the breadboard.
2. Mount the Flora to the breadboard. In the first prototype I have it floating above the mux via hookup wire.
3. Wire the Flora to the I2C mux: VIN, GND, SDA, SCL.
4. Wire the I2C mux to each of the Flora 9 DOF sensors (VIN, GND, SDA, SCL) with the male/male jumper wire.
5. Mount the sensors to the golf glove with electric tape and/or hot glue.
6. Mount the breadboard to the golf glove. I chose to mount it onto the velcro tab.

Overall time: 7 - 8 hours. (Maybe much less if you have soldering experience.)

# Future plans

1. Mobility. Currently the wearable glove requires being tethered to a computer via USB. It would be nice to have a battery and Bluetooth communications. The first attempt at adding Bluetooth failed because of Bluetooth transfer speeds required modifying firmware.
2. Sensor fusion. Being able to reliably take all the sensor input data and produce a single view of the hand has proved difficult. Many sensor fusion algorithms are proprietary and the publicly available ones will have to be heavily modified to build a model of a hand and fingers.
3. Applications. Once we have a sensor fusion layer, we can build applications on top of that platform, such as a keyboard.
