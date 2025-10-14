# Binary Watch (ATtiny1616)

> **Inspired by:** taifur https://www.instructables.com/member/taifur/

 > [PCB Binary Watch – Instructables](https://www.instructables.com/PCB-Binary-Watch/)

This project is a **Binary Digital Watch** designed in **KiCad** using an **ATtiny1616** microcontroller.  
It displays the time using LEDs arranged in binary form, powered by a coin-cell battery and driven by a real-time clock (RTC).



<img width="438" height="470" alt="Screenshot 2025-10-14 210819" src="https://github.com/user-attachments/assets/a9c9edce-4c22-4671-a846-9b85bcb7d073" />

<img width="438" height="470" alt="Screenshot 2025-10-13 041315" src="https://github.com/user-attachments/assets/def53c58-b1f2-48ce-8356-3de8b79c05c4" />

<img width="438" height="470" alt="Screenshot 2025-10-13 041339" src="https://github.com/user-attachments/assets/6e69358f-7ccd-45c3-9abf-1135f80cbc59" />

---

##  Overview
- **MCU:** ATtiny1616 (AVR 0-series)
- **Power Source:** CR2032 coin-cell battery
- **Display:** 13 LEDs (binary representation of hours and minutes)
- **Resistors:** Current-limiting for LED control
- **Clock:** External RTC for accurate timekeeping
- **PCB:** 2-layer FR-4 board, compact circular layout for wristwatch form factor

---

##  Circuit Highlights
- The LEDs are arranged in groups:
  - **Hours (1–12)** → 4 LEDs (binary)
  - **Minutes (0–59)** → 6 LEDs (binary)
  - Controlled via GPIO pins of the ATtiny1616.
- **Resistors** limit LED current to protect the MCU pins.
- **Coin-cell holder (U4)** provides power and acts as the mechanical base.
- **UPDI header** included for programming the microcontroller.

---

##  PCB Design
- Designed and routed in **KiCad 8**.
- Features:
  - Front copper layer: signal traces and LED anodes.
  - Back copper layer: ground pour (GND).
  - Thermal reliefs for soldering.
  - Tented vias to avoid solder mask shorts.
- Optimized for low current draw and minimal power loss.

---

##  Fabrication Settings
| Parameter | Value |
|------------|--------|
| Layers | 2 |
| Material | FR-4 |
| Thickness | 1.6 mm |
| Finish | HASL-Lead-Free |
| Min track/space | 0.2 mm |
| Via | 0.6 mm / 0.3 mm drill |
| Solder mask | Green |
| Silkscreen | White |

---

##  Assembly & Testing
1. Program ATtiny1616 via **UPDI** interface.
2. Verify RTC communication and LED output sequence.
3. Insert CR2032 cell and confirm LED time display pattern.
4. Measure current draw to ensure low-power standby operation.

---

##  Files
- `Binary Watch.kicad_sch` — complete schematic  
- `Binary Watch.kicad_pcb` — routed PCB layout  
- `BOM.csv` — parts list for fabrication and assembly  

---

##  Future Improvements
- Add button input for time-setting.
- Integrate charging circuit for Li-ion coin cell.
- Add low-power sleep and wake functions in firmware.

---

### Author
Designed by **Moiz Zaheer Malik**  
Location: **Lippstadt, Germany**

---


