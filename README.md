# 🧠 ATmega32 Test Kit  

<img width="820" height="557" alt="Screenshot 2025-10-13 234818" src="https://github.com/user-attachments/assets/e3e09dd6-50f9-46b0-bba8-dd24b15c010f" />  

## 📘 Overview
The **ATmega32 Test Kit** is a custom-built hardware platform designed for **testing drivers, firmware, and basic embedded code** on the ATmega32 microcontroller.  
It provides **easy access to I/O ports**, visual feedback through **LEDs**, **push buttons**, and **display interfaces** (LCD + 7-segment), making it ideal for quick debugging and learning microcontroller programming.

> 🧩 Developed by [Youssef Alaa](https://github.com/Youssef5562)  
> Date: **13 / 10 / 2025**

---

## ⚙️ Features

- 🔹 8 LEDs (PORTD) for digital output testing  
- 🔹 8 Push Buttons (PORTC or PORTB) for digital input testing  
- 🔹 7-Segment Display (via 74HC4511 driver)  
- 🔹 16x2 LCD display interface (4-bit mode)  
- 🔹 Reset button  
- 🔹 Ready ISP header for programming  
- 🔹 Clearly labeled ports for easier debugging  
- 🔹 Designed for **CodeVisionAVR**, **Proteus simulation**, or **real hardware**

---

## 🧰 Components Used

| Component | Quantity | Description |
|------------|-----------|-------------|
| **ATmega32** | 1 | Main microcontroller |
| **LEDs** | 8 | Output indication |
| **Push Buttons** | 8 | Input testing |
| **Resistors (220Ω, 10kΩ)** | Several | For LEDs and pull-ups |
| **74HC4511** | 1 | 7-Segment display driver |
| **7-Segment Display** | 1 | Numeric output test |
| **16x2 LCD** | 1 | Text display testing |
| **Reset Switch** | 1 | Manual reset |
| **Capacitors (0.1µF, 10µF)** | Several | Decoupling and power filtering |
| **Power Source (5V)** | 1 | External or USB-powered |

---

## 🖥️ Pin Mapping

| Function | Port | Notes |
|-----------|------|-------|
| LEDs | PORTD (D0–D7) | Active HIGH |
| Push Buttons | PORTC (C0–C7) | Pulled-up inputs |
| LCD | PORTA / PORTB | Configurable |
| 7-Segment | PORTB + 74HC4511 | Display driver |
| Reset | RESET pin | Pull-up with 10kΩ |
| Power | VCC = 5V | Common GND |


```bash
git clone https://github.com/Youssef5562/ATmega32-Test-Kit.git
cd ATmega32-Test-Kit
