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

# Instructions

// todo

# Future plans

1. Mobility. Currently the wearable glove requires being tethered to a computer via USB. It would be nice to have a battery and Bluetooth communications. Our first attempt at adding Bluetooth failed because of Bluetooth transfer speeds required modifying firmware.
2. Sensor fusion. Being able to reliably take all the sensor input data and produce a single view of the hand has proved difficult. Many sensor fusion algorithms are proprietary and the publicly available ones will have to be heavily modified to build a model of a hand and fingers.
3. Applications. Once we have a sensor fusion layer, we can build applications on top of that platform, such as a keyboard.
