Smart Energy Monitoring System using ESP32

A real-time energy monitoring system using ESP32, ACS712 Current Sensor, and ZMPT101B Voltage Sensor to measure AC Voltage, Current, and Power Consumption. The measured values are displayed on a 16x2 LCD with I2C interface, providing an efficient and low-cost solution for energy monitoring applications.

---

📌 Overview

The Smart Energy Monitoring System is an ESP32-based project designed to monitor electrical parameters in real time. The system acquires voltage and current data using dedicated sensors, processes the measurements through the ESP32 microcontroller, and displays the results on an LCD screen.

This project can be further extended with IoT platforms such as Blynk, ThingSpeak, or cloud services for remote monitoring and smart energy management.

---

🎯 Objectives

- Measure AC Voltage using ZMPT101B Voltage Sensor
- Measure AC Current using ACS712 Current Sensor
- Calculate Real-Time Power Consumption
- Display readings on a 16x2 LCD
- Develop a low-cost energy monitoring solution
- Provide a platform for future IoT integration

---

🛠 Hardware Components

Component| Quantity
ESP32 Development Board| 1
ACS712 Current Sensor| 1
ZMPT101B Voltage Sensor| 1
16x2 LCD Display| 1
I2C Module| 1
LED Bulb (Load)| 1
Breadboard| 1
Jumper Wires| As Required
AC Source / Inverter Output| 1

---

⚙️ Working Principle

The system continuously measures voltage and current from the connected AC load.

Step 1: Voltage Measurement

The ZMPT101B sensor measures the AC voltage and provides an analog output proportional to the input voltage.

Step 2: Current Measurement

The ACS712 sensor measures the current flowing through the load and generates an analog signal corresponding to the current value.

Step 3: Data Processing

The ESP32 reads the analog outputs of both sensors through its ADC pins and processes the values.

Step 4: Power Calculation

Power (W) = Voltage (V) × Current (A)

Step 5: Display Output

The calculated Voltage, Current, and Power values are displayed on the LCD screen in real time.

---

🔌 Circuit Connections

ACS712 → ESP32

ACS712 Pin| ESP32 Pin
VCC| 5V
GND| GND
OUT| GPIO35

ZMPT101B → ESP32

ZMPT101B Pin| ESP32 Pin
VCC| 3.3V
GND| GND
OUT| GPIO34

LCD (I2C) → ESP32

LCD Pin| ESP32 Pin
VCC| 5V
GND| GND
SDA| GPIO21
SCL| GPIO22

---

🏗 System Architecture

AC Source / Inverter Output
            │
            ▼
      ACS712 Sensor
            │
            ▼
         LED Bulb

AC Source ─────────► ZMPT101B

ACS712 + ZMPT101B
            │
            ▼
          ESP32
            │
            ▼
      LCD Display

---

📊 Sample Output

Voltage : 230 V
Current : 0.15 A
Power   : 34.5 W

The LCD continuously updates the measured values, allowing users to monitor energy consumption in real time.

---

✨ Features

- Real-Time Voltage Monitoring
- Real-Time Current Monitoring
- Power Calculation
- LCD Display Interface
- ESP32-Based Processing
- Low-Cost and Compact Design
- Easy Integration with IoT Platforms
- Suitable for Academic Projects and Research

---

🌍 Applications

- Smart Energy Meter
- Home Energy Monitoring
- Industrial Load Monitoring
- Renewable Energy Monitoring
- Energy Consumption Analysis
- IoT-Based Monitoring Systems
- Academic Mini Projects
- Electrical Laboratory Experiments

---

🔮 Future Scope

- Blynk Cloud Integration
- ThingSpeak Dashboard Monitoring
- Mobile Application Support
- Cloud Data Logging
- Overload and Fault Detection
- Energy Billing System
- Power Factor Measurement
- Historical Data Analysis
- Smart Home Integration

---

📸 Project Setup

The project consists of:

- ESP32 Development Board
- ACS712 Current Sensor
- ZMPT101B Voltage Sensor
- LCD Display Module
- AC Load (Bulb)
- Inverter/AC Supply

These components work together to provide real-time monitoring of electrical parameters.

---

👩‍💻 Authors

- Prathika 
- Prathiksha 
- priyanka

---

📜 License

This project is developed for educational, academic, and research purposes. Feel free to use, modify, and extend it for learning and innovation.

---

⭐ If you found this project useful, consider giving it a star on GitHub!
