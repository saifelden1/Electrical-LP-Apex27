# Week 5 — Sensors, Signal Conditioning & KiCad PCB Layout

[![Week](https://img.shields.io/badge/Week-5%20of%206-blue.svg)](#)
[![Focus](https://img.shields.io/badge/Focus-Analog%20Front-Ends%20%7C%20PCB%20Layout-brightgreen.svg)](#)
[![Task](https://img.shields.io/badge/Task-task--2--daq--pcb-orange.svg)](#)

Welcome to **Week 5** of the Apex Racing Team Electrical Low Voltage Onboarding Track.

---

## Weekly Objectives
1. **Automotive Sensor Front-Ends**: Analog vs digital sensor outputs; temperature (NTC, PT1000), pressure transducers ($0.5\text{V} - 4.5\text{V}$), wheel speed (Hall effect).
2. **Passive Signal Conditioning**: Voltage divider scaling (5V down to 3.3V ADC levels), first-order RC low-pass filter design ($f_c$).
3. **Noise & EMI Mitigation**: Conducted vs radiated noise, shielded twisted pair (STP) cabling, single-ended shield grounding, ceramic decoupling capacitors.
4. **KiCad PCB Layout**: Importing netlist, component placement strategy, power routing, trace width sizing via **IPC-2152**, continuous ground plane pour, and running Design Rules Check (DRC).
5. **Systematic Diagnostics**: Multimeter fault-finding procedure (voltage-drop, continuity, resistance) on sensor circuits.

---

## Daily Operational Guide & Curated Links

* **Day 1 (Monday) — Sensor Conditioning & RC Filters**:
  * 📺 [Automotive Sensor Types & Conditioning](https://www.youtube.com/watch?v=pP5K9x_M2Y4)
  * 📺 [RC Low-Pass Filter Design & Calculations](https://www.youtube.com/watch?v=OBM5T5_V8eY)
  * Calculate $R$ and $C$ for a $100\text{ Hz}$ cutoff filter on a suspension sensor.
* **Day 2 (Tuesday) — Noise, EMI & Shielding**:
  * 📺 [Electrical Noise, EMI & Shielding](https://www.youtube.com/watch?v=7X8M2v5Y9pA)
  * Review vehicle harness layout; mark noise-sensitive analog lines and shielding points.
* **Day 3 (Wednesday) — Live Session: Task 2 DAQ PCB Layout**:
  * 45-min live session: PCB layout workflow in KiCad 8.0, component placement, power trace routing, and ground plane pours.
  * 📺 [KiCad 8.0 PCB Layout Tutorial](https://www.youtube.com/watch?v=C7-8nAUq4Lc)
  * Task specifications: [`Tasks/Task-2-DAQ-PCB/README.md`](../../Tasks/Task-2-DAQ-PCB/README.md)
* **Day 4 (Thursday) — IPC-2152 Trace Widths & DRC**:
  * 🔗 [IPC-2152 Trace Width Calculator](https://www.4pcb.com/trace-width-calculator.html)
  * Calculate trace widths for power ($1.0\text{ mm}$) and signal ($0.25\text{ mm}$); run DRC with 0 errors.
* **Day 5 (Friday) — Offline Workshop Day**:
  * 📺 [Systematic Electrical Fault Finding](https://www.youtube.com/watch?v=qX1X8Y8Z9zA)
  * Meet at workshop: troubleshoot a pre-faulted sensor circuit board using systematic multimeter tests.
* **Day 6 (Saturday) — Milestone Task 2 Submission**:
  * Submit Task 2 deliverable: KiCad PCB layout + Gerber files + report by 11:59 PM.
* **Day 7 (Sunday) — Friendly 1-on-1 Oral Check-in**:
  * 10-minute check-in: explain ground plane continuity, filter cutoff math, and IPC trace sizing.
