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

## System Workflow

**Scheduled Operation**
```text
RTC Module Tracks Time
        ↓
Arduino Checks Schedule
        ↓
Correct Medicine Slot Activated
        ↓
LED Indicator Turns On
```

**User Interaction Workflow**
```text
User Approaches Device
        ↓
Ultrasonic Sensor Detects Presence
        ↓
Arduino Triggers Servo Motor
        ↓
Medicine Compartment Opens
```

**Notification Workflow**
```text
Scheduled Medicine Time
        ↓
GSM Module Sends SMS Reminder
        ↓
User Receives Notification
```
---

## System Startup
After powering the system:
- RTC module initializes schedule
- LEDs indicate current active compartment
- GSM module initializes communication
- Ultrasonic sensor waits for user interaction

---

## Diagrams

<img width="1280" height="960" alt="WhatsApp Image 2026-04-23 at 3 39 42 PM" src="https://github.com/user-attachments/assets/f1803ea1-ab9a-4a9b-8cc2-c609eba3a52d" />

<img width="1280" height="960" alt="WhatsApp Image 2026-04-23 at 3 39 34 PM" src="https://github.com/user-attachments/assets/a38e7632-8c94-4567-8bd2-e4c3dcc79d92" />

<img width="1280" height="960" alt="WhatsApp Image 2026-04-23 at 3 39 30 PM" src="https://github.com/user-attachments/assets/9b89b569-0312-4d02-80e4-5ba77f7a7927" />

<img width="960" height="1280" alt="WhatsApp Image 2026-04-23 at 3 39 16 PM" src="https://github.com/user-attachments/assets/68735ca7-5eec-4ab7-a474-b22864922dfe" />

 
*RTC module tracks time. ESP32 (Arduino Uno) controls LEDs to indicate compartments. Ultrasonic sensor detects user, triggering servo to open the correct compartment. GSM module sends reminders.*
 
*RTC module communicates via I2C. LEDs connected through resistors indicate active compartment. Ultrasonic sensor connects to digital pins. Servo motors open lids when user approaches. GSM module connected via UART.*

---

## Potential Applications
- Elderly healthcare assistance
- Home medication automation
- Patient reminder systems
- Assistive healthcare devices
- IoT-based healthcare monitoring
- Smart healthcare prototypes

---
## Challenges Faced
During development, several technical challenges were encountered:
- Servo motor calibration for accurate lid movement
- False triggering from ultrasonic sensor noise
- GSM network latency during SMS delivery
- Limited battery backup duration
- Synchronization between RTC scheduling and actuator control

These challenges helped improve practical understanding of embedded systems integration and real-world hardware limitations. 

---

## Future Improvements
Planned future enhancements include:
- Mobile app integration
- Wi-Fi/Bluetooth connectivity
- Voice assistant support
- Rechargeable battery system
- Cloud-based medication tracking
- AI-based medicine scheduling
- Multi-user profile support
- Medicine intake logging system
- OLED/LCD status display

## Possible Advanced Extensions
Potential future research directions:
- Computer vision pill verification
- Smart health analytics
- Emergency caregiver notification system
- IoT healthcare dashboard
- AI-powered patient adherence prediction 

---

## Conclusion
The Smart Medicine Dispenser using Arduino Uno successfully automates medication reminders and dispensing based on time and user proximity. The project enhanced skills in sensor integration, actuator control, and IoT notifications. Despite challenges with sensor accuracy and prototype durability, the system effectively indicated and dispensed medicines, providing a reliable assistive healthcare solution.

---

## Working Video

WhatsApp Video 2026-04-23 at 3.39.30 PM.mp4

---

## Author
Abashesh Ranabhat

Computer Engineer | AI & Robotics Enthusiast | Embedded Systems Developer
- [GitHub] (https://github.com/Alpha107)
- [LinkedIn] (https://www.linkedin.com/in/abashesh-ranabhat/)

---

## Final Note
This project demonstrates the integration of:
- Embedded Systems
- Sensor-Based Automation
- IoT Communication
- Assistive Healthcare Technology

to create an automated medicine dispensing and reminder system aimed at improving healthcare accessibility and medication adherence.
