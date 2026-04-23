# Smart Medicine Dispenser Using Arduino Uno

An automated medicine dispenser that opens compartments based on time and proximity, with notifications sent via GSM. This project demonstrates automation, IoT, and assistive technology.

---

## Introduction
The Smart Medicine Dispenser is designed to help users take medicines on time, reducing missed doses. The system consists of a box with three compartments for **morning, day, and night doses**. An RTC module tracks the current time and controls LEDs to indicate the active compartment. When a user approaches, an ultrasonic sensor detects their presence, triggering servo motors to open the compartment lid. Additionally, a GSM module sends notifications to remind users.

This project combines automation, human-machine interaction, and IoT-based alerts, making it useful for elderly or medically-dependent users. It also provides experience in sensor integration, actuator control, and time-based automation.

---

## Components Used

| Component | Description | Purpose |
|-----------|------------|--------|
| Arduino Uno | ATmega328P microcontroller | Main controller |
| Servo Motors | Micro servos (SG90) | Open compartment lids |
| Ultrasonic Sensor | HC-SR04 | Detect user proximity |
| RTC Module | DS3231 / DS1307 | Track real-time and schedule medicine |
| GSM Module | SIM800 / SIM900 | Sends SMS reminders |
| LEDs | Indicator lights | Show active compartment |
| Resistors | Various values | Current limiting for LEDs |
| Jumper Wires | Electrical connections | Circuit wiring |
| Batteries & Holders | Power supply | System power |
| Cardboard / Prototype Box | 3-compartment medicine box | Physical structure |

---

## Diagrams

<img width="1280" height="960" alt="WhatsApp Image 2026-04-23 at 3 39 42 PM" src="https://github.com/user-attachments/assets/f1803ea1-ab9a-4a9b-8cc2-c609eba3a52d" />

<img width="1280" height="960" alt="WhatsApp Image 2026-04-23 at 3 39 34 PM" src="https://github.com/user-attachments/assets/a38e7632-8c94-4567-8bd2-e4c3dcc79d92" />

<img width="1280" height="960" alt="WhatsApp Image 2026-04-23 at 3 39 30 PM" src="https://github.com/user-attachments/assets/9b89b569-0312-4d02-80e4-5ba77f7a7927" />

<img width="960" height="1280" alt="WhatsApp Image 2026-04-23 at 3 39 16 PM" src="https://github.com/user-attachments/assets/68735ca7-5eec-4ab7-a474-b22864922dfe" />

 
*RTC module tracks time. ESP32 (Arduino Uno) controls LEDs to indicate compartments. Ultrasonic sensor detects user, triggering servo to open the correct compartment. GSM module sends reminders.*
 
*RTC module communicates via I2C. LEDs connected through resistors indicate active compartment. Ultrasonic sensor connects to digital pins. Servo motors open lids when user approaches. GSM module connected via UART.*

---

## Problems Faced
- Coordinating RTC timing with LED indicators and servo actuation  
- Ultrasonic sensor false detections  
- Servo calibration to open cardboard lids accurately  
- GSM network delays causing late notifications  
- Limited battery life for continuous operation  

---

## Future Improvements
- Use a stronger, durable box instead of cardboard  
- Wi-Fi or mobile app notifications for smarter monitoring  
- Multi-user support for family schedules  
- Voice alerts or buzzer for additional reminders  
- Rechargeable or solar-powered battery system  
- Logging of medicine intake for medical records  

---

## Conclusion
The Smart Medicine Dispenser using Arduino Uno successfully automates medication reminders and dispensing based on time and user proximity. The project enhanced skills in sensor integration, actuator control, and IoT notifications. Despite challenges with sensor accuracy and prototype durability, the system effectively indicated and dispensed medicines, providing a reliable assistive healthcare solution.

---

## Working Video

WhatsApp Video 2026-04-23 at 3.39.30 PM.mp4
