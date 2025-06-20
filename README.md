# 🚦 Finite State Machine-Based Traffic Signal Controller

## 📌 Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [System Architecture](#system-architecture)
- [Hardware Requirements](#hardware-requirements)
- [Pin Configuration](#pin-configuration)
- [State Transitions (Finite State Machine)](#state-transitionsfinite-state-machine)
- [Testing & Validation](#testing--validation)
- [Future Enhancements](#future-enhancements)
- [Published Paper](#-published-paper)
- [Team Members (Amrita School of Computing, Bengaluru)](#team-members-amrita-school-of-computing-bengaluru)
- [Mentor](#-mentor)
- [Acknowledgment](#-acknowledgment)


## Overview

This project implements a **Finite State Machine (FSM)-based Traffic Signal Controller** to efficiently manage traffic at a two-way intersection with integrated pedestrian support. Developed using **Arduino Uno** and simulated on **Tinkercad**, the system mimics real-world urban traffic behavior, incorporating both vehicle detection and pedestrian-initiated crossing sequences. The FSM logic ensures systematic and responsive transitions between traffic light states, enhancing traffic flow and pedestrian safety in a smart, cost-effective manner.

## Features

- **Dynamic Traffic Signal Control**: Manages main road and side road signals using FSM logic for predictable and coordinated switching.  
- **Pedestrian Assistance**: Enables safe crossing via push-button requests that trigger a dedicated pedestrian light sequence.  
- **Configurable Crossing Duration**: Crossing time is adjustable using a potentiometer, allowing flexibility between 1–10 seconds.  
- **Vehicle Detection Simulation**: Potentiometers emulate real-world induction coils to detect waiting vehicles on the side road.  
- **Real-Time Feedback**: Serial Monitor integration provides live system updates for debugging and status visualization.  
- **Tinkercad Simulation**: Entire hardware logic is digitally simulated, enabling testing without physical components.


## Technologies Used

* **Platform**: Arduino Uno (C++)
* **Simulation Tool**: Tinkercad Circuits by Autodesk
* **Hardware Simulation**: Potentiometers for vehicle detection, push buttons for pedestrian requests
* **Components**: LEDs, Push Buttons, Potentiometers, Breadboard, Serial Monitor

## System Architecture

```
┌──────────────┐    ┌─────────────────┐    ┌──────────────┐
│ Main Road TL │───▶ Pedestrian Ctrl │───▶ Side Road TL │
└──────────────┘    └─────────────────┘    └──────────────┘
```
## Hardware Requirements 
![image](https://github.com/user-attachments/assets/fed9f4f8-ccf5-4790-9ccc-017da26942d7)



## Pin Configuration

| Pin | Component | Function |
|-----|-----------|----------|
| **Digital Pins** |
| D3 | Main Road Green LED | Traffic signal output |
| D4 | Main Road Yellow LED | Traffic signal output |
| D5 | Main Road Red LED | Traffic signal output |
| D6 | Pedestrian Green LED | Crossing signal output |
| D7 | Pedestrian Red LED | Crossing signal output |
| D8 | Side Road Green LED | Traffic signal output |
| D9 | Side Road Yellow LED | Traffic signal output |
| D10 | Side Road Red LED | Traffic signal output |
| D11 | Push Button 1 | Pedestrian request input |
| D12 | Push Button 2 | Pedestrian request input |
| **Analog Pins** |
| A0 | Vehicle Detection Pot | Simulates induction coil |
| A1 | Pedestrian Timer Pot | Controls crossing duration |

### State Transitions(Finite State Machine) 

![image](https://github.com/user-attachments/assets/7419986a-ea16-4d8d-87ba-83bb062299aa)

## Testing & Validation

* ✅ Pedestrian push buttons
* ✅ Potentiometer-controlled crossing time
* ✅ FSM logic verification
* ✅ Serial output confirmation

> 🧪 All hardware and logic tests were validated using the Tinkercad simulation platform, ensuring accurate digital representation of the Arduino circuit and logic states.

## Future Enhancements

* [ ] IR-based vehicle detection
* [ ] Sound/buzzer alerts
* [ ] LCD countdown timer
* [ ] Smart city integration

## 📄 Published Paper

**Title:** Modelling and Design of a Finite State Machine-Based Traffic Signal Controller for Efficient Urban Traffic Management

**Authors:** Kandibanda Lohith, Mudumala Varnika Narayani, Naga Ruthvika Durupudi, Nunnaguppala Rohit, Niharika Panda

**Publication:** 2nd International Conference on Artificial Intelligence, Computing Technologies, Internet of Things (IoT) and Data Analytics (AICTA 2024)
**Conference Date:** 15–17 November 2024
**Conference Location:** NIT Raipur, India (Hybrid Mode)

**Publisher:** Springer – Lecture Notes in Networks and Systems (LNNS) Serie

## Team Members (Amrita School of Computing, Bengaluru)

*B.Tech CSE, Batch of 2022–2026*
**Amrita School of Computing, Bengaluru**
**Amrita Vishwa Vidyapeetham, India**

* **Naga Ruthvika Durupudi**
* **Kandibanda Lohith**
* **Mudumala Varnika Narayani**
* **Nunnaguppala Rohit**

## 🎓 Mentor

* **Ms. Niharika Panda**
  Lecturer
  Department of Computer Science and Engineering
  Amrita School of Computing, Bengaluru
  Amrita Vishwa Vidyapeetham, India

## 🙏 Acknowledgment

This project was developed as part of the academic curriculum for the **B.Tech CSE Batch of 2022–2026** under the mentorship of **Ms. Niharika Panda**, Amrita School of Computing, Amrita Vishwa Vidyapeetham, Bengaluru campus.

---

> 📚 Developed as part of the academic curriculum at **Amrita School of Computing, Bengaluru**
