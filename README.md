# Power control: Home Assistant
So after setting up HA and tinkering with it, I got the idea from, of course, JARVIS from Iron Man, where different appliances can be controlled by JARVIS, or in this case, HA. All the materials needed will be listed down below and u may change the amount of ports and sockets depending on ur needs BUT AT LEAST AS OF NOW, ANY CHANGES WOULD MAKE THE 3D FILES FOR THE BODY USELESS SINCE IT WAS DESIGNED FOR A CERTAIN AMOUNT OF PORTS AND SOCKETS (IT MAY STILL WORK IF U DECREASE THE AMOUNT INSTEAD OF INCREASING IT BUT IT WILL RESULT ON WHOLES ON THE BODY. With that in mind, while designing the body, I got the idea of why not also add DATA ports to connect to either ur HA or any other computer that may need more ports, so I decided to add a port hub as well as 4 individual 5V and 12V ports for actual power control.


QUICK IMPORTANT NOTICE: THE ACTUAL GUIDE ON HOW TO SET UP HA WILL NOT BE INCLUDED IN THIS GITHUB PAGE. I WILL ONLY GUIDE U THROUGH THE DESIGN I MADE AS WELL AS SETTING  UP THE ESP32 TO CONTROL THE POWER CONTROLLER.

----------------------------------
# THE PROJECT IS NOT DONE YET. UNFORTUNATELY, THE PARTS HAVE NO FULL DIMENSIONS PUBLISHED, SO I HAD TO APPROXIMATE MOST OF THE DIMENSIONS, MEANING THAT THE CURRENT CAD MODELS ARE OFF AND WILL NOT FIT. AS SOON AS I GET THE MODELS, I WILL UPDATE EVERY MODEL, ADD MORE DETAIL, AND ENSURE THEY ACTUALLY FIT. PLS DO NOT ATTEMPT TO PRINT AS IS; SCHEMATIC, CODE, AND PARTS SHOULD WORK BUT HAVE NOT BEEN TESTED!! USE AT UR ON RISK. THANKS FOR THE UNDERSTANDING AND I APOLOGIZE FOR ANY INCONVENIENCE.
----------------------------------

# Full Assembly
<img width="562" height="315" alt="enclosure with comp" src="https://github.com/user-attachments/assets/9585e631-0b5a-4456-b01a-d8da501eb4d6" />
<img width="548" height="317" alt="enclosure with lid" src="https://github.com/user-attachments/assets/d3ab3297-15f9-4c5a-95a1-e7994aa9b9c4" />

# Inserts Map
To assemble everything, take the inserts that fit in each hole and, using ur woldering iron, press them till they are at the same level as the material surrounding them. 

Insert brass inserts map: ** Ignore this; once I have the actual measurements and have updated the model to a final one, I will create a map showing which exact holes use which insert.**

# Component map

<img width="880" height="577" alt="image" src="https://github.com/user-attachments/assets/701d07ad-68c2-43b6-b500-bad64cdf9564" />
**Future note: update image with labeled parts once detailed and closer to reality models have been made**

# Schematic
<img width="663" height="407" alt="shematic" src="https://github.com/user-attachments/assets/44d2183a-5f65-4367-a244-d735f0b4f708" />

# PCB
This PCB is fully optional, and u can use it for cable management, if ur ok with messy cables, ignore it; if u want something clean, make the PCB (all Gerber files are under the PCB folder)
<img width="221" height="268" alt="PCB screenshot" src="https://github.com/user-attachments/assets/3ffff288-5c76-4155-b24f-d4b91c9488a9" />


# BOM
|Part|Amount|Price|Link|
|:------------:|:----:|:---:|:--:|
|Buck Power Converter Step Down Voltage Regulator 12V-5V 20A|1|$26.19|[Aliexpress](https://www.aliexpress.us/item/3256806445858334.html?spm=a2g0o.cart.0.0.742038dazTbZ1p&mp=1&pdp_npi=6%40dis%21USD%21USD+26.19%21USD+26.19%21%21USD+26.19%21%21%21%402101ca8b17881203541565017e0e76%2112000037877472884%21ct%21US%216359134517%21%211%210%21&gatewayAdapt=glo2usa)|
|USB Female port|4|$2.91|[Aliexpress](https://www.aliexpress.us/item/2255800984460804.html?spm=a2g0o.cart.0.0.742038dazTbZ1p&mp=1&pdp_npi=6%40dis%21USD%21USD+2.91%21USD+2.91%21%21USD+2.91%21%21%21%402101ca8b17881203541565017e0e76%2112000052246244306%21ct%21US%216359134517%21%211%210%21&gatewayAdapt=glo2usa)|
|Female Wall Socket|4|$3.09|[Aliexpress](https://www.aliexpress.us/item/2255799950902957.html?spm=a2g0o.cart.0.0.742038dazTbZ1p&mp=1&pdp_npi=6%40dis%21USD%21USD+3.09%21USD+3.09%21%21USD+3.09%21%21%21%402101ca8b17881203541565017e0e76%2110000000412254835%21ct%21US%216359134517%21%212%210%21&gatewayAdapt=glo2usa)|
|Power Supply 12V 120W|1|$11.08|[Aliexpress](https://www.aliexpress.us/item/3256807161025414.html?spm=a2g0o.cart.0.0.742038dazTbZ1p&mp=1&pdp_npi=6%40dis%21USD%21USD+11.08%21USD+11.08%21%21USD+10.97%21%21%21%402101ca8b17881203541565017e0e76%2112000040387111145%21ct%21US%216359134517%21%212%210%21&gatewayAdapt=glo2usa)|
|MOSFET Relay LR7843-30V 161A|4|$7.71|[Aliexpress](https://www.aliexpress.us/item/3256805438795816.html?spm=a2g0o.cart.0.0.742038dazTbZ1p&mp=1&pdp_npi=6%40dis%21USD%21USD+7.71%21USD+7.71%21%21USD+7.71%21%21%21%402101ca8b17881206844632683e0e76%2112000052735209265%21ct%21US%216359134517%21%213%210%21&gatewayAdapt=glo2usa)|
|8-channel Relay with optocoupler|1|$5.87|[Aliexpress](https://www.aliexpress.us/item/3256811743748492.html?spm=a2g0o.cart.0.0.742038dazTbZ1p&mp=1&pdp_npi=6%40dis%21USD%21USD+11.75%21USD+5.87%21%21USD+5.81%21%21%21%402101ca8b17881206844632683e0e76%2112000057053925896%21ct%21US%216359134517%21%211%210%21&gatewayAdapt=glo2usa)|
|ESP-32|1|$4.72|[Aliexpress](https://www.aliexpress.us/item/3256808317516268.html?spm=a2g0o.cart.0.0.742038dazTbZ1p&mp=1&pdp_npi=6%40dis%21USD%21USD+4.72%21USD+4.72%21%21USD+4.72%21%21%21%402101ca8b17881206844632683e0e76%2112000045457574256%21ct%21US%216359134517%21%211%210%21&gatewayAdapt=glo2usa)|
|FE2.1 Based USB 2.0 7 Port Hub Splitter|1|$7.4+$5.52|[Aliexpress](https://www.aliexpress.us/item/3256809182802772.html?spm=a2g0o.cart.0.0.742038dazTbZ1p&mp=1&pdp_npi=6%40dis%21USD%21USD+9.25%21USD+7.40%21%21USD+7.40%21%21%21%402101ca8b17881208414901970e0e76%2112000048890257449%21ct%21US%216359134517%21%211%210%21&pdp_ext_f=%7B%22cart2PdpParams%22%3A%7B%22pdpBusinessMode%22%3A%22retail%22%7D%7D&gatewayAdapt=glo2usa)|
|Aprox. Total| |$107.74| |



# What for??
Buck Power Converter Step Down Voltage Regulator 12V-5V 20A: steps down 12V to 5V, safe for most appliances and USB hub.
USB Female port: Connect DC appliances (12V and 5V).
Female Wall Socket: Connect AC appliances.
Power Supply 12V 120W: Supplies DC to the USB ports and USB hub.
MOSFET Relay LR7843-30V 161A: Controls power (on/off) for DC appliances (12V and 5V).
8-channel Relay with optocoupler:  Controls power (on/off) for AC appliances.
ESP-32: Brain to control the relays and connect to HA.
FE2.1 Based USB 2.0 7 Port Hub Splitter: Enables the computer to communicate with other devices digitally through the USB ports rather than turning things on or off.
