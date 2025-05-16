# 🕒 Embedded Systems Final Project – CSE211s Spring 2025

**Course**: CSE211s – Introduction to Embedded Systems  
**Institution**: Faculty of Engineering, Ain Shams University  
**Department**: Mechatronics  
**Platform**: STM32 NUCLEO-F401RE + Arduino Multifunction Shield  
**Submitted**: Spring 2025

## 📌 Project Overview

This project demonstrates the use of an STM32 NUCLEO-F401RE development board in conjunction with an Arduino Multifunction Shield to implement a **Real-Time Clock (RTC)** and **Analog Voltage Display** system.

The design showcases embedded systems principles, using on-chip peripherals like ADC and timers, as well as interfacing with input switches and a 7-segment display.

---

## 🚀 Features

### 1. Real-Time Clock (RTC)
- Upon power-up or reset, the 7-segment display starts counting from 00:00 (MM:SS).
- The two least significant digits show **seconds**, and the two higher digits show **minutes**.
- Pressing **Switch S1** at any time resets the time to zero (00:00).

### 2. Analog Voltage Display
- The on-board potentiometer provides a variable voltage signal.
- Pressing **Switch S3**:
  - Temporarily switches the 7-segment display to show the **current input voltage** (in volts).
  - The RTC continues running in the background.
- Releasing **Switch S3** returns the display to showing the elapsed time.

---

## 🧰 Hardware Used

- **STM32 NUCLEO-F401RE**
- **Arduino Multifunction Shield**
  - 7-Segment Display
  - On-board Potentiometer
  - Switches S1 and S3

---

## 🛠️ Software Structure

### 📂 Project Files
- `main.c`: Main application logic
- `startup_stm32f401xe.s`: Startup code and vector table
- `isr_handlers.c/h`: Interrupt Service Routines (ISRs)
- `adc.c/h`: ADC initialization and voltage reading
- `rtc.c/h`: Timer-based real-time clock logic
- `display.c/h`: Interface for 7-segment display control
- `switch.c/h`: Switch input handling (S1 and S3)

> All code is thoroughly commented for readability and maintainability.

---

## 📽️ Deliverables

1. ✅ **Video Demo** of the working system  
2. ✅ **Final Report** with detailed explanation of code structure  
3. ✅ **Source Code** (this repository)

---

## 📏 ADC Voltage Range

Using the on-board potentiometer, the ADC reads analog voltages in the approximate range of:
- **Minimum Voltage**: ~0.00 V
- **Maximum Voltage**: ~3.30 V (based on 3.3V reference on Nucleo board)

---

## 📦 How to Build & Flash

1. Open the project in STM32CubeIDE or your preferred IDE.
2. Connect your Nucleo-F401RE board via USB.
3. Build the project.
4. Flash it to the board and observe the 7-segment display behavior.

---

## 🎥 Demo Video



https://github.com/user-attachments/assets/18e439ed-a508-451e-a2b7-f4c1124f3c4b



---

## 👨‍💻 Authors
- Marwan Ashraf
- Kyrillos Hany
- Mina Waguih

---

## 📄 License

This project is submitted as coursework for academic purposes. Please respect academic integrity policies.
Spring 2025 – Ain Shams University

---

