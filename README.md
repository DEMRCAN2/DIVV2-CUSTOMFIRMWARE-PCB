# DIVV2-CUSTOMFIRMWARE-PCB
This repository contains the custom PCB design files and modified firmware for the DIY V2 project. The original codebase and hardware layout have been customized to improve performance, add new features, and fit a custom form factor.


Key Modifications
Hardware (Custom PCB)

  Redesigned Layout: Optimized trace routing and component placement for better stability and a smaller footprint.
  Custom Pinout: Remapped I/O pins to match the new board architecture.


Software (Modified Firmware)

  Custom Pin Definitions: Updated firmware pin mappings to fully support the custom PCB.
  Feature Enhancements: Removed GPS and annoying PCF8574 module for easy wiring buttons
  And added some suprise features to wifi deauther, ble spammer, wifi handshake capture, subghz stuff if yall look yall will see
  Bug Fixes & Optimization: Cleaned up unused code and optimized memory usage.
## ⚠️ Disclaimer

This project, including all hardware designs (PCB) and firmware, is provided strictly for **educational, research, and authorized security testing purposes only**. 

* **Legal Compliance:** Users are solely responsible for ensuring that their use of this hardware and software complies with all applicable local, national, and international laws and regulations regarding radio frequency (RF) transmissions and wireless communications.
* **No Liability:** The author and contributors assume no liability and are not responsible for any misuse, damage, or legal consequences resulting from the use or modification of the files provided in this repository.
* **Authorized Use Only:** Do not use this project to interfere with, disrupt, or access networks, devices, or frequencies without explicit permission from the rightful owner.












## ⚙️ Firmware Build Environment

* **Arduino IDE:** `v2.x`
* **ESP32 Board Package:** `2.0.10` or `2.0.11` (*Espressif Systems* — replace `platform.txt` using the modified file from [cifertech/ESP32-DIV](https://github.com))
* **Board:** `ESP32S3 Dev Module`
* **Flash Size:** `16MB (128Mb)`
* **Partition Scheme:** `Minimal SPIFFS (1.9MB APP with OTA/190KB SPIFFS)`
* **PSRAM:** `OPI PSRAM`
* **Upload Speed:** `921600`

---

## 📚 Required Libraries

| Library | Version |
| :--- | :--- |
| **TFT_eSPI** *(Custom)* | `v2.5.x` |
| **XPT2046_Touchscreen** | `v1.4` |
| **RF24** *(Custom)* | `v1.4.x` |
| **ELECHOUSE_CC1101_SRC_DRV** *(Custom)* | `v2.5.x` |
| **rc-switch** | `v2.6.4` |
| **IRremoteESP8266** | `v2.8.x` |
| **Adafruit PN532** | `v1.3.x` |
| **Adafruit NeoPixel** | `v1.12.x` |
| **ArduinoJson** | `v6.21.x` / `v7.x` |
| **SD / SPI / FS / WiFi / BLE** | *Built-in (ESP32 Core 2.0.10)* |
