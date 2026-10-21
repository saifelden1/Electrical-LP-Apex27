# Week 2 — Components & Power Switching (MOSFETs, Relays & E-Stop)

[![Week](https://img.shields.io/badge/Week-2%20of%206-blue.svg)](#)
[![Focus](https://img.shields.io/badge/Focus-Capacitors%20%7C%20MOSFETs%20%7C%20Relays-brightgreen.svg)](#)

Welcome to **Week 2** of the Apex Racing Team Electrical Low Voltage Onboarding Track.

---

## Weekly Objectives
1. **Passive Energy Storage**: Capacitors (ceramic vs electrolytic, ESR, voltage derating), Inductors and back-EMF ($V = -L \frac{di}{dt}$).
2. **Electromechanical Switching**: Automotive relays (coil voltage, contact ratings, NO/NC), flyback diode protection.
3. **Solid-State Switching**: N-Channel vs P-Channel Power MOSFETs, gate threshold voltage ($V_{GS(th)}$), on-resistance ($R_{DS(on)}$), gate charging.
4. **Safety Switches**: Emergency Stop (E-Stop) switches, fail-safe normally closed (NC) operation, pull-up/pull-down resistor sizing.
5. **KiCad Library Design**: Creating custom schematic symbols (`.kicad_sym`) and associating PCB footprints (`.kicad_mod`).

---

## Daily Operational Guide & Curated Links

* **Day 1 (Monday) — Capacitors & Inductive Flyback**:
  * 📺 [Capacitor Types, Filtering & ESR](https://www.youtube.com/watch?v=f_MZNsEqyQw)
  * 📺 [Automotive Relays & Flyback Diodes](https://www.youtube.com/watch?v=k5_a1Z_L46s)
  * Calculate inductor back-EMF spike suppression diode ratings.
* **Day 2 (Tuesday) — Power MOSFET Switching**:
  * 📺 [MOSFETs as Switches & Gate Driving](https://www.youtube.com/watch?v=GrvvkYTW_0k)
  * Compare BJT vs MOSFET power dissipation; select logic-level N-MOSFET for a 12V / 5A fan.
* **Day 3 (Wednesday) — Live Session: Custom KiCad Libraries**:
  * 45-min live session: creating custom symbols and assigning footprints in KiCad 8.0.
  * 📺 [KiCad Custom Symbols & Footprints](https://www.youtube.com/watch?v=ZbhwG7eqvB8)
* **Day 4 (Thursday) — E-Stop & Control Circuits**:
  * 📺 [Emergency Stop Switch Wiring Standards](https://www.youtube.com/watch?v=8XJ9G2V8X3Y)
  * Draft schematic for MOSFET high-side/low-side load switch with gate pull-down.
* **Day 5 (Friday) — Offline Workshop Day**:
  * Meet mentor at team lab: wire a MOSFET circuit on breadboard to switch a 12V load.
  * Measure gate threshold and check switching cold performance.
* **Day 6 (Saturday) — Week 2 Submission**:
  * Submit MOSFET schematic + relay/MOSFET selection calculation sheet by 11:59 PM.
* **Day 7 (Sunday) — Friendly 1-on-1 Oral Check-in**:
  * 10-minute check-in: explain $V_{GS(th)}$, $R_{DS(on)}$ thermal heating, and flyback diode placement.
