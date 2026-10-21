# Milestone Task 2 — Technical Report: Sensor DAQ PCB

**Applicant Name**: ____________________  
**Sub-Team**: Electrical Systems (Low Voltage)  
**Date**: ____________________  
**Git Branch**: `task-2-daq-pcb`  

---

## 1. Signal Conditioning Calculations

### 1.1 Voltage Divider Scaling (5V to 3.3V)
* **$R_1$ (High-Side)**: ________ $k\Omega$
* **$R_2$ (Low-Side to GND)**: ________ $k\Omega$
* **Calculated Maximum Output Voltage ($V_{out} = 5.0\text{V} \times \frac{R_2}{R_1 + R_2}$)**: ________ V

### 1.2 RC Low-Pass Filter Design
* **Filter Resistor ($R_f$)**: ________ $\Omega$
* **Filter Capacitor ($C_f$)**: ________ $\mu\text{F} / \text{nF}$
* **Calculated Cutoff Frequency ($f_c = \frac{1}{2\pi R C}$)**: ________ Hz

---

## 2. PCB Layout & IPC-2152 Verification
| Net / Trace Type | Current (A) | Trace Width (mm) | Temperature Rise (deg C) |
| :--- | :--- | :--- | :--- |
| **+12V Battery Input** | ________ A | ________ mm | $< 10^\circ\text{C}$ |
| **+5V Sensor Rail** | ________ A | ________ mm | $< 10^\circ\text{C}$ |
| **Analog Signals** | $< 1\text{ mA}$ | ________ mm | Negligible |

---

## 3. KiCad DRC Verification & 3D Render
* Attach screenshot of KiCad 8.0 **Design Rules Check (DRC)** showing **0 errors, 0 unrouted nets**.
* Attach top and isometric 3D renders of your routed PCB.
