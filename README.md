# 🎲 Digital Random Number Generator PCB

![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)
![PCB Design](https://img.shields.io/badge/PCB-KiCad-blue.svg)
![Project Status](https://img.shields.io/badge/Status-Completed-success.svg)

A custom-designed **Digital Random Number Generator PCB** developed using **KiCad**.  
This project uses an 8051-family microcontroller, dual seven-segment displays, 74LS48 BCD-to-seven-segment display driver ICs, push-button controls, and a regulated 5V logic power supply to generate and display random numbers.

---

## 📌 Project Overview

The **Digital Random Number Generator PCB** is a digital electronics and embedded hardware project designed to generate and display random numbers using two seven-segment displays.

The circuit is built around an **8051-family microcontroller**, which handles the random number generation logic. The generated number is separated into two BCD digits and sent to two **74LS48 BCD-to-seven-segment decoder/driver ICs**. Each driver IC then controls one seven-segment display.

This project demonstrates the complete PCB design workflow in KiCad, including schematic design, component footprint assignment, PCB layout, routing, silkscreen labeling, 3D visualization, and preparation for fabrication.

---

## ✨ Key Features

- Microcontroller-based random number generation
- Dual seven-segment display output
- 74LS48 BCD-to-seven-segment decoder/driver ICs
- Push-button input for number generation
- Dedicated reset/control button
- 5V DC logic power input
- Crystal oscillator circuit for microcontroller clock generation
- Current-limiting resistors for display protection
- Organized schematic sections for power, control, and display output
- Compact PCB layout with mounting holes
- Complete KiCad schematic, PCB layout, and 3D PCB preview

---

## 🧠 System Architecture

```txt
Push Button Input
        ↓
8051 Microcontroller
        ↓
Random Number Generation Logic
        ↓
BCD Output Signals
        ↓
74LS48 Display Driver ICs
        ↓
Dual Seven-Segment Displays
```

---

## ⚙️ Hardware Description

The PCB is divided into three main sections:

1. **Power Supply Section**
2. **Random Number Generation Control Section**
3. **Display Driver and Seven-Segment Output Section**

The user presses the push button to trigger the random number generation process. The microcontroller generates a random value and sends the corresponding BCD output signals to the display driver ICs. The 74LS48 ICs decode the BCD signals and drive the seven-segment displays.

---

## 🧩 Main Components

| Component | Description |
|---|---|
| 8051 Microcontroller | Main control unit used for random number generation |
| 74LS48 IC | BCD-to-seven-segment decoder/driver |
| Seven-Segment Displays | Displays the generated random number |
| Push Buttons | Used for reset and random number generation control |
| Crystal Oscillator | Provides the clock signal for the microcontroller |
| Capacitors | Used for oscillator stability, reset timing, and filtering |
| Resistors | Used for current limiting and pull-up/pull-down functions |
| Screw Terminal | Provides external 5V power input |
| PCB | Custom-designed printed circuit board created using KiCad |

---

## ⚡ Power Supply

The circuit is designed to operate using a regulated **5V DC power supply**.

Power is supplied through a screw terminal connector.

```txt
+5V  → VCC
GND  → Ground
```

> ⚠️ Always verify the power polarity before powering the PCB.

---

## 🔢 Display Driver Section

The display section uses two **74LS48 BCD-to-seven-segment decoder/driver ICs**.

Each display driver receives a 4-bit BCD input from the microcontroller and controls one seven-segment display. Current-limiting resistors are used to protect the display segments.

The display section includes:

- Two seven-segment displays
- Two 74LS48 display driver ICs
- Segment current-limiting resistors
- BCD signal routing from the microcontroller
- Seven-segment output routing to the displays

---

## 🎛️ Control Section

The control section contains the main microcontroller circuit and supporting components.

It includes:

- 8051-family microcontroller
- Push-button input
- Reset button
- Crystal oscillator circuit
- Oscillator capacitors
- Reset capacitor
- Pull-up/pull-down resistors

The microcontroller manages the random number generation process and sends the correct BCD values to the display driver section.

---

## 🖥️ PCB Design

The PCB was designed using **KiCad** and includes:

- Schematic capture
- Footprint assignment
- PCB layout design
- Manual routing
- Silkscreen labeling
- Mounting holes
- 3D PCB visualization
- Fabrication-ready design structure

The board layout is organized to clearly separate the power input, microcontroller control section, and display output section.

---

## 📷 PCB Preview

The project includes the following design previews:

### Schematic

<img width="1332" height="790" alt="image" src="https://github.com/user-attachments/assets/f1ae511b-3926-4e8e-965b-1aaf17f32330" />

![Schematic](images/schematic.png)

### PCB Layout
<img width="787" height="590" alt="image" src="https://github.com/user-attachments/assets/6f053cf9-9607-44b0-b32e-1d7d82930a3e" />

![PCB Layout](images/pcb-layout.png)

### 3D View

<img width="893" height="836" alt="image" src="https://github.com/user-attachments/assets/2b5b3d40-ff3a-4f4a-a4c3-8733d09bdbf0" />
<img width="1079" height="857" alt="image" src="https://github.com/user-attachments/assets/7673b002-5eed-468b-b001-a8e7f95f6ed1" />
<img width="954" height="804" alt="image" src="https://github.com/user-attachments/assets/5623065a-372f-4d3c-a419-2d82d28b806d" />
<img width="954" height="741" alt="image" src="https://github.com/user-attachments/assets/b57711ba-6243-4efe-a75d-9b43e9d94268" />
<img width="1064" height="861" alt="image" src="https://github.com/user-attachments/assets/5faf467c-ee9d-48e9-b4de-ff0d022af7e3" />

![3D View](images/3d-front.png)


---

## 🚀 Applications

This PCB can be used for:

- Digital electronics learning
- Embedded systems practice
- Microcontroller-based hardware design
- Seven-segment display driver testing
- Random number display applications
- KiCad PCB design portfolio development
- Basic digital logic demonstration projects

---

## ✅ Project Status

| Section | Status |
|---|---|
| Schematic Design | Completed |
| PCB Layout | Completed |
| 3D PCB Preview | Completed |
| Gerber File Export | Ready / To be generated |
| Hardware Testing | Pending |

---

## 👨‍💻 Author

**Fernando S.M.H.G.**

---

## 📜 License

This project is licensed under the **MIT License**.

You are free to use, modify, and distribute this project for educational, personal, and development purposes, provided that the original license terms are followed.

See the `LICENSE` file for more details.
