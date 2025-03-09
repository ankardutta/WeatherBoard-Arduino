# 🌦️ IoT Weather Monitoring & Display System 🌡️ [Batch 2021-2024]

[![Arduino](https://img.shields.io/badge/Arduino-00979D?style=for-the-badge&logo=Arduino&logoColor=white)](https://www.arduino.cc/)
[![IoT](https://img.shields.io/badge/IoT-FF6F00?style=for-the-badge&logo=iot&logoColor=white)](https://iot.eclipse.org/)
[![Weather](https://img.shields.io/badge/Weather_Monitoring-4A90E2?style=for-the-badge)](https://en.wikipedia.org/wiki/Weather_station)

As a faculty member of the Computer Science and Technology (CST) department, I had the privilege of serving as the project coordinator for "Weather Display Board in College Campus". This innovative project aimed to 

i) Design and develop an interactive display board 

ii) Showcases real-time weather updates, providing students, faculty, and staff with a convenient and accessible means of staying informed about current weather conditions on campus.

A real-time weather monitoring system with LED display capabilities using IoT components.

![System Overview](media/system-overview.jpg) 

## 🛠️ Hardware Components
| Component              | Quantity | Image                      |
|------------------------|----------|----------------------------|
| Arduino Uno            | 1        | ![Arduino](Media/arduino.jpg) |
| DHT22 Sensor           | 1        | ![DHT22](Media/dht22.jpg)    |
| P10 LED Module (DMD)   | 16        | ![P10](Media/p10-led.jpg)    |
| RTC Module             | 1        | ![RTC](Media/rtc.jpg)        |
| SMPS 16A               | 1        | ![SMPS](Media/smps.jpg)      |


## 💻 Software Used
![Arduino IDE](https://img.shields.io/badge/Arduino_IDE-00979D?style=for-the-flat&logo=arduino&logoColor=white)
![DMD Library](https://img.shields.io/badge/DMD_Library-FF6F00?style=for-the-flat)

## 📋 System Process Flow
```mermaid
graph TD
    A[Power On] --> B[RTC Initialization]
    B --> C[DHT22 Sensor Read]
    C --> D[Data Processing]
    D --> E[P10 LED Display]
    E --> F[Repeat Every 1 Minutes]
```
### 🎥 Demo Video
1. https://github.com/user-attachments/assets/82dcd58c-07ed-447a-b3dd-98a2bfbe6d50

2. https://github.com/user-attachments/assets/d4ce427b-b08d-433d-99a2-e957efd91fe5

### 🔌 Wiring Diagram

Final Circuit Images: ![circuit](https://github.com/user-attachments/assets/47e6dd71-d5b8-4a99-b18e-b3fad5955c5e)

Component	Arduino Pin	Color Code

DHT22 Data	D2	🟢 Green

RTC SCL	A5	🔵 Blue

RTC SDA	A4	🟡 Yellow

P10 CLK	D13	🔴 Red

P10 DATA	D11	⚪ White
