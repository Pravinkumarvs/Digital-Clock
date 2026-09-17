A hardware-based Digital Clock built using discrete ICs without a microcontroller.

📌 Overview
A digital clock designed entirely using digital electronics. The project demonstrates the fundamentals of counters, clock division, sequential logic, and seven-segment display interfacing without relying on programmable devices such as Arduino or ESP32.

The clock displays time in 24-hour format (HH:MM:SS) and includes AM/PM indication using LEDs.

This project is intended for educational purposes to strengthen understanding of Digital Electronics and Hardware Design.

✨ Features
24-Hour Time Format
Hours, Minutes, and Seconds Display
Breadboard Prototype
Expandable to PCB Design
No Microcontroller Required
🛠 Hardware Used
ICs
CMOS CD4026BE
NE555 Timer
Logic Gates
Displays
Common Cathode 7-Segment Displays
Passive Components
Resistors
Capacitors
Push Buttons
LEDs
Power
5V Regulated Supply
⚙️ Working Principle
A clock pulse is generated using an Timer 555 IC.
The pulse is converted into a precise 1 Hz signal.
CD4026BE ICs count the pulses and converts BCD to a seven-segment display signals.
Counter carry outputs cascade into the next digit.
Logic resets counters at appropriate values:
Seconds: 59 → 00
Minutes: 59 → 00
Hours: 23 → 00
📂 Repository Structure
Digital_clock/
│
├── docs/
│   ├── BlockDiagram.png
│   ├── BreadboardLayout.png
│   └── ProjectReport.pdf
│
├── Schematic/
│
│
├── images/
│   ├── FinalClock.jpg
│
├── README.md
└── LICENSE
🚀 Project Status
Current Stage:

 Project Planning
 Component Selection
 Schematic Design
 Breadboard Prototype
 Functional Testing
 Final Documentation
📚 Concepts Used
Digital Electronics
Sequential Logic
Decade Counters
Frequency Division
Seven-Segment Displays
Clock Generation
Reset Logic
Cascaded Counters
Teammates :
PRAVINKUMAR VS
MAHITHA S
🎯 Future Improvements
Alarm Function
Stopwatch Mode
Date Display
--

📜 License
This project is released for educational and learning purposes.
