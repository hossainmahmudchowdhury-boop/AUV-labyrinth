# AUV-labyrinth

#### Outlook

![image alt](https://github.com/hossainmahmudchowdhury-boop/AUV-labyrinth/blob/main/Images/Screenshot%202026-10-01%20182908.png)

This project is about an underwater submarine that can follow a route to survey the aquatic environment. It can detect the number of fish in an area and observe aquatic biology. In this project, it emphasizes an ML-based detection system and a water quality checker.
![image alt](https://github.com/hossainmahmudchowdhury-boop/AUV-labyrinth/blob/main/Images/Screenshot%202026-10-05%20205444.png)

### PCB 


![image alt](https://github.com/hossainmahmudchowdhury-boop/AUV-labyrinth/blob/main/Images/Screenshot%202026-10-26%20192654.png)
![image alt](https://github.com/hossainmahmudchowdhury-boop/AUV-labyrinth/blob/main/Images/Screenshot%202026-10-26%20192739.png)

## Bill of Materials (BOM)

The following table lists the estimated components and costs for the underwater surveillance submarine prototype. The system combines onboard image processing, sensor data collection, underwater imaging, and remote communication.

### 1. Mechanical and PCB Fabrication

| Category | Component | Description | Estimated Cost (USD) |
|---|---|---|---:|
| Mechanical | Waterproof 3D Printing | Custom submarine body | $125.00 |
| PCB Fabrication | Custom Motherboard | Main PCB with replaceable Raspberry Arduino nano headers, power regulation, and sensor interfaces | $58.00 |
| **Subtotal** | | | **$183.00** |

### 2. Electronics and Sensors

| Component | Specification / Purpose | Qty. | Unit Cost (USD) | Total (USD) | Link |
|---|---|---:|---:|---:|---:|
| Servo Motor | Servo rotation control | 6 | $7.40 | $44.40 | [Link](https://shorturl.at/46V4L) |
| Drive Motor | Propulsion | 1 | $46.00 | $46.00 | [Link](https://www.aliexpress.com/item/1005006684228018.html)|
|  CanMV K230 mini AI development board  | Image processing and onboard computing | 1 | $43.37  | $43.37  | [Link](https://www.aliexpress.com/item/1005008934429939.html)|
| Arduino Nano V3.0 Type C  | Sensor interfacing and data acquisition | 1 | $3.00 | $3.00 | [Link](https://www.aliexpress.com/item/1005011889513227.html)|
|  8x8 Thermal Imager Module | Thermal imaging for research | 1 | $32.08  | $32.08  | [Link](https://www.aliexpress.com/item/1005009168490634.html)|
| Gyro Sensor | 3-axis motion and orientation sensing | 1 | $9.51 | $9.51 | [Link](https://www.aliexpress.com/item/1005008666420561.html)|
| Lithium-ion Battery | Rechargeable power supply | 1 | $22.10 | $22.10 | [Link](https://www.aliexpress.com/item/1005006920168445.html)|
| Extension Cable | 20 m communication/data cable | 1 | $78.70 | $78.70 | [Link](https://www.aliexpress.com/item/1005012780715462.html)|
| Memory Card | 32 GB microSD card | 1 | $10.43  | $10.43  | [Link](https://www.aliexpress.com/item/1005007498167692.html)|
| Light/Infrared Color Spectrometer | Light measurement and spectral analysis | 1 | $8.01 | $8.01 | [Link](https://www.aliexpress.com/item/1005013219123992.html)|
| NEO-M8N GPS Module  |1 | $17.49 | $17.49 |  [Link](https://www.aliexpress.com/item/1005008748794240.html)|

| **Subtotal** | | | | **$345.50** |

### 3. Miscellaneous and Logistics

| Component | Description | Estimated Cost (USD) |
|---|---|---:|
| Passive Components and Hardware | Resistors, capacitors, connectors, and other miscellaneous parts | $15.00 |
| Shipping | Estimated shipping charges | $50.00 |
| **Subtotal** | | **$65.00** |

### 4. Estimated Project Cost

| Category | Estimated Cost (USD) |
|---|---:|
| Mechanical and PCB Fabrication | $183.00 |
| Electronics and Sensors | $345.50 |
| Miscellaneous and Shipping | $65.00 |
| **Total Estimated Cost** | **$593.50** |

> **Note:** All prices are approximate and may vary depending on supplier, availability, shipping, and import duties. Additional waterproof connectors, cable glands, motor drivers, battery protection, and pressure-resistant sealing may increase the final cost if they are not already included.

### 5. Mainboard Design Overview

The custom motherboard is designed around a removable Arduino Nano, connected through headers rather than permanently soldered to the PCB. The board is intended to provide:

- Sensor interfaces using I²C and SPI.
- MicroSD storage interface for sensor readings and other data the Pico can manage.
- USB/UART communication with external equipment.
- Gyroscope interface for motion and stability measurements.
- Motor-driver and servo-control connections.
- 5 V and 3.3 V power regulation.



**Design consideration:** 
