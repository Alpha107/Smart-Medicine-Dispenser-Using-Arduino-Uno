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

## System Diagrams

### Block Diagram
![Block Diagram](images/block_diagram.png)  
*RTC module tracks time. ESP32 (Arduino Uno) controls LEDs to indicate compartments. Ultrasonic sensor detects user, triggering servo to open the correct compartment. GSM module sends reminders.*

### Circuit Diagram
![Circuit Diagram](images/circuit_diagram.png)  
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

## Images
*(Replace the placeholders with your actual images)*  
![Medicine Dispenser Front](images/medicine_dispenser_front.png)  
![Medicine Dispenser Top](images/medicine_dispenser_top.png)
