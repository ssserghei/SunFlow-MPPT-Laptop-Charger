# SunFlow-MPPT-Laptop-Charger
High-Efficiency Solar-to-USB-C Laptop Charger
---

This repository contains the documentation and hardware specifications for a modular Solar MPPT Charger system, designed as a 3-layer "sandwich" assembly in Altium Designer.

## 🛠 System Architecture

The project is divided into three functional modules, each with its own dedicated documentation:

---

### 2. MPPT Charger Power

The power conversion stage responsible for efficient energy transfer from solar panels to batteries.

| Top View | Bottom View |
| --- | --- |
|  |  |

**Documentation:**

* 📄 [Schematic (PDF)](https://www.google.com/search?q=Solar_MPPT_Charger_Power/Schematic_Prints/%3CPOWER_SCHEMATIC_PDF%3E)
* 🛠️ [Assembly Drawing](https://www.google.com/search?q=Solar_MPPT_Charger_Power/Assembly_drawing/%3CPOWER_ASSEMBLY_PDF%3E)
* 📋 [Bill of Materials (BOM)](https://www.google.com/search?q=Solar_MPPT_Charger_Power/BOM_Factory/%3CPOWER_BOM_XLSX%3E)

---

### 3. MPPT Charger Control

The logic and control unit that manages the charging profiles, display interface, and communications.

**Documentation:**

* 📄 [Schematic (PDF)](https://www.google.com/search?q=Solar_MPPT_Charger_Control/Schematic_Prints/%3CCONTROL_SCHEMATIC_PDF%3E)
* 🛠️ [Assembly Drawing](https://www.google.com/search?q=Solar_MPPT_Charger_Control/Assembly_drawing/%3CCONTROL_ASSEMBLY_PDF%3E)
* 📋 [Bill of Materials (BOM)](https://www.google.com/search?q=Solar_MPPT_Charger_Control/BOM_Factory/%3CCONTROL_BOM_XLSX%3E)

---

## ⚡ Technical Specs

* **ADC:** TI INA237 (85V, 16-bit, Ultra-precise sensing)
* **Interfaces:** XT-60, USB-C (Symmetrical support), USB-A 3.0
* **Design:** 4-layer PCB with dedicated GND planes for noise immunity.

## 🚀 How to use this Repo

This repository is for documentation purposes. To order or manufacture these boards, please refer to the assembly drawings and BOM files in each respective folder.

---

### 1. Current Monitoring Tool (Standalone/Integrated)

A high-precision power analyzer based on the **INA237** (16-bit, 85V). It features a unique star-shaped layout with XT-60, USB-A, and USB-C connectors.

| Top View | Bottom View |
| --- | --- |
|  |  |

**Documentation:**

* 📄 [Schematic (PDF)](https://www.google.com/search?q=Solar_MPPT_Charger_Current_Monitoring_Tool/Schematic_Prints/%3CMONITOR_SCHEMATIC_PDF%3E)
* 🛠️ [Assembly Drawing](https://www.google.com/search?q=Solar_MPPT_Charger_Current_Monitoring_Tool/Assembly_drawing/%3CMONITOR_ASSEMBLY_PDF%3E)
* 📋 [Bill of Materials (BOM)](https://www.google.com/search?q=Solar_MPPT_Charger_Current_Monitoring_Tool/BOM_Factory/%3CMONITOR_BOM_XLSX%3E)
  
---
