# ESPHome Avatto Wi-Fi Thermostat

<img src="https://github.com/user-attachments/assets/63bfc073-f346-4c63-9e43-525a7d93bdd8" alt="Thermostat image" width="500" />

## Description

<img src="https://github.com/user-attachments/assets/368a2296-467e-4e3b-9bb2-4ee4fa601caf" alt="Home Assistant device page" width="600" />

This repository contains the ESPHome configuration for the **Avatto Tuya Wi-Fi Thermostat**, enabling seamless integration with Home Assistant and other smart home systems. By leveraging ESPHome, you can customize and enhance the functionality of your thermostat, providing greater control and automation capabilities.

**Product Link:** [AliExpress - Avatto Tuya Wi-Fi Thermostat](https://www.aliexpress.com/item/1005006902833391.html)  

`Product: '{"p":"m3j5wouhgsvjlma9","v":"1.0.0","m":0}'`

# Hardware

### Original hardware

- **Module:** WBR3 (RTL8710)
- **Compatibility:** Not compatible with ESPHome or OpenBeken

<img src="https://github.com/user-attachments/assets/422707e3-9005-48b2-b6bb-3b2d0e7d082b" alt="WBR3 photo" width="150"/>  

### Replacement Hardware

- **Module:** ESP-C3-12F
- **Product Link:** [AliExpress](https://www.aliexpress.com/item/1005004475310734.html)

<details>
   <summary>esptool flash_id output</summary>
   
   ```
   Chip is ESP32-C3 (QFN32) (revision v0.3)
   Features: WiFi, BLE, Embedded Flash 4MB (XMC)
   Crystal is 40MHz
   MAC: 84:f7:03:b6:b2:70
   Uploading stub...
   Running stub...
   Stub running...
   Manufacturer: 20
   Device: 4016
   Detected flash size: 4MB
   ```
   
</details>
   
<img src="https://github.com/user-attachments/assets/e24fc948-8d01-45a8-96fb-244b848b8731" alt="Replaced ESP-C3-12F" width="500" />

### Flashing Guide

> **📝 NOTE**  
> To enter flashing mode, **GPIO8** needs to be pulled high (to VCC) and **GPIO9** pulled low.  
> **Pre-flash** the module before soldering it to the board.

Follow the [Flashing Guide](https://github.com/espressif/esp-idf/issues/9005#issuecomment-1878941288) to correctly flash the ESP-C3-12F module.

## Documentation

- **ESP-C3-12F Datasheet:** [`docs/esp-c3-12f_specification.pdf`](docs/esp-c3-12f_specification.pdf)
- **Datapoints Description:** The [`docs/datapoints.md`](docs/datapoints.md) file contains descriptions of all known datapoints used by the device.

## License

This project is licensed under the [MIT License](LICENSE).
