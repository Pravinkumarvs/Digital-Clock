# ⏰ Digital Clock Using Discrete ICs

A hardware-based **Digital Clock** built using discrete ICs without a microcontroller.

---

## 📌 Overview

A digital clock designed entirely using digital electronics. The project demonstrates the fundamentals of **counters, clock division, sequential logic, and seven-segment display interfacing** without relying on programmable devices such as Arduino or ESP32.

The clock displays time in **24-hour format (HH:MM:SS)** and includes **AM/PM indication using LEDs**.

This project is intended for educational purposes to strengthen understanding of **Digital Electronics and Hardware Design**.

---

## ✨ Features

- 24-hour time format
- Hours, minutes, and seconds display
- Breadboard prototype
- Expandable to PCB design
- No microcontroller required

---

## 🛠️ Hardware Used

### ICs

- CMOS CD4026BE
- NE555 Timer
- Logic Gates

### Displays

- Common Cathode 7-Segment Displays

### Passive Components

- Resistors
- Capacitors
- Push Buttons
- LEDs

### Power

- 5V Regulated Supply

---

## ⚙️ Working Principle

- A clock pulse is generated using the **NE555 Timer IC**.
- The pulse is converted into a precise **1 Hz signal**.
- **CD4026BE ICs** count the pulses and provide seven-segment display drive signals.
- Counter carry outputs are cascaded to the next digit.
- Logic gates are used to reset the counters at appropriate values:
  - Seconds: `59 → 00`
  - Minutes: `59 → 00`
  - Hours: `23 → 00`

---

## 📂 Repository Structure

```text
Digital_clock/
│
├── docs/
│   ├── BlockDiagram.png
│   ├── BreadboardLayout.png
│   └── ProjectReport.pdf
│
├── Schematic/
│   └──
│
├── images/
│   └── FinalClock.jpg
│
├── README.md
└── LICENSE
