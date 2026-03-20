# CPS-Driven-Cold-Chain-Telematics-System   


![ESP32-S3](https://img.shields.io/badge/Hardware-ESP32--S3-red)
![Arduino](https://img.shields.io/badge/Firmware-Arduino-green)
![ThingSpeak](https://img.shields.io/badge/Cloud-ThingSpeak-yellow)
![GPS](https://img.shields.io/badge/Tracking-GPS-green)
![Flask](https://img.shields.io/badge/Backend-Flask-black)
![CPS](https://img.shields.io/badge/System-CPS-critical)
![Telematics](https://img.shields.io/badge/System-Telematics-informational)

# Project Overview  
This project implements a real-time Cyber physical system to monitor and maintain temperature conditions in industrial cold chain environments.  
Using an ESP32-S3 and thermoelectric cooling (Peltier module), the system ensures reliable temperature regulation with continuous feedback and cloud-based monitoring.

---

# Objectives  
- Design a reliable embedded system for cold chain temperature monitoring and feedback control.  
- Maintain stable low-temperature conditions for sensitive storage.

---

# Tech Stack  

**Hardware:**  
- Microcontroller: ESP32-S3  
- Sensors/Modules: TMP102 Sensor, (Peltier Module + Heat Sink + Fan), (2V, 6A) Power Source, NEO-6M, (15cmx15cmx20cm) Box setup.

**Software:**  
- IDE: Arduino IDE  
- Languages: C 

---

# Embedded Control Module (ESP32-S3)

Responsible for:

- Sensor data acquisition (temperature & geolocation)
- Closed-loop thermal control using Peltier-based actuation
- Cloud telemetry integration for real-time monitoring
- Local web server for dynamic threshold configuration

--

# System Architecture  

The system continuously monitors temperature using sensors and dynamically controls the Peltier module to maintain the desired cooling range.

**Flow:**  
Example architecture:

```
Temperature Sensor (TMP102)
Pressure / Control Inputs
GPS Module
   │
   ▼
ESP32 (Embedded Controller)
   │
   ├── Temperature Monitoring & Feedback Control (Peltier + Fan + Heatsink)
   ├── Threshold Management (User-defined Range)
   ├── Data Processing & Decision Logic
   │
   ▼
WiFi Communication (ESP32)
   │
   ├── ThingSpeak Cloud Dashboard (Real-time Monitoring)
   ├── Email Alert System (Threshold Breach Notification)
   │
   ▼
Flask Backend (Localhost Server)
   │
   ├── Multi-Factor Authentication (OTP via Email)
   ├── User Interface (Set Temperature Range)
   └── Secure Access Control
   │
   ▼
User / Operator
   │
   ├── Monitor Temperature & Location
   ├── Set Threshold Values
   └── Receive Alerts
```

---

# Features  
- Real-time temperature, location monitoring  
- Closed-loop temperature control using feedback  
- Multi-factor authentication (MFA) based cloud monitoring  
- Reliable and scalable embedded design  

---

# Results  
- Successfully maintains cold chain temperature conditions  
- Achieved stable cooling around **8°C**  
- Demonstrates consistent performance under controlled environment  

---

# Future Improvements  
- End-to-end encrypted communication (TLS)  
- Advanced cloud dashboard with analytics  
- Power optimization for long-term deployment  
- AI-based predictive temperature control  

---

# Contributors  

This project was collaboratively developed by:  
- **Navin Pragaash G**  
- **Vignesh R**  
- **Badma Priya**  

---

# Research / Publication  

This work has been presented as a research paper and is currently under review for publication.

**Paper Title:** *"Industrial Cold Chain: A Tracking System With Temperature Maintenance"*  
**Status:** Under Review / Submitted  
**Conference/Journal:** To be submitted  

*Note: Full paper will be linked once published.*

---

# License  
MIT License  

# Acknowledgements
- Python Community 
- ESP32 Development Community  
- Matlab Central (Community) 

---
