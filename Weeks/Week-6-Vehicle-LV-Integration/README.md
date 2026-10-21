# Week 6 — Vehicle LV Architecture & Shutdown Circuit (SDC)

[![Week](https://img.shields.io/badge/Week-6%20of%206-blue.svg)](#)
[![Focus](https://img.shields.io/badge/Focus-LV%20Architecture%20%7C%20Shutdown%20Circuit-brightgreen.svg)](#)
[![Task](https://img.shields.io/badge/Task-task--3--harness--sdc-orange.svg)](#)

Welcome to **Week 6** (Capstone Week) of the Apex Racing Team Electrical Low Voltage Onboarding Track.

---

## Weekly Objectives
1. **Formula Student EV Electrical Architecture**: Low-Voltage (LV) control system vs High-Voltage (HV) tractive system; galvanic isolation barriers.
2. **The Shutdown Circuit (SDC) Loop**: Series normally closed (NC) safety loop controlling accumulator isolation relays (AIRs).
3. **Safety Interlocks**: Cockpit Emergency Stop, External Emergency Stops, Inertia Switch ($6\text{g}$ mechanical), BSPD, IMD latch, and Brake Over-Travel Switch (BOTS).
4. **LV Charging & DC-DC Regulation**: Auxiliary charger connection, DC-DC converter regulation from HV to LV battery.
5. **Electrical-to-Embedded Integration**: Master ECU connector pinout tables, wire colors, signal matching, and documentation handoff.

---

## Daily Operational Guide & Curated Links

* **Day 1 (Monday) — Vehicle Electrical Architecture**:
  * 📺 [Formula Student EV Architecture Overview](https://www.youtube.com/watch?v=9X9Y1v2W3zA)
  * Draw high-level block diagram of vehicle LV subsystems (PDU, DAQ, ECU, Dashboard).
* **Day 2 (Tuesday) — Shutdown Circuit (SDC) Deep-Dive**:
  * 📺 [Formula Student Shutdown Circuit Design](https://www.youtube.com/watch?v=4Y9Z2v8W1xA)
  * Trace SDC loop; verify all switches are series NC and explain fail-safe behavior on wire break.
* **Day 3 (Wednesday) — Live Session: Task 3 Full Harness Integration**:
  * 45-min live session: Task 3 vehicle harness schematic and master ECU pinout documentation.
  * Task specifications: [`Tasks/Task-3-Harness-SDC/README.md`](../../Tasks/Task-3-Harness-SDC/README.md)
* **Day 4 (Thursday) — ECU Pinout Specification**:
  * 📺 [ECU Pinouts & Wire Schedule Spec](https://www.youtube.com/watch?v=6X7Z1v8W2yB)
  * Complete connector pinout schedule matching electrical harness wires to embedded firmware pins.
* **Day 5 (Friday) — Offline Workshop Day**:
  * Meet at team workshop: physical mock-up review of harness routing and bench testing the SDC loop.
  * Verify safety trip operation when each E-Stop and the inertia switch is tripped.
* **Day 6 (Saturday) — Final Capstone Deadline (Task 3)**:
  * Submit full Task 3 Capstone package: vehicle LV schematic + SDC loop + wire schedule + report by 11:59 PM.
* **Day 7 (Sunday) — Capstone Oral Code Defense**:
  * 15-minute 1-on-1 Capstone defense covering all 6 weeks of electrical curriculum.
