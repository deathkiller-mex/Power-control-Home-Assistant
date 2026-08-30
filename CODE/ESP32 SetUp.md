Step 1: Flashing the ESP32
   * Plug the ESP32 into your computer using a data-capable Micro-USB cable.

   * Go to web.esphome.io.

   * Click Connect and select the USB serial port (usually labeled CP2102 or CH340).

   * Click Prepare for first use. It will ask for your Wi-Fi network name and password. This embeds your Wi-Fi credentials straight into the chip so it can join your local network.

Step 2: The Custom YAML Configuration
   * Once the ESP32 is on your Wi-Fi, you will manage it via the ESPHome dashboard.
   * This is the code following the schematic. IF FOR SOME REASON U WIRED IT DIFFERENTLY, REMEMBER TO CHANGE THE CODE TOO, OR IT WILL NOT WORK PROPERLY.
CODE: go to the YAML file in this same folder (I did not add it here to keep everything clean, and if I added it, the format messed everything up.)


Step 3: Pushing the Code Over Wi-Fi (OTA)
   * After pasting this into the ESPHome dashboard, click Install and select Wirelessly. ESPHome will compile the YAML code into C++, build the firmware, and beam it over your Wi-Fi network directly into the ESP32. (You never have to plug it into your computer via USB again; all future updates are wireless).

Step 4: Home Assistant Auto-Discovery
   * Once the wireless flash reaches 100%, open your Home Assistant dashboard.

   * Navigate to Settings > Devices & Services.

   * You will see a banner at the top saying "Discovered: Workbench Power (ESPHome)".

   * Click Configure and hit Submit.
