# Task 3 — Vehicle LV Wiring Harness & Shutdown Circuit (SDC)

[![Target](https://img.shields.io/badge/System-Vehicle%20Harness%20%7C%20SDC-blue.svg)](#)
[![Standards](https://img.shields.io/badge/Rules-Formula%20Student%20EV4-orange.svg)](#)
[![Milestone](https://img.shields.io/badge/Milestone-Capstone%20Task-brightgreen.svg)](#)

---

## Objective
The culmination of the 6-week Electrical Onboarding Track is the design of the **Vehicle Low-Voltage Wiring Harness** and the safety-critical **Shutdown Circuit (SDC) Loop**. You will produce an end-to-end electrical wiring schematic, an automotive harness assembly drawing, and a comprehensive master interconnect specification.

---

## Technical Specifications

### 1. Formula Student Shutdown Circuit (SDC)
The Shutdown Circuit is a hardware-interlocked safety loop that controls power to the tractive system accumulator isolation relays (AIRs). It must be wired strictly in **series normally closed (NC)** configuration:
1. **LV Master Switch (GLVMS)**: Main mechanical battery disconnect.
2. **Cockpit Emergency Stop**: Push-pull red mushroom switch accessible by the driver.
3. **Left & Right External Emergency Stops**: Mounted on the roll hoop / chassis sides.
4. **Inertia Switch (Crash Sensor)**: Mechanical g-force sensor ($6\text{g}$ rating) positioned rigidly on the chassis.
5. **Brake System Plausibility Device (BSPD)**: Hardware trip on hard braking while throttle is active.
6. **Insulation Monitoring Device (IMD) Relay**: Latched fault contact for HV tractive isolation degradation.
7. **Brake Over-Travel Switch (BOTS)**: Mechanical switch tripped if hydraulic brake pressure drops.

### 2. Vehicle Low-Voltage Wiring Harness
* **Architecture**: Star power distribution originating at the central PDU; central chassis Star Ground.
* **Cable Sizing & Types**:
  * Automotive thin-wall wire (FLRY-B or Spec 55).
  * Minimum wire gauge sizing based on ampacity and mechanical pull strength (minimum 22 AWG for signals, 16-18 AWG for actuators).
* **Connectors**:
  * Sealed Deutsch DT/DTM connectors for chassis transitions.
  * Automotive heatshrink boots (Raychem -25) and Raychem DR-25 diesel-resistant sleeving.
* **Electrical-to-Embedded Interface**:
  * Unified pinout schedule specifying connector, pin number, wire color, signal type, voltage, and destination MCU pin.

---

## Technical Deliverables
1. **Full Vehicle LV & SDC Schematic (`Vehicle_LV_Harness.kicad_sch`)**:
   * Complete wiring schematic showing power distribution, SDC loop, and sensor interconnects.
2. **Wiring Harness Schedule & Master BOM**:
   * Wire gauge selection table, circuit breaker/fuse schedule, and connector pinout matrix.
3. **Capstone Technical Report**:
   * Completed `Template_Report.md` documenting fail-safe operation and oral defense preparation.
