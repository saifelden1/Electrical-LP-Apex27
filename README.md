# Apex Racing Team — Electrical Low Voltage (LV) Systems Learning Phase

[![Platform](https://img.shields.io/badge/CAD-KiCad%208.0+-blue.svg)](https://www.kicad.org)
[![Subsystem](https://img.shields.io/badge/System-Low%20Voltage%20(LV)%20%26%20DAQ-darkgreen.svg)](#)
[![Standards](https://img.shields.io/badge/Standards-IPC--2152%20%7C%20FS%20Rules-orange.svg)](#)
[![Harnessing](https://img.shields.io/badge/Wiring-Raychem%20DR--25%20%7C%20Deutsch%20DT-brightgreen.svg)](#)

Welcome to the **Apex Racing Team** Electrical Low Voltage (LV) Systems Onboarding & Training Track. This training program is designed to develop foundational engineering proficiency in low-voltage vehicle electronics, circuit protection, sensor data acquisition (DAQ) signal conditioning, printed circuit board (PCB) design using **KiCad 8.0**, and motorsport-grade wiring harness fabrication.

---

## Repository Structure & Curriculum Map

All weekly learning guides and hands-on milestone tasks are organized into isolated Git branches and mirrored directly inside local directories on `main` for instant navigation:

```bash
git clone https://github.com/saifelden1/Electrical-LP-Apex27.git
cd Electrical-LP-Apex27
```

### 6-Week Curriculum Roadmap & Materials
| Week | Module | Assigned Materials | Core Focus Areas | Local Directory | Branch |
| :--- | :--- | :---: | :--- | :--- | :--- |
| **Week 1** | Fundamentals & KiCad Intro | **4 Videos** (~1.2h) | Ohm's/Kirchhoff's Laws, Resistor ratings, Voltage dividers, KiCad 8.0 schematic setup & ERC | [`Weeks/Week-1-Electrical-Basics/`](Weeks/Week-1-Electrical-Basics/) | `week-1-electrical-basics` |
| **Week 2** | Components & Switching | **5 Videos** (~1.5h) | Capacitors, Inductors & flyback diodes, Relays vs Power MOSFETs ($R_{DS(on)}$, $V_{GS}$), E-Stop switches | [`Weeks/Week-2-Components-Switching/`](Weeks/Week-2-Components-Switching/) | `week-2-components-switching` |
| **Week 3** | Protection & Wire Sizing | **5 Videos** (~1.5h) | Fuse selection, Wire gauge ($AWG/mm^2$) coordination, P-MOSFET reverse polarity, TVS diodes | [`Weeks/Week-3-Protection-Safety/`](Weeks/Week-3-Protection-Safety/) | `week-3-protection-safety` |
| **Week 4** | Power Distribution & Harness | **5 Videos** (~1.5h) | LV power budgeting (peak/continuous), Automotive harness routing, Deutsch DT crimping, Star ground | [`Weeks/Week-4-Power-Harnessing/`](Weeks/Week-4-Power-Harnessing/) | `week-4-power-harnessing` |
| **Week 5** | Sensors, DAQ & KiCad PCB | **6 Videos** (~1.8h) | Analog front-ends (scaling, RC filtering), Noise/EMI shielding, KiCad 2-layer PCB layout & IPC-2152 | [`Weeks/Week-5-Sensors-DAQ-PCB/`](Weeks/Week-5-Sensors-DAQ-PCB/) | `week-5-sensors-daq-pcb` |
| **Week 6** | Vehicle LV Architecture & SDC | **4 Videos** (~1.2h) | Formula Student EV LV vs HV, Shutdown Circuit (SDC) loop, ECU pinouts, Dual-MCU/Embedded interface | [`Weeks/Week-6-Vehicle-LV-Integration/`](Weeks/Week-6-Vehicle-LV-Integration/) | `week-6-vehicle-lv-integration` |

### Practical Milestone Tasks (Hardware & CAD Deliverables)
| Task | Target Systems | Key Deliverable | Local Directory | Branch |
| :--- | :--- | :--- | :--- | :--- |
| **Task 1: PDU Input Protection** | Fuse, P-MOSFET, TVS | KiCad schematic of complete input protection stage, ERC verification, wire/fuse calculation sheet | [`Tasks/Task-1-PDU-Protection/`](Tasks/Task-1-PDU-Protection/) | `task-1-pdu-protection` |
| **Task 2: Sensor DAQ PCB Layout** | 4-Ch Analog Front-End | 2-layer KiCad PCB layout, RC low-pass filters, IPC-2152 trace widths, DRC pass, Gerber exports | [`Tasks/Task-2-DAQ-PCB/`](Tasks/Task-2-DAQ-PCB/) | `task-2-daq-pcb` |
| **Task 3: Vehicle Harness & SDC** | Full LV System, E-Stops | Complete vehicle LV wiring schematic, Shutdown Circuit (SDC) loop, ECU pinout spec, crimp log | [`Tasks/Task-3-Harness-SDC/`](Tasks/Task-3-Harness-SDC/) | `task-3-harness-sdc` |

---

## Master Spreadsheet Roadmap (`APEX_Electric_Learning_Plan.xlsx`)

The repository root includes a comprehensive planning workbook structured with:
1. **`6_Week_Curriculum`**: High-contrast, screenshot-ready overview with video counts and watch times for team announcement channels.
2. **`Resource_Directory`**: Central indexed table of all video tutorials, KiCad 8.0 guides, IPC standards, and Formula Student rules.
3. **`W1_Daily_Operations` – `W6_Daily_Operations`**: Actionable day-by-day operations following the proven 7-day cadence (Main sessions, Live whiteboard, KiCad design, Offline workshop, Deliverable submission, Oral review).
4. **`Suggestions_and_Rules`**: Formula Student LV scrutineering rules and motorsport design best practices.

---

## Training Philosophy & Oral Defense Policy

> [!IMPORTANT]
> **Engineering Rigor & Oral Defense Standard**
> * Using AI tools (Claude, ChatGPT, Gemini, etc.) as research assistants and calculation checkers is **permitted and encouraged**.
> * **However**, submitting schematics, PCB layouts, or wire calculations without complete first-principles comprehension is strictly disqualified.
> * **Every candidate will participate in an individual 1-on-1 technical oral defense where you must explain and justify every component value, trace width, fuse rating, and layout decision in your submission.**
> * If you cannot clearly defend why a capacitor value was chosen, how trace heating was calculated, or how the shutdown circuit remains fail-safe, the milestone will not be accepted.

---

## Required Submission Package

For each completed milestone task, candidates must submit:
1. **KiCad Project Files**: Complete `.kicad_pro`, `.kicad_sch`, and `.kicad_pcb` files passing ERC and DRC with **0 errors**.
2. **Manufacturing Deliverables (Gerbers)**: For PCB tasks, complete RS-274X Gerber layers and Excellon drill files.
3. **Engineering Calculations**: Detailed math for power budgets, wire sizing ($I_{wire} > I_{fuse}$), voltage drops, and filter cutoffs ($f_c$).
4. **Physical / Simulation Proof**: Clear photos/videos of breadboard measurements, crimp pull-tests, or multimeter testing.
5. **Technical Report**: Completed [`Template_Report.md`](Tasks/Task-1-PDU-Protection/Template_Report.md) documenting design choices and troubleshooting logs.

---

## Toolchain & CAD Setup
* **CAD Software**: [KiCad 8.0 or newer](https://www.kicad.org/download/).
* **Standards Reference**: IPC-2152 (Trace sizing for current and temperature rise).
* **Hand Tools (Workshop)**: Digital multimeter, wire strippers, ratcheting crimpers (open-barrel & Deutsch), heat gun.
