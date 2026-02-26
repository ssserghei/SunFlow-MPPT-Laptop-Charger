# SunFlow-MPPT-Laptop-Charger/ Solar-to-USB-C Laptop Charger
---

This repository contains the documentation and hardware specifications for a modular Solar MPPT Charger system, designed as a 3-layer "sandwich" assembly in Altium Designer.

## 🛠 System Architecture

The project is designed as a modular high-power solar charging solution, consisting of three interconnected layers that form a high-performance "sandwich" assembly.
1. MPPT Control Unit (Power Management)
* Core Controller: Based on the LT8491 High Voltage Buck-Boost Battery Charging Controller.
* Function: Handles the sophisticated MPPT algorithm and optimized battery charging profiles.
* Communication: Provides an I2C interface to output system telemetry (voltage, current, and temperature) to the monitoring unit.
2. Power Stage (H-Bridge)Topology: 
* Features a 4-switch H-Bridge Buck-Boost configuration.
* Capability: Efficiently steps voltage up or down, allowing the system to work with solar panel voltages both above and below the battery voltage.
* Thermal Design: Optimized PCB layout for high-current handling and heat dissipation.
3. Smart Monitoring & Interface Unit (HMI)Main MCU: STM32 microcontroller that acts as the system's "brain" for data processing and user interface.
* Visual Interface: Integrated 128x32 OLED display for real-time visualization of power, energy ($Wh$), and charging status.
* Precision Sensing: Utilizes the INA237 16-bit ADC for ultra-accurate high-side current monitoring up to 85V.
* Standalone Capability: Equipped with XT-60, USB-A, and USB-C ports, allowing it to function as a universal standalone power meter.

| Top View |
| :---: | 
| ![Top View](<https://github.com/ssserghei/SunFlow-MPPT-Laptop-Charger/blob/ba2cd1cfb76640df7c12672f7040a9a51f43a725/Solar%20MPPT%20Charger%20Assembly/main_assembly_3D.jpg.jpg>)|

---

### 2. MPPT Charger Power

The power conversion stage responsible for efficient energy transfer from solar panels to batteries.

| Top View | Bottom View |
| :---: | :---: |
| ![Top View](<Solar MPPT Charger Power/PCB 3D Print_TOP/SSS_MPPT_Charger_Power_PCB 3D Print.png>) | ![Bottom View](<Solar MPPT Charger Power/PCB 3D Print_BOT/SSS_MPPT_Charger_Power_PCB 3D Print.png>)    |

**Documentation:**

* 📄 [Schematic (PDF)](https://github.com/ssserghei/SunFlow-MPPT-Laptop-Charger/blob/811f29efc645808a5f0bbe54c9bd5787e2f680a9/Solar%20MPPT%20Charger%20Power/Schematic%20Prints/SSS_MPPT_Charger_Power.PDF)
* 🛠️ [Assembly Drawing](https://github.com/ssserghei/SunFlow-MPPT-Laptop-Charger/blob/811f29efc645808a5f0bbe54c9bd5787e2f680a9/Solar%20MPPT%20Charger%20Power/Assembly%20drawing/SSS_MPPT_Charger_Power_Assembly%20drawing.PDF)
* 📋 [Bill of Materials (BOM)](https://github.com/ssserghei/SunFlow-MPPT-Laptop-Charger/blob/811f29efc645808a5f0bbe54c9bd5787e2f680a9/Solar%20MPPT%20Charger%20Power/BOM%20Factory/SSS_MPPT_Charger_Power_BOM.xlsx)

---

### 3. MPPT Charger Control

The logic and control unit that manages the charging profiles, display interface, and communications.

| Top View | Bottom View |
| :---: | :---: |
| ![Top View](<Solar MPPT Charger Control/PCB 3D Print_TOP/SSS_MPPT_Charger_Control_PCB 3D Print.png>) | ![Bottom View](<Solar MPPT Charger Control/PCB 3D Print_BOT/SSS_MPPT_Charger_Control_PCB 3D Print.png>)    |

**Documentation:**

* 📄 [Schematic (PDF)](https://github.com/ssserghei/SunFlow-MPPT-Laptop-Charger/blob/ba2cd1cfb76640df7c12672f7040a9a51f43a725/Solar%20MPPT%20Charger%20Control/Schematic%20Prints/SSS_MPPT_Charger_Control.PDF)
* 🛠️ [Assembly Drawing](https://github.com/ssserghei/SunFlow-MPPT-Laptop-Charger/blob/811f29efc645808a5f0bbe54c9bd5787e2f680a9/Solar%20MPPT%20Charger%20Control/Assembly%20drawing/SSS_MPPT_Charger_Control_Assembly%20drawing.PDF)
* 📋 [Bill of Materials (BOM)](https://github.com/ssserghei/SunFlow-MPPT-Laptop-Charger/blob/ba2cd1cfb76640df7c12672f7040a9a51f43a725/Solar%20MPPT%20Charger%20Control/BOM%20Factory/SSS_MPPT_Charger_Control_BOM.xlsx)

---
### 1. Current Monitoring Tool (Standalone/Integrated)

A high-precision power analyzer based on the **INA237** (16-bit, 85V). It features a unique star-shaped layout with XT-60, USB-A, and USB-C connectors.

| Top View | Bottom View |
| :---: | :---: |
| ![Top View](<Solar MPPT Charger Current Monitoring Tool/PCB 3D Print_TOP/SSS_Current_Monitoring_PCB 3D Print.png>) | ![Bottom View](<Solar MPPT Charger Current Monitoring Tool/PCB 3D Print_BOT/SSS_Current_Monitoring_PCB 3D Print.png>)    |

**Documentation:**

* 📄 [Schematic (PDF)](https://github.com/ssserghei/SunFlow-MPPT-Laptop-Charger/blob/ba2cd1cfb76640df7c12672f7040a9a51f43a725/Solar%20MPPT%20Charger%20Current%20Monitoring%20Tool/Schematic%20Prints/SSS_Current_Monitoring.PDF)
* 🛠️ [Assembly Drawing](https://github.com/ssserghei/SunFlow-MPPT-Laptop-Charger/blob/ba2cd1cfb76640df7c12672f7040a9a51f43a725/Solar%20MPPT%20Charger%20Current%20Monitoring%20Tool/Assembly%20drawing/SSS_Current_Monitoring_Assembly%20drawing.PDF)
* 📋 [Bill of Materials (BOM)](https://github.com/ssserghei/SunFlow-MPPT-Laptop-Charger/blob/ba2cd1cfb76640df7c12672f7040a9a51f43a725/Solar%20MPPT%20Charger%20Current%20Monitoring%20Tool/BOM%20Factory/SSS_Current_Monitoring_BOM.xlsx)
  
---

**🛠 Manufacturing Note:**

Please note that this repository contains documentation only (PDF Schematics, Assembly Drawings, and BOM).
- Gerber Files: Not included in this public preview.
- Source Files: Altium Designer project files are kept private to protect the core intellectual property.
- Note: If you are interested in the full design files, or a technical deep-dive into the LT8491 configuration, feel free to contact me directly via GitHub.

---

**⚠️ Project Status: In Development**

Important: The project is currently in the second prototype design stage and may contain errors or unverified hardware configurations. If you are interested in replicating this design, please wait for the official test results and hardware validation.

---

