# Task 2 — Sensor DAQ Signal Conditioning & 2-Layer PCB Layout

[![Target](https://img.shields.io/badge/System-Sensor%20DAQ%20%7C%20PCB-blue.svg)](#)
[![CAD](https://img.shields.io/badge/CAD-KiCad%208.0-brightgreen.svg)](#)
[![Standards](https://img.shields.io/badge/Standard-IPC--2152%20%7C%20DRC-brightgreen.svg)](#)

---

## Objective
Vehicle sensors operate in an electrically hostile motorsport environment filled with ignition spikes, inductive kickback, and inverter switching noise. In this task, you will design a **4-Channel Sensor Data Acquisition (DAQ) Front-End** schematic and lay out a manufacturing-ready **2-Layer PCB** in **KiCad 8.0**.

---

## Circuit Specifications
1. **Analog Sensor Channels (Channels 1 & 2)**:
   * Designed for $0\text{V} - 5\text{V}$ automotive sensors (e.g. linear suspension potentiometers, brake pressure transducers).
   * Resistor divider to scale $5\text{V}$ maximum sensor output down to **$3.3\text{V}$** for STM32 / MCU ADC inputs ($R_1 = 5.1\text{ k}\Omega, R_2 = 10\text{ k}\Omega$).
   * Passive first-order RC low-pass filter with a cutoff frequency of **$f_c \approx 100\text{ Hz}$** to attenuate high-frequency noise.
2. **Digital / Pulse Channels (Channels 3 & 4)**:
   * Designed for open-collector Hall-effect wheel speed sensors.
   * Onboard $4.7\text{ k}\Omega$ pull-up resistor to $+5\text{V}$ rail.
   * Series current-limiting resistor ($1\text{ k}\Omega$) and $3.3\text{V}$ clamping protection.
3. **Power & Connectors**:
   * $+12\text{V}$ battery input with basic onboard linear or LDO regulation ($+5\text{V}$ and $+3.3\text{V}$).
   * Automotive-grade screw terminal or Molex Micro-Fit connector for sensor harness inputs.
   * Standard header connector for interface cable to the Embedded MCU ECU board.

---

## PCB Layout Constraints
* **Board Dimensions**: Maximum $60\text{ mm} \times 50\text{ mm}$, 2 copper layers ($1.6\text{ mm}$ FR4, $1\text{ oz}$ copper).
* **Layer Stackup**:
  * **Top Layer**: Signal routing, power rails, component placement (SMD 0805 passives preferred).
  * **Bottom Layer**: Continuous, unbroken ground plane (GND copper pour).
* **Trace Width Sizing (IPC-2152)**:
  * Power rails ($+12\text{V}, +5\text{V}$): Minimum **$1.0\text{ mm}$** width.
  * Analog & digital signal traces: **$0.25\text{ mm} - 0.35\text{ mm}$** width.
  * Minimum electrical clearance: **$0.25\text{ mm}$** ($10\text{ mils}$).
* **Decoupling Placement**: $100\text{ nF}$ ceramic bypass capacitors placed directly adjacent to IC power pins with short vias to ground.

---

## Technical Deliverables
1. **KiCad Schematic & PCB Layout**:
   * Complete `.kicad_sch` and `.kicad_pcb` passing Design Rules Check (DRC) with **0 errors**.
2. **Manufacturing Package**:
   * Standard RS-274X Gerber files (`.gbr`) and Excellon drill files (`.drl`) exported to `Fabrication/Gerber/`.
3. **Technical Report**:
   * Completed `Template_Report.md` documenting RC filter cutoff calculations, IPC trace width math, and 3D PCB views.
