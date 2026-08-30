# Power control: Home Assistant
So after setting up HA and tinkering with it, I got the idea from, of course, JARVIS from Iron Man, where different appliances can be controlled by JARVIS, or in this case, HA. All the materials needed will be listed down below and u may change the amount of ports and sockets depending on ur needs BUT AT LEAST AS OF NOW, ANY CHANGES WOULD MAKE THE 3D FILES FOR THE BODY USELESS SINCE IT WAS DESIGNED FOR A CERTAIN AMOUNT OF PORTS AND SOCKETS (IT MAY STILL WORK IF U DECREASE THE AMOUNT INSTEAD OF INCREASING IT BUT IT WILL RESULT ON WHOLES ON THE BODY. With that in mind, while designing the body, I got the idea of why not also add DATA ports to connect to either ur HA or any other computer that may need more ports, so I decided to add a port hub as well as 4 individual 5V and 12V ports for actual power control.


QUICK IMPORTANT NOTICE: THE ACTUAL GUIDE ON HOW TO SET UP HA WILL NOT BE INCLUDED IN THIS GITHUB PAGE. I WILL ONLY GUIDE U THROUGH THE DESIGN I MADE AS WELL AS SETTING  UP THE ESP32 TO CONTROL THE POWER CONTROLLER.

# Full Assembly
<img width="562" height="315" alt="enclosure with comp" src="https://github.com/user-attachments/assets/9585e631-0b5a-4456-b01a-d8da501eb4d6" />
<img width="548" height="317" alt="enclosure with lid" src="https://github.com/user-attachments/assets/d3ab3297-15f9-4c5a-95a1-e7994aa9b9c4" />


# Schematic
<img width="663" height="407" alt="shematic" src="https://github.com/user-attachments/assets/44d2183a-5f65-4367-a244-d735f0b4f708" />


# BOM
|Part|Amount|Price|Link|
|:------------:|:----:|:---:|:--:|
|Buck Power Converter Step Down Voltage Regulator 12V-5V 20A|1|$26.19|[Aliexpress](https://www.aliexpress.us/item/3256806445858334.html?spm=a2g0o.cart.0.0.742038dazTbZ1p&mp=1&pdp_npi=6%40dis%21USD%21USD+26.19%21USD+26.19%21%21USD+26.19%21%21%21%402101ca8b17881203541565017e0e76%2112000037877472884%21ct%21US%216359134517%21%211%210%21&gatewayAdapt=glo2usa)|
|USB Female port|4|$2.91|[Aliexpress](https://www.aliexpress.us/item/2255800984460804.html?spm=a2g0o.cart.0.0.742038dazTbZ1p&mp=1&pdp_npi=6%40dis%21USD%21USD+2.91%21USD+2.91%21%21USD+2.91%21%21%21%402101ca8b17881203541565017e0e76%2112000052246244306%21ct%21US%216359134517%21%211%210%21&gatewayAdapt=glo2usa)|
|Female Wall Socket|4|$3.09|Aliexpress|
|Power Supply 12V 120W|1|$11.08|Aliexpress|
|MOSFET Relay LR7843-30V 161A|4|$7.71|Aliexpress|
|8-channel Relay with optocoupler|1|$5.87|Aliexpress|
|ESP-32|1|$4.72|Aliexpress|
|FE2.1 Based USB 2.0 7 Port Hub Splitter|1|$7.4+$5.52|Aliexpress|
|Aprox. Total| |$107.74| |



Approximate Total, , ,$107.74


# What for??
