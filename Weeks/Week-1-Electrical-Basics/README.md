# Week 1 — Electrical Fundamentals, Resistors & KiCad 8.0 Intro

[![Week](https://img.shields.io/badge/Week-1%20of%206-blue.svg)](#)
[![Focus](https://img.shields.io/badge/Focus-Ohm's%20%7C%20KVL%2FKCL%20%7C%20KiCad%20Intro-brightgreen.svg)](#)

Welcome to **Week 1** of the Apex Racing Team Electrical Low Voltage Onboarding Track.

---

## Weekly Objectives
1. **Circuit Quantities & Fundamentals**: Voltage, current, resistance, power ($P = V \times I$). Units and metric prefixes.
2. **Resistor Engineering**: Resistor color bands, power derating ($1/4\text{W}, 1/2\text{W}, 1\text{W}$), SMD resistor codes (0805, 1206).
3. **Network Theorems**: Series and parallel equivalent resistance; Voltage divider formula; Kirchhoff's Voltage and Current Laws (KVL/KCL).
4. **KiCad 8.0 Fundamentals**: Project creation (`.kicad_pro`), schematic capture editor (`.kicad_sch`), placing symbols, wires, labels, `PWR_FLAG`, and running Electrical Rules Check (ERC).

---

## Daily Operational Guide & Curated Links

* **Day 1 (Monday) — Circuit Fundamentals & Resistors**:
  * 📺 [Circuit Analysis & Ohm's Law](https://www.youtube.com/watch?v=F_vLWkkOETI)
  * 📺 [Resistor Color Codes & Ratings](https://www.youtube.com/watch?v=uXr4lAP8XVE)
  * Solve short V/I/R/P calculation set; decode 5 resistor color bands.
* **Day 2 (Tuesday) — Voltage Dividers & KCL/KVL**:
  * Derive voltage divider formula: $V_{out} = V_{in} \frac{R_2}{R_1 + R_2}$.
  * Calculate divider values to scale $12\text{V}$ battery bus to $3.3\text{V}$ logic levels.
* **Day 3 (Wednesday) — Live Session: KiCad 8.0 Schematic Capture**:
  * 45-min live session: installing KiCad 8.0, project creation, schematic editor shortcuts (`A` place symbol, `W` wire, `R` rotate).
  * 📺 [KiCad 8.0 Beginner Tutorial (Part 1)](https://www.youtube.com/watch?v=aVUqo3PC6wo)
* **Day 4 (Thursday) — ERC & Power Flags**:
  * Learn why KiCad requires `PWR_FLAG` on power rails and how to resolve common ERC errors.
  * Draw voltage divider + LED indicator schematic; pass ERC with 0 errors.
* **Day 5 (Friday) — Offline Workshop Day**:
  * Meet mentor at team lab: assemble voltage divider on breadboard.
  * 📺 [How to Use a Digital Multimeter](https://www.youtube.com/watch?v=ts0EKAmNxv0)
  * Measure actual circuit voltages vs theoretical calculations.
* **Day 6 (Saturday) — Week 1 Submission**:
  * Submit problem set + KiCad schematic files by 11:59 PM.
* **Day 7 (Sunday) — Friendly 1-on-1 Oral Check-in**:
  * 10-minute check-in: explain voltage divider calculation and KiCad ERC rules.
