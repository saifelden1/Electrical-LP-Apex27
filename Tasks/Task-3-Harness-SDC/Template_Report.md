# Milestone Task 3 — Technical Report: Vehicle LV Harness & SDC

**Applicant Name**: ____________________  
**Sub-Team**: Electrical Systems (Low Voltage)  
**Date**: ____________________  
**Git Branch**: `task-3-harness-sdc`  

---

## 1. Shutdown Circuit (SDC) Loop Architecture
Trace the current flow through your SDC loop from the $+12\text{V}$ battery rail to the final shutdown relay coil:
```
+12V Battery -> [GLVMS] -> [Cockpit E-Stop] -> [Left E-Stop] -> [Right E-Stop] -> [Inertia Sw] -> [BOTS] -> [BSPD] -> [IMD Latch] -> Shutdown Relay Coil -> GND
```
* Explain why every element must be wired in **Series Normally Closed (NC)**:
  * *Explanation*: __________________________________________________

---

## 2. Master Connector & ECU Interface Schedule
| Connector ID | Pin # | Wire Color | Signal Name | Voltage Level | Wire Gauge | Destination Subsystem |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **CONN_ECU** | 1 | RED | +12V_LOGIC | 12V DC | 18 AWG | Master ECU Power |
| **CONN_ECU** | 2 | BLK | GND_POWER | 0V | 18 AWG | Star Ground Block |
| **CONN_ECU** | 3 | BLU | SENS_THROTTLE_1 | 0.5V - 4.5V | 22 AWG | TPS Sensor 1 |
| **CONN_ECU** | 4 | WHT | CAN_HIGH | Differential | 24 AWG (STP) | Vehicle CAN Bus |
| **CONN_ECU** | 5 | GRN | CAN_LOW | Differential | 24 AWG (STP) | Vehicle CAN Bus |

---

## 3. Harness Fabrication & Crimp Verification
* Attach photos/documentation of your physical crimp pull-test or mock-up assembly.
* What heatshrink sleeving and strain-relief measures are used at high-vibration chassis points?
