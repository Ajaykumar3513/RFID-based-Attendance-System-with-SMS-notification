# RFID-Based Attendance System with SMS Notification

## Project Overview

This project implements an **RFID-based attendance system** that automates the process of tracking attendance for students or employees. Each individual uses an RFID card to mark their presence, and the system sends an instant SMS notification to a predefined number, such as a parent or supervisor, ensuring real-time updates. This project improves attendance monitoring efficiency and provides a reliable, automated method for real-time tracking.

## Features
- **Automated Attendance Logging**: Individuals use RFID cards to log their attendance instantly.
- **SMS Notification**: Sends real-time SMS notifications to a predefined number (parent, supervisor, etc.) upon attendance registration.
- **Real-time Monitoring**: The system provides a quick and efficient way to monitor attendance records.

## Components Used
- **RFID Reader (RC522)**: Reads the RFID cards used by individuals.
- **RFID Tags/Cards**: Unique cards assigned to each individual for attendance marking.
- **Arduino Uno**: The microcontroller used to control the system.
- **GSM Module (SIM800L)**: Responsible for sending SMS notifications.
- **LCD Display (Optional)**: Displays attendance status and confirmation messages.
- **Buzzer (Optional)**: Signals successful or unsuccessful attendance logging.
- **Breadboard and Jumper Wires**: For wiring components together.
- **Power Supply**: 5V DC power supply for Arduino and other components.

## How It Works
1. **RFID Card Scanning**: Individuals scan their RFID card using the RFID reader.
2. **Attendance Logging**: The RFID card's unique ID is processed by the Arduino, and the system logs the attendance.
3. **SMS Notification**: Upon successful attendance marking, the GSM module sends an SMS notification to a predefined mobile number, informing them of the individual's attendance.
4. **Display Feedback**: Optionally, the system can display confirmation on an LCD screen or signal success with a buzzer.

## System Flow
1. RFID card is scanned.
2. Arduino processes the card's unique ID.
3. If the card is valid:
   - Attendance is logged.
   - SMS is sent via GSM module to the predefined number.
4. If the card is invalid:
   - The system alerts the user via the LCD display or buzzer.


## Customization
- Modify the **predefined mobile number** in the code to the actual number where you want to send the SMS notification.
- You can add or remove **RFID cards** in the system by modifying the `registeredCard` variable in the code.

## Applications
- Schools and universities for student attendance tracking.
- Offices and workplaces for employee attendance management.
- Restricted areas where access is controlled via RFID cards.

## Future Enhancements
- Integrate a **database** to store attendance logs for future reference.
- Implement a **web-based interface** for real-time attendance monitoring.
- Expand the system to support multiple RFID readers.

## Project Cost (Approximate)
| Component            | Price (INR) |
|----------------------|-------------|
| Arduino Uno          | ₹500        |
| RFID Reader (RC522)  | ₹250        |
| GSM Module (SIM800L) | ₹450        |
| LCD Display          | ₹150        |
| Buzzer               | ₹20         |
| Jumper Wires         | ₹50         |
| Total Cost           | ₹1420       |
