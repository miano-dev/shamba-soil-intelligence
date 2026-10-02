# Shamba Soil Intelligence

### IoT-Based Soil Fertility Monitoring, NPK Sensing & Agricultural Intelligence

**Status:** Working prototype / field-developed system  
**Hardware:** ESP32 SoC · NPK soil probe · Raspberry Pi · Custom PCB  
**Software:** Web application · Soil monitoring · Satellite data integration  
**IP:** Core implementation is proprietary and under patent protection

## Overview

**Shamba Soil Intelligence** is a physical IoT system developed to monitor soil fertility and environmental conditions at farm level and present the resulting information through a digital application.

The system combines:

- An **ESP32-based sensing device**
- An **NPK soil probe**
- A **custom printed PCB**
- A **Raspberry Pi edge/gateway platform**
- A **web application**
- **Satellite data**
- Farm-level data visualization and analysis

The objective is to connect measurements from the physical soil environment with digital agricultural intelligence that can be used to understand conditions within a specific farm or shamba.

> **This repository documents the engineering architecture and development work. The source code, PCB design files, detailed circuit schematics, firmware implementation and other proprietary technical information are intentionally not published because the technology is under patent protection.**

---

## System Architecture

```text
                    ┌─────────────────────┐
                    │     FARM / SHAMBA   │
                    │                     │
                    │   Soil Conditions   │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │     NPK PROBE       │
                    │                     │
                    │  Soil Fertility     │
                    │  Measurements       │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │       ESP32         │
                    │                     │
                    │ Sensor Interface    │
                    │ Processing          │
                    │ Connectivity        │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │    RASPBERRY PI     │
                    │                     │
                    │ Edge / Gateway      │
                    │ Data Processing     │
                    │ Communications      │
                    └──────────┬──────────┘
                               │
                    ┌──────────┴──────────┐
                    │                     │
                    ▼                     ▼
          ┌─────────────────┐   ┌─────────────────┐
          │  WEB APPLICATION│   │ SATELLITE DATA  │
          │                 │   │                 │
          │ Monitoring      │   │ Farm / Field    │
          │ Visualization   │   │ Intelligence    │
          │ Analysis        │   │                 │
          └────────┬────────┘   └────────┬────────┘
                   │                     │
                   └──────────┬──────────┘
                              ▼
                    ┌─────────────────────┐
                    │ AGRICULTURAL        │
                    │ INTELLIGENCE        │
                    │                     │
                    │ Farm-level insight  │
                    │ & decision support  │
                    └─────────────────────┘
```

## Hardware

The physical monitoring platform was developed around an **ESP32 system-on-chip** and an **NPK soil probe**.

| Component | Role |
|---|---|
| ESP32 SoC | Embedded sensing, processing and connectivity |
| NPK probe | Soil nutrient measurement |
| Custom PCB | Device integration and electrical interface |
| Raspberry Pi | Edge computing / gateway |
| Power electronics | Device power and regulation |
| Soil interface | Physical connection to the monitored environment |

The device is a purpose-built engineering system rather than a software-only demonstration.

## Embedded System

The ESP32 forms the embedded control and sensing layer. Its responsibilities include the interface between the physical sensing hardware and the higher-level data system.

The embedded architecture addresses:

- Sensor interfacing
- Measurement acquisition
- Device processing
- Communications
- Device-level control
- Data transfer
- Hardware/software integration

The detailed firmware implementation is proprietary and is therefore not included in this repository.

## Custom PCB

A printed PCB was developed for the physical device. The PCB provides the electrical integration between the sensing hardware, embedded controller and supporting electronics.

The actual PCB design files, schematics, Gerbers, component-level design information and production files are intentionally withheld from this public repository because they form part of the protected technology.

A high-level block diagram is provided instead to demonstrate the engineering architecture.

## Raspberry Pi Edge Platform

A Raspberry Pi is used as part of the edge/gateway layer. The edge platform provides an intermediate computing and communication layer between the physical monitoring device and the application environment.

This architecture separates:

**Device sensing → edge processing → application/data services**

## Web Application

A dedicated web application was developed to make the collected agricultural information accessible through a digital interface.

The application provides the software layer for:

- Farm monitoring
- Soil information
- Sensor data visualization
- Farm-level analysis
- Digital presentation of measurements
- Integration of additional agricultural information

Screenshots and demonstrations can be added without exposing the underlying implementation.

## Satellite Data

The system also incorporates satellite information as an additional source of agricultural intelligence.

The purpose is to complement measurements from the physical soil-monitoring device with broader information about the farm and surrounding field conditions.

```text
Physical Measurements
        +
Satellite Information
        +
Farm Data
        │
        ▼
Agricultural Intelligence
```

## Engineering Challenges

The project involved engineering across several layers.

### Hardware

- Sensor integration
- Embedded controller selection
- PCB development
- Electrical interfaces
- Physical deployment considerations

### Embedded

- ESP32 development
- Sensor communication
- Measurement acquisition
- Device connectivity
- Hardware/software integration

### Edge Computing

- Raspberry Pi integration
- Device-to-gateway communication
- Data handling
- Edge architecture

### Software

- Web application development
- Data visualization
- Application architecture
- Agricultural information presentation

### Systems Integration

The project required integration between:

**Sensors → embedded electronics → edge computing → data → web application → agricultural intelligence**

This end-to-end integration is the primary engineering focus of the project.

## Intellectual Property

The underlying technology is being developed as intellectual property and is currently **under patent protection / patenting process**.

For that reason, this repository intentionally does **not** contain:

- Source code
- ESP32 firmware
- PCB design files
- Detailed schematics
- Gerber files
- Proprietary algorithms
- Detailed electrical design
- Proprietary communications implementation
- Production documentation

The repository exists to document the project at an architectural and engineering level while protecting the underlying implementation.

## What Can Be Demonstrated

Although the implementation is proprietary, the project can be demonstrated through:

- Photographs of the physical device
- Photographs of the custom PCB
- Photographs of the sensing setup
- Web application screenshots
- Architecture diagrams
- System demonstrations
- Non-confidential performance information
- High-level technical explanations

## Engineering Domains

**IoT** — Connected physical sensing and monitoring  
**Embedded Systems** — ESP32-based device development  
**Instrumentation** — Soil sensing and measurement  
**Electronics** — Custom PCB and hardware integration  
**Edge Computing** — Raspberry Pi gateway architecture  
**Data Systems** — Collection, processing and visualization  
**Web Engineering** — Agricultural monitoring application  
**Remote Sensing** — Satellite data integration  
**Agricultural Technology** — Farm-level soil and fertility intelligence

## Project Development

The project was developed as a practical field-oriented system rather than as a purely theoretical prototype.

```text
Agricultural Problem
        ↓
System Concept
        ↓
Sensor Selection
        ↓
Embedded Device
        ↓
Custom PCB
        ↓
Edge/Gateway System
        ↓
Web Application
        ↓
Satellite Integration
        ↓
Field-Oriented System
```

## Portfolio Context

This project represents my broader engineering approach of connecting **instrumentation, embedded systems, electrical hardware, software and operational requirements** into an integrated working system.

It complements my professional experience in:

- Industrial automation
- PLC systems
- Instrumentation
- Sensor integration
- Embedded controls
- IoT
- Electrical systems
- Data acquisition
- Connected monitoring
- Field deployment
- System troubleshooting

**John Muturi Miano**  
Instrumentation & Control · Industrial Automation · IoT · Embedded Systems

[GitHub Profile](https://github.com/miano-dev)
