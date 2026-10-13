# Vigilix — Edge-AI Driver Vigilance and Risk Monitoring System

**Group 21 – Team Invictus**

## Introduction

Vigilix is a low-cost, retrofit driver safety and fleet monitoring system designed to detect driver drowsiness and distraction using Edge AI and computer vision. The system processes camera input locally on a Raspberry Pi to identify prolonged eye closure, head drooping, and sustained looking-away behaviour. When potential risks are detected, an ESP32 activates immediate alerts through a buzzer, vibration motor, or warning LEDs.

The system also incorporates contextual information, such as GPS-derived vehicle speed, to provide explainable driving-risk levels. A secure, multi-user web application enables drivers to review their trips and alerts, fleet managers to supervise multiple drivers and vehicles, and administrators to manage users, vehicles, devices, and access permissions.

Designed for transport operators, logistics companies, and other organizations operating vehicle fleets, Vigilix aims to improve driver safety through real-time warnings, event tracking, and centralized fleet supervision.

## Key Features

- **Edge AI:** Local computer vision processing for driver vigilance monitoring.
- **Drowsiness Detection:** Identification of prolonged eye closure and head drooping.
- **Distraction Detection:** Monitoring of sustained looking-away behaviour.
- **Real-Time Alerts:** Immediate warnings using a buzzer, vibration motor, and LEDs.
- **Contextual Risk Assessment:** Combines driver-state indicators with vehicle-speed information.
- **Fleet Supervision:** Monitoring of multiple drivers, vehicles, trips, and safety events.
- **Multi-User Web Application:** Dedicated interfaces for drivers, fleet managers, and administrators.
- **Offline Operation:** Local detection and alerts continue without an Internet connection.
- **Privacy-Focused Processing:** Facial video is processed locally rather than continuously uploaded.
- **Performance Evaluation:** Testing of detection accuracy, false alarms, response latency, and system reliability.

## System Architecture

The system integrates embedded hardware, edge computing, communication services, and a web-based monitoring platform.

- **Raspberry Pi:** Runs the computer vision pipeline, temporal analysis, and risk assessment engine.
- **ESP32:** Interfaces with contextual sensors and controls physical warning devices.
- **Camera and Sensors:** Capture driver behaviour and relevant contextual information.
- **Backend and Database:** Store user accounts, vehicle and device records, trips, alerts, and system health logs.
- **Web Application:** Provides role-based dashboards for drivers, fleet managers, and administrators.
- **Communication:** Uses MQTT or HTTP to transmit events and device-health information.

## Project Objectives

1. Develop a standalone Edge-AI driver vigilance monitoring prototype.
2. Provide timely local alerts for potential drowsiness and distraction.
3. Evaluate whether temporal analysis and contextual sensing can reduce false warnings.
4. Build a secure web application for multi-user fleet supervision.
5. Evaluate detection performance, alert latency, edge-device performance, and offline reliability.

## Target Users

- **Drivers:** Monitor their driving status, review trips, and receive safety alerts.
- **Fleet Managers:** Supervise multiple drivers and vehicles, review safety events, and identify potential risks.
- **Administrators:** Manage user accounts, permissions, vehicles, devices, and system logs.

## Technology Stack

- **Edge Computing:** Raspberry Pi, Raspberry Pi OS/Linux
- **Embedded Systems:** ESP32, sensors, buzzer, vibration motor, warning LEDs
- **AI and Computer Vision:** Python and suitable computer vision libraries
- **Communication:** MQTT or HTTP
- **Backend and Database:** To be finalized during implementation
- **Web Technologies:** To be finalized during implementation

## Expected Outcome

The project aims to deliver a working hardware prototype, a local driver-warning mechanism, a secure multi-user web application, an event database, and an experimental evaluation report. The system is intended as a driver-assistance and fleet-supervision solution and will not directly control the vehicle.

---

*Developed by Group 21 – Team Invictus as an Embedded Systems project at the University of Peradeniya.*
