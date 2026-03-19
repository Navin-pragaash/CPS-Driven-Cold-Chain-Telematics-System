# 📌 Industrial Cold Chain Monitoring System  

## 📖 Overview  
This project implements a real-time embedded system to monitor and maintain temperature conditions in industrial cold chain environments.  
Using an ESP32-S3 and thermoelectric cooling (Peltier module), the system ensures reliable temperature regulation with continuous feedback and cloud-based monitoring.

---

## 🎯 Objectives  
- Design a reliable embedded system for cold chain temperature control  
- Implement real-time data acquisition and feedback control  
- Ensure efficient hardware–software co-design  
- Maintain stable low-temperature conditions for sensitive storage  

---

## 🛠️ Tech Stack  

**Hardware:**  
- Microcontroller: ESP32-S3  
- Sensors/Modules: Temperature Sensor, Peltier Module, Heat Sink + Fan  

**Software:**  
- IDE: Arduino IDE  
- Languages: C 

---

## ⚙️ System Architecture  

The system continuously monitors temperature using sensors and dynamically controls the Peltier module to maintain the desired cooling range.

**Flow:**  
Temperature Sensor → ESP32-S3 → Control Algorithm → Peltier module and relay → Cooling Output → Cloud Monitoring  

![Architecture](images/architecture.png)

---

## 🚀 Features  
- Real-time temperature monitoring  
- Closed-loop temperature control using feedback  
- Multi-factor authentication (MFA) based cloud monitoring  
- Reliable and scalable embedded design  

---

## ▶️ Usage  
- Power the system  
- Monitor real-time temperature readings  
- Observe cooling response via Peltier module  
- Access cloud dashboard for remote monitoring  

---

## 📊 Results  
- Successfully maintains cold chain temperature conditions  
- Achieved stable cooling around **8°C**  
- Demonstrates consistent performance under controlled environment  

---

## 🔐 Future Improvements  
- End-to-end encrypted communication (TLS)  
- Advanced cloud dashboard with analytics  
- Power optimization for long-term deployment  
- AI-based predictive temperature control  

---

## 👥 Contributors  

This project was collaboratively developed by:  
- **Navin Pragaash G**  
- **Vignesh R**  
- **Badma Priya**  

---

## 📄 Research / Publication  

This work has been presented as a research paper and is currently under review for publication.

**Paper Title:** *"Industrial Cold Chain Monitoring using ESP32-S3 with Thermoelectric Cooling"*  
**Status:** Under Review / Submitted  
**Conference/Journal:** To be submitted  

*Note: Full paper will be linked once published.*

---

## 📜 License  
MIT License  

