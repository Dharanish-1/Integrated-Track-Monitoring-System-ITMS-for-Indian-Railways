# Hardware

## Integrated Track Monitoring System (ITMS)

The hardware prototype is a mobile railway track monitoring platform designed to collect real-time information about railway track conditions using multiple sensors integrated with an ESP32-based control system.

The system combines sensor-based monitoring, wireless communication, and robotic mobility to enable contactless and intelligent railway track inspection.

## Hardware Prototype

![ITMS Hardware Prototype](images/prototype.jpg)

## Main Hardware Components

| Component | Purpose |
|---|---|
| ESP32 Development Board | Main controller and Wi-Fi communication |
| Ultrasonic Sensor | Distance and obstacle detection |
| ToF Distance Sensor | Precise short-range distance measurement |
| Vibration Sensor | Detection of abnormal vibrations |
| IMU Sensor | Monitoring tilt and motion |
| GPS Module | Location tracking |
| GSM Module | Communication and alert transmission |
| Motor Driver | Controls the DC motors |
| DC Gear Motors | Drives the robotic platform |
| Robot Chassis | Mechanical platform for the system |
| Camera Module | Captures railway track images |
| Battery Supply | Powers the complete system |

## Hardware Architecture

The ESP32 acts as the central controller of the monitoring system. It receives data from the connected sensors and processes the measurements before transmitting the information wirelessly to the monitoring dashboard.

```text
             ┌─────────────────────┐
             │      Sensors        │
             │                     │
             │ Ultrasonic          │
             │ ToF                 │
             │ Vibration           │
             │ IMU                 │
             │ GPS                 │
             └──────────┬──────────┘
                        │
                        ▼
             ┌─────────────────────┐
             │        ESP32        │
             │  Data Acquisition   │
             │  & Processing       │
             └──────────┬──────────┘
                        │ Wi-Fi
                        ▼
             ┌─────────────────────┐
             │ Flask Monitoring    │
             │     Dashboard       │
             └─────────────────────┘

             ┌─────────────────────┐
             │ Motor Driver        │
             └──────────┬──────────┘
                        │
                        ▼
             ┌─────────────────────┐
             │ DC Gear Motors      │
             │ + Robot Chassis     │
             └─────────────────────┘
Functional Modules
1. Sensing Module

The sensing module consists of multiple sensors for monitoring different physical parameters associated with railway track conditions.

2. Processing & Communication Module

The ESP32 collects sensor readings, processes the data, and transmits the information to the monitoring dashboard through Wi-Fi.

3. Mobility Module

The motor driver and DC gear motors provide movement for the robotic inspection platform.

4. Location & Communication

GPS provides location information, while the GSM module can be used for communication and alert transmission.

5. Vision Module

A camera is used to capture images of the railway track. The captured images can be processed using computer-vision techniques for detecting possible track abnormalities.

Power Supply

The complete prototype is powered using a battery supply capable of providing power to the ESP32, sensors, communication modules, and motor driver.

Hardware Workflow
Track
  ↓
Sensor & Camera Data
  ↓
ESP32
  ↓
Data Processing
  ↓
Wi-Fi Communication
  ↓
Flask Dashboard
  ↓
Real-Time Monitoring
Prototype

The prototype integrates the sensing, processing, communication, and mobility modules into a single robotic platform for railway track monitoring.

Future Hardware Improvements
Custom PCB integration
Improved power-management system
Industrial-grade sensors
Robust mechanical enclosure
Improved camera mounting
CAN-based communication
Battery monitoring and protection
Edge-AI processing for onboard anomaly detection
