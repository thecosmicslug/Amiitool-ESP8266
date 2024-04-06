# Amiitool-ESP8266 - Amiibo Manipulation using ESP8266
Based on Wifiibo, But with all the web configuration and wifi taken out because I wanted something portable.
I was worried that the Wifiibo project might disappear one day, so ive uploaded my own backup.

The original can be found [https://github.com/Xerxes3rd/Wifiibo](https://github.com/Xerxes3rd/Wifiibo) for reference.

Using an ESP8266 (with the Arduino development environment) and an NFC reader, you can read & store existing amiibos, create new amiibos using amiibo data files, and view your amiibo data. 

The library that runs most of the amiibo functions is a port of [amiitool](https://github.com/socram8888/amiitool) for the ESP8266 using the Arduino environment.

## Features
* Save/back up existing amiibo
* Create blank amiibos without any existing dumps (requires encryption keys)
* Create new ammibos using data files (requires encryption keys)


## Getting Started
### Hardware
Wifiibo requires the following hardware:
* ESP8266
* PN532 NFC board 


Remember to flip the DIP switches on the PN532 board to SPI mode (ch1: OFF, ch2: ON).


Wifiibo also uses modified versions of the following libraries; they are included with Wifiibo, so you don't need to download them separately (they also use different library names so they will coexist with existing copies):
* [Adafruit_PN532](https://github.com/adafruit/Adafruit-PN532)
* [mbedtls](https://tls.mbed.org/)
 
## References & Credits
Wifiibo mostly uses software & libraries written by others.  The following resources were used to develop Wifiibo:
* [Kostia Plays](https://games.kel.mn/en/create-amiibo-clones-with-arduino/) - Tons of info on how to read & write amiibos by @konstantin-kelemen
* [amiitool](https://github.com/socram8888/amiitool) - Software to encrypt/decrypt amiibo data by @socram8888
* [GBATemp](http://wiki.gbatemp.net/wiki/Amiibo) - amiibo data structure information
* [3dBrew](https://www.3dbrew.org/wiki/Amiibo) - amiibo/NTAG215 data structure information
* [amiibo API](https://github.com/N3evin/AmiiboAPI/) - Online amiibo database & index by @N3vin

