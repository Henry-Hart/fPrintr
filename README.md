# fPrintr
A nice fingerprint gui
## Overview
This uses an (any) arduino and a liquid crystal display screen to add fingerprints to an inbuilt database which can be analysed or moved afterwards
## Requirements
### Software
* Arduino IDE (use this for compiling and uploading) https://www.arduino.cc/en/software
### Tech
* 128x64 SPI OLED Display https://www.amazon.co.uk/128x64-Display-Module-U8glib-Arduino/dp/B077K3V128
* Basically any arduino https://store.arduino.cc
* Adafruit fingerprint sensor https://www.amazon.co.uk/Fingerprint-Scanner-Optical-Arduino-Mega2560/dp/B07H56V1VN
### Libraries
* Adafruit fingerprint sensor library https://www.arduino.cc/reference/en/libraries/adafruit-fingerprint-sensor-library
* U8glib https://www.arduino.cc/reference/en/libraries/u8glib
* (SoftwareSerial <-- Comes with Arduino IDE, but the reference is here https://www.arduino.cc/en/Reference/SoftwareSerial)
## Explanation
* Scans a fingerprint twice, validates it and stores it
* Uses the liquid crystal display (lcd) screen to display text and some lovely images showing what to do next
* Also has a serial monitor output
## Additional details
* If you are using an arduino Leonardo/Micro, you don't need SoftwareSerial; uncomment `#define hardwareSerial`
* If you want to access the fingerprints, use the examples in the Adafruit fingerprint sensor library
* If you want to change the images, use LCDAssistant* http://en.radzio.dxp.pl/bitmap_converter
* *The website isn't secure, but I have checked my version for malware. The sha512sum is 
```
e7f1e988f6af2135a180146542d2b7b718554887ad1f94fcb827be1b929fad6ef85b8003e99837e0ea375f2435b24b4e658d09cd1d0d7cff4c371f11baf52333
```
## Disclaimer
* I made this ages ago so I will probably update it quite a lot
* Some of the links I have given might stop working
* There will definitely be cheaper components out there, so don't necessarily buy the first one you see
