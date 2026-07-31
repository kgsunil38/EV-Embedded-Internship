# Embedded EV & Battery Management Project - Abeyaantrix Edusoft LLP

## Project Overview
This repository contains the firmware configurations, control logic, and battery simulation models developed during my VTU-affiliated Embedded EV engineering internship at Abeyaantrix Edusoft LLP. The project focuses on real-time embedded systems application in Electric Vehicle (EV) subsystems, specifically targeting Battery Management Systems (BMS) and motor controllers.

## Core Modules & Technical Details

### 1. Battery Module Design & C-Rate Calculation
* Designed custom battery modules optimizing cell configurations via **Series connections** (for voltage scaling) and **Parallel connections** (for current capacity scaling in Ah).
* Implemented mathematical firmware logic for real-time **C-Rate monitoring** using the standardized formula:  
  `C-Rate = Charge/Discharge Current (A) / Battery Capacity (Ah)`
* Implemented threshold protections to prevent high C-rate degradation factors like lithium plating, internal impedance escalation, and thermal runaway.

### 2. Embedded Control & Subsystem Interfacing
* Developed firmware utilizing **Arduino IDE (C/C++ environment)** to establish sensory data streams.
* Configured Analog-to-Digital Converter (**ADC**) processing pipelines utilizing precise Sample and Hold (S/H) timing circuits alongside Quantizing & Encoding maps to process analog temperature and voltage sensor data.
* Engineered core microcontroller algorithms managing **Pulse Width Modulation (PWM)** sequences via dedicated driver IC hardware for stable speed and direction regulation of DC/BLDC electric motors.
* Built automated relay control switching systems to handle safe load isolation between high-power AC/DC circuits and low-voltage digital microcontrollers.

## Technical Stack
* **Microcontrollers & Hardware Platforms:** Arduino Uno (ATmega328P), Embedded EV development architectures
* **Core Languages:** Embedded C, Simplified C++
* **Key Protocols & Hardware Modules:** ADC (S/H & Quantization), PWM, SPDT Relays, L293D Motor Drivers, 16x2 LCD, Infrared Sensors

