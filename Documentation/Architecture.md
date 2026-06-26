# System Architecture

## Overview

The Home Energy Management System (HEMS) is a modular embedded platform designed to monitor, manage and optimise residential energy systems. The system is built around a distributed architecture where each subsystem performs a dedicated function and communicates over a Controller Area Network (CAN) bus. This modular approach allows individual components to be developed, tested and upgraded independently while maintaining interoperability across the entire system. The long-term objective is to integrate battery management, renewable energy, energy monitoring, automation and robotics into a single scalable platform.

---

## High-Level Architecture

<img width="476" height="597" alt="image" src="https://github.com/user-attachments/assets/f70f5b7f-f009-478d-91d6-ac14b2d71974" />


---

# Subsystems

## Battery Pack

The Battery Pack provides the primary energy storage for the system. It supplies electrical power to all connected subsystems and acts as the central energy source for charging, monitoring and energy management.

---

## Battery Management System (BMS)

The Battery Management System monitors the operating condition of the battery pack. It measures electrical and thermal parameters, estimates battery state and provides protection against unsafe operating conditions. The BMS also communicates battery information to the rest of the system.

---

## MPPT Charger

The Maximum Power Point Tracking (MPPT) charger manages energy transfer from a renewable energy source to the battery. Its purpose is to maximise charging efficiency while maintaining safe charging conditions.

---

## CAN Bus Network

The CAN Bus Network provides reliable communication between all system modules. It allows distributed devices to exchange data without requiring direct point-to-point wiring, enabling a scalable and modular architecture.

---

## Gateway Controller

The Gateway Controller acts as the central communication hub for the system. It collects information from the CAN network and makes it available to external software platforms such as Home Assistant and future web-based dashboards.

---

## Display Node

The Display Node provides a local human-machine interface (HMI) for the system. It presents operating information including battery status, power flow and system diagnostics.

---

## Sensor Nodes

Sensor Nodes collect environmental and electrical measurements throughout the system. These measurements provide additional data for monitoring, automation and future control strategies.

---

## Home Assistant

Home Assistant provides a central software platform for visualising system performance, storing historical data and implementing automation rules. It enables users to monitor the system remotely through a unified dashboard.

---

## Robotic Arm

The Robotic Arm is an optional expansion module designed to demonstrate system integration beyond energy management. It provides a programmable automation platform that can interact with the physical environment while sharing information with the rest of the HEMS network.

---

# Design Philosophy

The Home Energy Management System is designed around the following engineering principles:

- Modular subsystem architecture
- Distributed CAN bus communication
- Expandable hardware design
- Custom PCB development
- Scalable embedded software
- Maintainable system documentation
- Industry-standard engineering practices
- Iterative hardware and firmware development

---

# Future Expansion

The architecture has been designed to support future modules without requiring significant redesign. Planned future expansions include:

- Smart load management
- Grid monitoring
- Battery balancing
- EV charger integration
- Three-phase power monitoring
- Solar forecasting
- Machine learning energy optimisation
- Mobile application
- Voice assistant
- Industrial communication protocols
