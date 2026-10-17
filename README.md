# AUV-labyrinth

#### Outlook

![image alt](https://github.com/hossainmahmudchowdhury-boop/AUV-labyrinth/blob/main/Images/Screenshot%202026-10-01%20182908.png)

This project is about an underwater submarine that can follow a route to survey the aquatic environment. It can detect the number of fish in an area and observe aquatic biology. In this project, it emphasizes an ML-based detection system and a water quality checker.
![image alt](https://github.com/hossainmahmudchowdhury-boop/AUV-labyrinth/blob/main/Images/Screenshot%202026-10-05%20205444.png)

### PCB Loading.....

## Bill of Materials (BOM)

The following table lists the estimated components and costs for the underwater surveillance submarine prototype. The system combines onboard image processing, sensor data collection, underwater imaging, and remote communication.

### 1. Mechanical and PCB Fabrication

| Category | Component | Description | Estimated Cost (USD) |
|---|---|---|---:|
| Mechanical | Waterproof 3D Printing | Custom submarine body | $125.00 |
| PCB Fabrication | Custom Motherboard | Main PCB with replaceable Raspberry Pi Pico headers, power regulation, and sensor interfaces | $58.00 |
| **Subtotal** | | | **$183.00** |

### 2. Electronics and Sensors

| Component | Specification / Purpose | Qty. | Unit Cost (USD) | Total (USD) |
|---|---|---:|---:|---:|
| Servo Motor | Servo rotation control | 6 | $1.20 | $7.20 |
| Drive Motor | Propulsion | 2 | $2.00 | $4.00 |
| Raspberry Pi Zero 2 W | Image processing and onboard computing | 1 | $32.65 | $32.65 |
| Raspberry Pi Pico | Sensor interfacing and data acquisition | 1 | $3.00 | $3.00 |
| Raspberry Pi Camera | Visual imaging | 1 | $9.71 | $9.71 |
| Thermal Camera | Thermal imaging for research | 1 | $23.02 | $23.02 |
| Gyro Sensor | 4-axis motion and orientation sensing | 1 | $8.91 | $8.91 |
| Lithium-ion Battery | Rechargeable power supply | 1 | $25.00 | $25.00 |
| Extension Cable | 30 m communication/data cable | 1 | $39.51 | $39.51 |
| Memory Card | 32 GB microSD card | 1 | $17.14 | $17.14 |
| Light/Infrared Color Spectrometer | Light measurement and spectral analysis | 1 | $8.01 | $8.01 |
| **Subtotal** | | | | **$178.15** |

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
| Electronics and Sensors | $178.15 |
| Miscellaneous and Shipping | $65.00 |
| **Total Estimated Cost** | **$426.15** |

> **Note:** All prices are approximate and may vary depending on supplier, availability, shipping, and import duties. Additional waterproof connectors, cable glands, motor drivers, battery protection, and pressure-resistant sealing may increase the final cost if they are not already included.

### 5. Mainboard Design Overview

The custom motherboard is designed around a removable Raspberry Pi Pico, connected through headers rather than permanently soldered to the PCB. The board is intended to provide:

- Sensor interfaces using I²C and SPI.
- MicroSD storage interface for sensor readings and other data the Pico can manage.
- USB/UART communication with external equipment.
- Gyroscope interface for motion and stability measurements.
- Motor-driver and servo-control connections.
- 5 V and 3.3 V power regulation.
- Voltage and current monitoring.

The Raspberry Pi Zero 2 W handles camera-related processing, while the Pico focuses on sensor acquisition and low-level control. Thermal imaging and spectral processing may require additional software, interfaces, or processing resources, depending on the selected modules.

**Design consideration:** The Pico is not intended to replace the Raspberry Pi Zero 2 W as the main image-processing computer. The final PCB layout and power system should be verified against the electrical requirements of each connected module.
