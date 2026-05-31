# TGC-Core Devboard Mega v1

![Board Render](TGC-Core-devboard-Mega-v1.png)

## Overview
The **TGC-Core-devboard-Mega-v1** is an open-source hardware development board. Based on the file naming and standard conventions, it is designed around the "Mega" architecture (typically the Microchip ATmega2560) but upgraded with modern physical interfaces, such as a **USB-C** connector for power and data, and standard 6mm tactile push buttons for reset/user input. 

This repository contains the complete set of KiCad EDA files necessary to view, modify, and manufacture the printed circuit board (PCB).

---

## Features
* **Architecture:** Mega-compatible (ATmega2560) platform.
* **Modern Connectivity:** Upgraded from the legacy USB Type-B to a robust **USB-C 2.0** connector.
* **Native KiCad Design:** Fully designed using KiCad, allowing for easy community modification and inspection.
* **Standard Form Factor:** Designed for compatibility with existing shields and standard development workflows.

---

## Repository Structure

The project is entirely self-contained within the following KiCad design files:

| File Name | Description |
| :--- | :--- |
| `TGC-Core-devboard-Mega-v1.kicad_pro` | The main **KiCad Project file**. Open this file to load the entire project space. |
| `TGC-Core-devboard-Mega-v1.kicad_sch` | The **Schematic file**. Contains the logical connections, components (like the USB-C plug and SW_Push buttons), and wiring. |
| `TGC-Core-devboard-Mega-v1.kicad_pcb` | The **PCB Layout file**. Contains the physical board routing, copper layers, and silkscreen definitions. |
| `TGC-Core-devboard-Mega-v1.png` | A visual render or top-down image of the board design. |

---

## Hardware Specifications (Expected)

*Based on standard Mega-compatible board parameters:*

* **Microcontroller:** ATmega2560 (8-bit AVR)
* **Operating Voltage:** 5V
* **Clock Speed:** 16 MHz
* **Digital I/O Pins:** 54 (of which 15 provide PWM output)
* **Analog Input Pins:** 16
* **Hardware Serial Ports (UARTs):** 4
* **Flash Memory:** 256 KB (8 KB used by bootloader)
* **SRAM:** 8 KB
* **EEPROM:** 4 KB

---

## Getting Started

### 1. Viewing and Editing the Hardware
To view or modify the hardware design:
1. Download and install [KiCad EDA](https://www.kicad.org/). *(Note: Ensure your KiCad version is up to date, as these files use modern KiCad file formatting).*
2. Open the `TGC-Core-devboard-Mega-v1.kicad_pro` file.
3. From the project manager, open the Schematic Editor or PCB Editor to explore the design.

### 2. Software & Programming
Because this board shares the Mega architecture, it is fully compatible with the standard Arduino ecosystem:
1. Open the [Arduino IDE](https://www.arduino.cc/en/software).
2. Connect the board via a USB-C cable to your computer.
3. Go to **Tools > Board** and select **Arduino Mega or Mega 2560**.
4. Go to **Tools > Port** and select the active COM port.
5. Upload your sketches normally.

---

## License

This hardware design and its accompanying documentation are licensed under the **Creative Commons Attribution 4.0 International (CC BY 4.0)** Public License.

**You are free to:**
* **Share** — copy and redistribute the material in any medium or format.
* **Adapt** — remix, transform, and build upon the material for any purpose, even commercially.

**Under the following terms:**
* **Attribution** — You must give appropriate credit, provide a link to the license, and indicate if changes were made. You may do so in any reasonable manner, but not in any way that suggests the licensor endorses you or your use.

For the full legal text, please visit the [Creative Commons Website](https://creativecommons.org/licenses/by/4.0/).
