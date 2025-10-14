# USB-C Power Supply
> 3D  viwe
>
> <img width="438" height="470" alt="USB-C Power Supply correct way" src="https://github.com/user-attachments/assets/942fa11f-27ee-4ab7-af6f-745e009d5cb1" />

<img width="438" height="470" alt="USB-C Power Supply layout" src="https://github.com/user-attachments/assets/9d56daf3-6dff-4510-91b3-bffc93127122" />

> Layout


<img width="438" height="470" alt="Screenshot 2025-10-14 204818" src="https://github.com/user-attachments/assets/65bbc996-5c2c-42aa-874d-115fa6e00605" />


# USB-C Power Supply

## Overview
This project demonstrates the complete design and development of a **USB-C Power Supply** circuit.  
The goal was to create a small PCB that outputs **5 V** through a **USB Type-C** connector using correct CC (Configuration Channel) resistors.  
The board includes a power indicator LED, decoupling capacitors, and is fully ready for **JLCPCB** manufacturing.

---

## What Was Done
- Designed a **schematic** in **KiCad 8.0** for a 5 V USB-C power source.  
- Implemented **CC1** and **CC2 pull-down resistors (5.1 kΩ)** for correct USB-C negotiation.  
- Added **100 nF decoupling capacitor** for voltage stability.  
- Added **LED indicator** with **1 kΩ resistor** for power-on status.  
- Created and annotated all symbols and footprints in KiCad.  
- Designed a **two-layer PCB layout** following **JLCPCB** design rules.  
- Defined **board outline, silkscreen labels, mounting holes**, and reference text.  
- Generated **Gerber**, **Drill**, **BOM**, and **Pick-and-Place** files for fabrication.  
- Verified schematic (ERC) and layout (DRC) before manufacturing.  
- Prepared files for **JLCPCB assembly** and optional 3D-printed enclosure.

---

## Hardware Details
| Parameter | Description |
|------------|-------------|
| **Input** | USB-C Receptacle (VBUS = 5 V) |
| **Output** | 2-Pin Header (5 V / GND) |
| **Resistors** | 5.1 kΩ × 2 (CC1/CC2), 1 kΩ × 1 (LED) |
| **Capacitors** | 100 nF (Decoupling) |
| **Indicator** | Power LED |
| **Board Layers** | 2 |
| **Power** | 5 V @ up to 3 A |
| **Mounting** | 4 × M2 holes |

---

## Project Files
- `USB-C Power Supply.kicad_pro` – KiCad project file  
- `USB-C Power Supply.kicad_sch` – Schematic  
- `USB-C Power Supply.kicad_pcb` – PCB layout  
- `SCH.pdf` – Printable schematic reference  

---

## Manufacturing and Assembly
1. Export **Gerber** and **Drill** files from KiCad.  
2. Upload the ZIP archive to [**JLCPCB**](https://jlcpcb.com).  
3. Choose desired solder-mask and silkscreen colors.  
4. (Optional) Add logo or image for silkscreen layer.  
5. Order boards (with or without assembly) and test after delivery.

---

## Testing
- Connected a USB-C cable from a 5 V adapter.  
- Verified **5 V output** at the terminal header.  
- Observed **LED indicator ON** confirming active power.  
- Ensured no short circuits or trace issues.

---

## Results
The PCB provides a **stable 5 V output**, compact design, and clear labeling.  
It can serve as a reference or base module for **USB-powered embedded projects** or **sensor systems** that need a simple regulated power supply.

---

## Tools Used
- **KiCad 8.0** – Schematic capture and PCB layout  
- **JLCPCB** – PCB manufacturing and assembly  
- **Fusion 360 (optional)** – Enclosure and 3D model design  

---

## Author
**Moiz Zaheer Malik**  
Hochschule Hamm-Lippstadt (HSHL)  
October 2025
