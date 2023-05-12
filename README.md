# mega2560-wifi
Set up a Mega 2560 with built in ESP wifi and get working within the Arduino IDE

Code examples to come.

I recently purchase some Mega2560 with Wifi Boards from AliExpress, I wasn't after wifi on them but they were only a couple of dollars more so I figured why not!.

Upon trying I ran in to some hurdles and found the firmware version on the ESP8266 is older and doesn't support the WIFI_ESP library in Arduino.  It took a while to figure everything out as I couldn't find any tutorials start to finish on these boards, I found the required information spread across multiple sites and after a bit of trial and error got everything working.

## Notes:

### Dip Switch Settings

![image](https://github.com/The-Tinkerers-Chronicle/mega2560-wifi/assets/133438787/c7429c1f-ea2c-4ea5-9095-878ea236074d)

(source: https://www.aliexpress.com/item/32806021806.html?af=954319)

### ESP init data Memory Addresses

**The ESP8266 that was on my boards 512kb version, I assumme they are all the same.**
![image](https://github.com/The-Tinkerers-Chronicle/mega2560-wifi/assets/133438787/563bbf2d-2444-403d-92b1-c73616a877fc)

(source: https://arduino.stackexchange.com/questions/33590/endless-loop-on-boot-after-reflashing-esp-12e-with-at-firmware)

## Firmware Update

### The tool for firmware update
To update the firmware you must download the special tool application and the firmware itself. Application for firmware update ESP8266 will use Flash Download Tools v2.4 from official site Espressif Systems. Link to the download page: http://espressif.com/en/products/hardware/esp8266ex/resources. You must go to "Tools" section.

### Firmware
The firmware can also be downloaded from the official site. A link to the download page on the official website: http://espressif.com/en/products/hardware/esp8266ex/resources. You must go to “SDKs & Demos” section and download firmware ESP8266 NONOS SDK version at least v1.3.0. This firmware version began to support AT commands v0.40.

All downloaded files must be unpacked and placed in the directory where the full path to the file contains only Latin characters, ie characters without the language localization.

![image](https://github.com/The-Tinkerers-Chronicle/mega2560-wifi/assets/133438787/593d8712-868e-42f0-a301-dd4b87f3a345)

(source: https://remotexy.com/en/help/esp8266-firmware-update/)
