# System Requirements

**Project:** Home Energy Management System (HEMS)

**Document Version:** 1.0

**Status:** Draft

**Author:** Chris Mazzer

**Last Updated:** 26 June 2026

---

# 1. Introduction

## 1.1 Purpose

This document defines the functional and non-functional requirements for the Home Energy Management System (HEMS).

The HEMS project aims to develop a modular embedded platform capable of monitoring, managing and optimising residential energy systems. It combines power electronics, battery management, embedded systems, PCB design, industrial communication and software engineering into a scalable architecture suitable for future expansion.

This document provides the baseline requirements that will guide hardware selection, firmware development, PCB design and system testing throughout the project.

---

## 1.2 Scope

Version 1 focuses on the development of a Battery Management System (BMS) capable of:

- Monitoring battery voltage
- Monitoring battery current
- Monitoring battery temperature
- Estimating battery State of Charge (SOC)
- Calculating power and energy usage
- Transmitting measurements over a CAN bus
- Displaying operating information locally
- Logging system data

Future releases will introduce solar charging, Home Assistant integration, smart load management and robotics.

---

# 2. Functional Requirements

## 2.1 Battery Monitoring

The Battery Management System forms the core of the project and is responsible for continuously monitoring the operating condition of the battery.

| ID | Requirement |
|----|-------------|
| FR-001 | Measure battery voltage. |
| FR-002 | Measure battery current. |
| FR-003 | Monitor battery temperature. |
| FR-004 | Estimate battery State of Charge (SOC). |
| FR-005 | Calculate instantaneous power. |
| FR-006 | Calculate accumulated energy transferred into and out of the battery. |

---

## 2.2 Communication

All distributed modules communicate over a CAN bus network.

| ID | Requirement |
|----|-------------|
| FR-007 | Broadcast battery measurements over the CAN bus. |
| FR-008 | Receive configuration commands from authorised CAN nodes. |
| FR-009 | Timestamp logged measurements. |
| FR-010 | Detect communication faults. |

---

## 2.3 User Interface

Users should be able to view system status without connecting additional equipment.

| ID | Requirement |
|----|-------------|
| FR-011 | Display battery information locally. |
| FR-012 | Indicate operating status using LEDs. |
| FR-013 | Provide diagnostic information through USB serial. |
| FR-014 | Display system fault messages. |

---

## 2.4 Data Logging

Historical operating data is useful for analysis, testing and fault finding.

| ID | Requirement |
|----|-------------|
| FR-015 | Record battery measurements. |
| FR-016 | Store timestamps with logged data. |
| FR-017 | Allow recorded data to be exported. |

---

## 2.5 Safety & Protection

The system must detect unsafe operating conditions and notify the user.

| ID | Requirement |
|----|-------------|
| FR-018 | Detect battery over-voltage. |
| FR-019 | Detect battery under-voltage. |
| FR-020 | Detect excessive current draw. |
| FR-021 | Detect excessive battery temperature. |
| FR-022 | Report faults over the CAN network. |

---

# 3. Non-Functional Requirements

## 3.1 Performance

| ID | Requirement |
|----|-------------|
| NFR-001 | Voltage measurement accuracy better than ±1%. |
| NFR-002 | Current measurement accuracy better than ±2%. |
| NFR-003 | Temperature accuracy within ±2 °C. |
| NFR-004 | Configurable CAN transmission interval. |

---

## 3.2 Reliability

| ID | Requirement |
|----|-------------|
| NFR-005 | Operate continuously for at least 24 hours without requiring a restart. |
| NFR-006 | Recover automatically following power restoration. |
| NFR-007 | Detect sensor failures where possible. |

---

## 3.3 Maintainability

The project is intended to follow good engineering practices throughout development.

| ID | Requirement |
|----|-------------|
| NFR-008 | Use modular firmware architecture. |
| NFR-009 | Separate hardware into independent subsystems where practical. |
| NFR-010 | Maintain complete design documentation within the GitHub repository. |
| NFR-011 | Track all hardware and software revisions using Git. |

---

## 3.4 Scalability

The architecture should support future expansion without major redesign.

| ID | Requirement |
|----|-------------|
| NFR-012 | Support additional CAN nodes. |
| NFR-013 | Allow future Home Assistant integration. |
| NFR-014 | Support future MPPT charger integration. |
| NFR-015 | Support future robotic arm integration. |
| NFR-016 | Allow future battery chemistry upgrades. |

---

# 4. Design Constraints

The following constraints define the initial design boundaries.

| Item | Constraint |
|------|------------|
| Controller | ESP32 |
| Communication | CAN Bus |
| PCB Software | KiCad |
| CAD Software | Fusion 360 |
| Mechanical Components | 3D Printed |
| Version Control | GitHub |
| Development | Modular architecture |

---

# 5. Assumptions

The following assumptions apply to Version 1 of the project.

- Development will be performed using laboratory equipment.
- The initial prototype will operate from a low-voltage DC battery.
- CAN bus will be the primary communication protocol.
- Hardware will be developed incrementally through multiple PCB revisions.
- Additional features will be introduced over several development phases.

---

# 6. Future Scope

The following features are planned but fall outside the scope of Version 1.

## Power Electronics

- MPPT solar charger
- Battery balancing
- DC-DC converter optimisation
- Solar generation monitoring

## Smart Home

- Home Assistant integration
- MQTT communication
- Remote monitoring
- Smart automation

## Robotics

- Desktop robotic arm
- Computer vision
- Automated tool handling
- Voice interaction

## Energy Management

- Smart load shedding
- Grid monitoring
- EV charger integration
- Three-phase energy monitoring
- Predictive energy analytics

---

# 7. Requirement Verification

Each requirement will be verified during development using one or more of the following methods.

| Method | Description |
|---------|-------------|
| Inspection | Review of hardware, software or documentation. |
| Test | Physical testing of the completed system. |
| Analysis | Mathematical calculations or simulations. |
| Demonstration | Functional operation under normal conditions. |

---

# 8. Revision History

| Version | Date | Description |
|----------|------------|---------------------------|
| 1.0 | 26 June 2026 | Initial system requirements. |
