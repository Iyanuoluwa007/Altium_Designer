# Embedded Control System for an Autonomous Cleaning Robot

This repository documents the design and implementation of the **electronic control system** for an autonomous cleaning robot. It includes detailed PCB and schematic designs created using **Altium Designer**, covering four main subsystems: Power Supply Unit (PSU), USB Control Unit (UCU), Microcontroller Unit (MCU), and Motor Driver Unit (MDU).

## 📌 Project Overview

The objective was to create a robust, modular embedded control system capable of powering and managing key robotic functions such as:

- Obstacle detection and avoidance  
- Motor control and path navigation  
- Wireless communication via ESP32  
- Integration with peripherals like cameras, ultrasonic sensors, and LCDs  

## 🔧 Hardware Components

- **PSU:** Based on LM2596T-5.0 and LM2596T-3.3 for 5V and 3.3V outputs  
- **UCU:** FT232RL-based USB-to-Serial interface  
- **MCU:** ATmega128 microcontroller interfacing with sensors and wireless modules  
- **MDU:** L6205 dual full-bridge motor driver for bidirectional DC motor control  
- **PCB Tool:** Altium Designer (schematic, layout, DRC, and 3D visualization)

## 📁 Folder Structure

```
/schematics         - Schematic files (.SchDoc)
/pcb_layouts        - PCB layout files (.PcbDoc)
/3d_views           - 3D renderings and screenshots
/outputs            - Gerbers, BOM, and PDFs
/docs               - Full project report
```

## ✅ Features

- Power-efficient voltage regulation with thermal management
- Fault-protected motor driver system
- Multiplexed UART switching for optimized communication
- Altium DRC-verified PCB designs with ground polygon pour
- Modular design enabling system scalability

## 📷 Previews

| Schematic | PCB Layout | 3D Render |
|----------|------------|-----------|
| PSU, UCU, MCU, MDU | 2D Altium Layout | Full-board 3D View |

> Note: Visuals available in the `3d_views/` and `outputs/` folders.

## 🔬 Testing & Validation

- **DRC:** No critical violations (Silk-to-solder mask clearance warning only)
- **Thermal Analysis:** Optimized using hatched polygon pour
- **System Integration:** Verified functional with all sensors and modules

## 📡 Future Improvements

- Add heatsinks/fans for thermal management  
- Upgrade to brushless DC motors  
- Include current sensing for real-time diagnostics  
- Add supercapacitor-based backup power

## 📚 References

Key component datasheets and academic papers are cited in the full [project report](./docs/Oke_Iyanuoluwa_Mech_Report.pdf).

## 👥 Authors

- **Oke Iyanuoluwa Enoch**  
- Team: Love Akinrele, Ifeorah Anthony, Revanth Reddy  
- MSc Robotics and Automation, University of Salford
