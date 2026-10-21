# Task 1 — Basic Protection & Power Distribution (PDU) Input Stage

[![Target](https://img.shields.io/badge/System-Circuit%20Protection%20%7C%20PDU-blue.svg)](#)
[![CAD](https://img.shields.io/badge/CAD-KiCad%208.0-brightgreen.svg)](#)
[![Milestone](https://img.shields.io/badge/Milestone-Task%201%20of%203-orange.svg)](#)

---

## Objective
Every vehicle ECU and power distribution node requires robust front-end electrical protection against automotive transients, human wiring errors, and catastrophic short circuits. In this task, you will design, calculate, and capture a complete **Automotive Input Protection Stage** in **KiCad 8.0**.

---

## Circuit Requirements & Specifications

The input protection circuit must safely condition a nominal **12V DC Low-Voltage Battery** bus supplying up to **5A continuous load**:

1. **Overcurrent Protection (Fuse)**:
   * Select a standard automotive blade fuse (ATO/ATC or Mini).
   * Fuse must be coordinated with vehicle wiring: $I_{continuous} \le I_{fuse} < I_{wire\_capacity}$.
2. **Reverse Polarity Protection (P-Channel MOSFET)**:
   * Protect downstream electronics against accidental reverse battery connection ($ -12\text{V} $ applied).
   * Implement an **ideal diode circuit** using a P-Channel Power MOSFET, gate pull-down resistor, and Zener gate clamp diode.
   * Total conduction voltage drop must be $< 0.1\text{V}$ at $5\text{A}$ ($R_{DS(on)} \le 20\text{ m}\Omega$).
3. **Transient Overvoltage Suppression (TVS Diode)**:
   * Bidirectional or Unidirectional automotive-grade TVS diode (e.g. SMCJ18A or SMBJ24A).
   * Clamping voltage must not exceed downstream component maximum ratings ($< 30\text{V}$).
4. **Bulk Decoupling & Status Indication**:
   * Low-ESR electrolytic capacitor ($100\ \mu\text{F} - 470\ \mu\text{F}$, $\ge 25\text{V}$) + high-frequency ceramic decoupling ($100\text{ nF}$).
   * Power-good indicator LED with current-limiting resistor sized for $\approx 10\text{ mA}$.

---

## Technical Deliverables
1. **KiCad 8.0 Schematic (`Protection_PDU.kicad_sch`)**:
   * Clean hierarchy, standardized net labels, correct `PWR_FLAG` placement.
   * Electrical Rules Check (ERC) passed with **0 errors and 0 warnings**.
2. **Engineering Calculation Sheet**:
   * P-MOSFET power dissipation at $5\text{A}$ ($P_{loss} = I^2 R_{DS(on)}$) vs equivalent Schottky diode loss.
   * Wire gauge selection and fuse rating coordination table.
   * Status LED current-limiting resistor calculation.
3. **Technical Report**:
   * Completed `Template_Report.md` submitted as a pull request.
