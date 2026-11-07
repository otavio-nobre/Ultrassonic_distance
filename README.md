# ESP32 Distance and Proximity Alert System

An embedded IoT project built with ESP32 and HC-SR04 Ultrasonic Sensor that provides real-time distance measurements and visually indicates object proximity using LED indicators.

---

## Features

- **Ultrasonic Distance Measurement:** Uses HC-SR04 to measure distance in centimeters via time-of-flight calculation.
- **Visual Alert Indicators:** 
  - **Green LED:** Indicates target object is at a safe distance (> 5 cm).
  - **Red LED:** Indicates target object is within the critical alert zone (≤ 5 cm).
- **Serial Monitoring:** Real-time distance updates streamed over 115200 baud serial connection.

---

## Demo and Hardware Preview

### Hardware Setup and States

| Object Detection (Dist <= 5 cm) | Safe Distance (Dist > 5 cm) |
| :---: | :---: |
| ![Red LED Active](assets/WhatsApp%20Image%202026-11-06%20at%2021.31.52.jpeg) | ![Green LED Active](assets/WhatsApp%20Image%202026-11-06%20at%2021.33.52.jpeg) |
| *Red LED active when an object is detected near the sensor* | *Green LED active when path is clear* |

---

## Hardware Requirements

- **ESP32 Development Board**
- **HC-SR04 Ultrasonic Distance Sensor**
- **1x Red LED**
- **1x Green LED**
- **2x Resistors (220Ω / 330Ω)**
- **Breadboard and Jumper Wires**
- **USB Data Cable**

---

## Circuit Pinout

| Component | ESP32 Pin |
| :--- | :--- |
| **HC-SR04 VCC** | 5V / VIN |
| **HC-SR04 GND** | GND |
| **HC-SR04 TRIG** | GPIO 14 |
| **HC-SR04 ECHO** | GPIO 27 |
| **Red LED** | GPIO 13 |
| **Green LED** | GPIO 12 |

---

## Getting Started

### Prerequisites

1. Install [Arduino IDE](https://www.arduino.cc/en/software).
2. Install the **ESP32 Board Package** by Espressif in the Board Manager.

### Installation and Flashing

1. Clone this repository:
   ```bash
   git clone [https://github.com/otavio-nobre/Ultrasonic-distance.git](https://github.com/otavio-nobre/Ultrasonic-distance.git)
