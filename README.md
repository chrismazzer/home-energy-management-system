# Home Energy Management System (HEMS)

> A modular Home Energy Management System designed to monitor, control and optimise residential energy systems using embedded electronics, power electronics, CAN bus networking and Home Assistant integration.
---

# Overview

The Home Energy Management System (HEMS) is a long-term engineering project focused on the design and development of a modular platform for monitoring, controlling and optimising residential energy systems.

The project aims to combine embedded systems, battery management, power electronics, industrial communication, custom PCB design and software engineering into a single integrated platform.

Rather than being a single device, HEMS is designed as a collection of interconnected modules communicating over a CAN bus network. This modular approach allows the system to be expanded over time while following engineering design practices commonly used in industry.

This project is being developed as a personal engineering portfolio while studying Electrical Engineering to gain practical experience in power electronics, embedded systems, PCB design, industrial communication and systems engineering.

---

# Project Objectives

The primary objectives of this project are to:

- Design a modular Battery Management System (BMS)
- Monitor battery voltage, current and temperature
- Estimate battery State of Charge (SOC)
- Design custom PCBs using KiCad
- Develop embedded firmware for ESP32 microcontrollers
- Implement CAN bus communication between system modules
- Develop an energy monitoring dashboard
- Integrate with Home Assistant
- Design an MPPT solar charger
- Build a modular robotic assistant for desktop automation
- Document the complete engineering design process

---

# Planned Features

## Battery Management

- Battery voltage monitoring
- Battery current monitoring
- Battery temperature monitoring
- State of Charge estimation
- Battery health monitoring
- Data logging
- Battery protection
- Cell balancing (future)

---

## Power Electronics

- MPPT solar charging
- Buck converter
- Battery charging algorithms
- Power measurement
- Energy monitoring
- Efficiency analysis

---

## Embedded Systems

- ESP32 firmware
- Sensor interfaces
- CAN bus communication
- Fault detection
- OTA firmware updates
- Real-time monitoring

---

## Dashboard

- Live battery data
- Historical graphs
- Energy consumption
- Solar generation monitoring
- Device diagnostics
- System alerts

---

## Home Assistant Integration

- MQTT communication
- Device discovery
- Automation support
- Mobile dashboard
- Remote monitoring

---

## Mechanical Design

- Custom 3D printed enclosure
- Modular PCB mounting
- Cable management
- Cooling system
- Professional enclosure design

---

# Planned System Architecture

```text
                  Solar Panel
                       │
                 MPPT Charger
                       │
                  Battery Pack
                       │
            Battery Management System
                       │
                   CAN Bus Network
      ┌──────────────┼──────────────┐
      │              │              │
  Display Node   Sensor Nodes   Robotic Arm
      │
 Raspberry Pi Gateway
      │
 Home Assistant Dashboard
```

---

# Hardware

## Current Hardware

- ESP32 Development Boards
- CAN Bus Modules
- 3D Printer
- Electronic test equipment
- Assorted sensors
- Breadboarding equipment

## Planned Hardware

- Custom PCB
- Current Sensors
- Voltage Monitoring Circuit
- Temperature Sensors
- LiFePO₄ Battery Pack
- MPPT Charger
- TFT Display
- Raspberry Pi
- Robotic Arm

---

# Software

## Embedded

- C/C++
- ESP-IDF
- Arduino Framework
- FreeRTOS

## Desktop

- Python

## Dashboard

- Home Assistant
- MQTT

## Engineering Tools

- KiCad
- Fusion 360
- Git
- GitHub

---

# Repository Structure

```text
Home-Energy-Management-System/
│
├── Documentation/
│   ├── Requirements
│   ├── Architecture
│   ├── Design Decisions
│   ├── Test Plans
│   └── Project Journal
│
├── Hardware/
│   ├── PCB
│   ├── Schematics
│   ├── BOM
│   └── Datasheets
│
├── Firmware/
│
├── Software/
│
├── CAD/
│
├── Testing/
│
├── Images/
│
└── README.md
```

---

# Development Roadmap

## Phase 1 — Battery Monitoring

- [ ] Define system requirements
- [ ] Select battery chemistry
- [ ] Measure battery voltage
- [ ] Measure battery current
- [ ] Measure battery temperature
- [ ] Estimate State of Charge

---

## Phase 2 — CAN Bus Network

- [ ] Design CAN architecture
- [ ] Implement communication protocol
- [ ] Test multiple CAN nodes

---

## Phase 3 — PCB Design

- [ ] Design PCB Revision A
- [ ] Manufacture PCB
- [ ] Assemble PCB
- [ ] Hardware validation

---

## Phase 4 — Dashboard

- [ ] Local display
- [ ] Web dashboard
- [ ] Historical logging
- [ ] Notifications

---

## Phase 5 — Home Assistant

- [ ] MQTT integration
- [ ] Device discovery
- [ ] Dashboard
- [ ] Automation

---

## Phase 6 — Power Electronics

- [ ] MPPT charger
- [ ] Charging control
- [ ] Battery protection
- [ ] Efficiency testing

---

## Phase 7 — Robotics

- [ ] Robotic arm
- [ ] CAN integration
- [ ] Desktop automation
- [ ] Vision system

---

# Current Status

**Project Phase:** Planning & System Architecture

Current focus:

- Repository setup
- System requirements
- Hardware architecture
- Initial subsystem design

---

# Future Improvements

Potential future additions include:

- Battery balancing
- Smart load shedding
- Grid monitoring
- EV charger integration
- Machine learning energy prediction
- Three-phase power monitoring
- Mobile application
- Voice assistant
- Predictive maintenance

---

# Contributing

This is currently a personal engineering project. Suggestions and feedback are always welcome through GitHub Issues.

---

# License

This project is not currently liscenced.

---

# Author

**Chris Mazzer**

Bachelor of Electrical Engineering (Honours)

The University of Queensland

This repository documents the complete engineering design, development and testing process of the Home Energy Management System project.

