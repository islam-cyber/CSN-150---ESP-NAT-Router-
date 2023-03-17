# CSN-150---ESP-NAT-Router-

Purpose
To Create a functioning WIFI PENETRATION TOOL!
Equipment that i used - Win 11 , ESP32 Device  -ESP32 Flash Download Tool V 3.9.3
Steps That I Followed

First we need to download flash and tools .
https://github.com/martin-ger/esp32_nat_router this for NAT router 
https://www.espressif.com/en/support/download/other-tools Flash tool , version 3.9.4 or 3.5 whterver 
After downloaded , exctract all of theme , then we need to open the tool , press on Developer mode then after that chosse ESP32 DownloadTool .  Undter SPIDownload , open the first tab to browse the file for nat router , first one need to select bootloader.bin . sp32_nat_router-master\build\esp32\bootloader.bin , then select second one firmware .  firmware.binesp32_nat_router-master\esp32_nat_router-master\build\esp32 . last one partitions.bin . then go to first one bootloadter and put 0x1000 , second one 0x10000 , last one (partitions.bin) 0x8000 . Now need to select for three items then connect the Device ESP32 . 
![Screenshot 2023-03-15 213102](https://user-images.githubusercontent.com/123830641/226068686-f262db39-f3ba-482f-9ff7-d5c4f0d1323f.png)

First Boot
After first boot the ESP32 NAT Router will offer a WiFi network with an open AP and the ssid "ESP32_NAT_Router". Configuration can either be done via a simple web interface or via the serial console.

![Screenshot 2023-03-15 213102](https://user-images.githubusercontent.com/123830641/226067544-718b6fc9-bcd2-4c97-8e8d-701e8ac7b567.png

The web interface allows for the configuration of all parameters. Connect you PC or smartphone to the WiFi SSID "ESP32_NAT_Router" and point your browser to "http://192.168.4.1". This page should appear: ![ESP32_NAT_UI3](https://user-images.githubusercontent.com/123830641/226068463-118757f7-adbf-46a9-9824-c6a3bd757ac5.png)


open the broswer and type 192.168.4.1 press enter , and type cred SSID and password to trying extend your network . you will see if you go over network icone it will seeing is disconnected , try to connect again with password that you put before on router interface . Now go to browser and test your network 

