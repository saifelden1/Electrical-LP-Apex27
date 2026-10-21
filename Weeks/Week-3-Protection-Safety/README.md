# Week 3 — Circuit Protection, Wire Coordination & Safe Testing

[![Week](https://img.shields.io/badge/Week-3%20of%206-blue.svg)](#)
[![Focus](https://img.shields.io/badge/Focus-Fuses%20%7C%20Wire%20Sizing%20%7C%20TVS-brightgreen.svg)](#)
[![Task](https://img.shields.io/badge/Task-task--1--pdu--protection-orange.svg)](#)

Welcome to **Week 3** of the Apex Racing Team Electrical Low Voltage Onboarding Track.

---

## Weekly Objectives
1. **Automotive Fusing**: Short circuits, melting $I^2 t$, fuse types (ATO, Mini, MIDI), fast-acting vs slow-blow.
2. **Wire & Fuse Coordination**: The cardinal safety rule: wire ampacity must always exceed fuse rating ($I_{wire} > I_{fuse}$).
3. **Wire Gauge Selection**: AWG and $mm^2$, conductor resistance, temperature derating (automotive FLRY-B cable).
4. **Transient & Reverse Protection**: Reverse battery connection protection (P-Channel MOSFET ideal diode), TVS transient clamping diodes.
5. **Grounding & Testing**: Star grounding vs ground loops; safe testing procedures using current-limited bench power supplies.

---

## Daily Operational Guide & Curated Links

* **Day 1 (Monday) — Fuses & Wire Sizing**:
  * 📺 [Automotive Fusing & Coordination](https://www.youtube.com/watch?v=yY3k9pBf0tE)
  * 📺 [Wire Gauge Sizing & Ampacity](https://www.youtube.com/watch?v=hZzM9T3V7q8)
  * Size wire gauge and fuse rating for a $15\text{A}$ vehicle branch circuit.
* **Day 2 (Tuesday) — Reverse Polarity & TVS Diodes**:
  * 📺 [Reverse Polarity Protection (Diode vs P-MOSFET)](https://www.youtube.com/watch?v=IrB-FPcv1Dc)
  * 📺 [TVS Diodes for Load Dump Transients](https://www.youtube.com/watch?v=wX1C5Q9H4cQ)
  * Calculate power loss of P-MOSFET vs Schottky diode at $5\text{A}$.
* **Day 3 (Wednesday) — Live Session: Task 1 PDU Protection**:
  * 45-min live session: complete walkthrough of Task 1 input protection schematic in KiCad 8.0.
  * Task specifications: [`Tasks/Task-1-PDU-Protection/README.md`](../../Tasks/Task-1-PDU-Protection/README.md)
* **Day 4 (Thursday) — Star Grounding & ERC**:
  * 📺 [Star Grounding & Eliminating Ground Loops](https://www.youtube.com/watch?v=2K2Q8v9W5sA)
  * Complete KiCad schematic and verify 0 ERC errors.
* **Day 5 (Friday) — Offline Workshop Day**:
  * Meet at team workshop: test reverse polarity circuit on current-limited bench supply.
  * Verify P-MOSFET blocks reverse voltage with zero damage.
* **Day 6 (Saturday) — Milestone Task 1 Submission**:
  * Submit Task 1 deliverable: KiCad schematic + calculation sheet + report by 11:59 PM.
* **Day 7 (Sunday) — Friendly 1-on-1 Oral Check-in**:
  * 10-minute check-in: explain why $I_{wire} > I_{fuse}$ and how TVS diodes clamp inductive spikes.
