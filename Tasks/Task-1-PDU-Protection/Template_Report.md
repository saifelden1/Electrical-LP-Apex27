# Milestone Task 1 — Technical Report: PDU Input Protection

**Applicant Name**: ____________________  
**Sub-Team**: Electrical Systems (Low Voltage)  
**Date**: ____________________  
**Git Branch**: `task-1-pdu-protection`  

---

## 1. Schematic Architecture & Component Sizing

### 1.1 Fuse Selection & Wire Coordination
| Parameter | Selected Value / Part Number | Engineering Justification |
| :--- | :--- | :--- |
| **Nominal Bus Current** | `5.0 A` | Continuous design load |
| **Selected Fuse Rating** | ________ A | Margin above continuous current |
| **Upstream Wire Gauge** | ________ AWG / $mm^2$ | Ensures $I_{wire} > I_{fuse}$ |

### 1.2 Reverse Polarity P-Channel MOSFET
* **MOSFET Part Number**: ____________________
* **$R_{DS(on)}$ at $V_{GS} = -12\text{V}$**: ________ $m\Omega$
* **Calculated Power Loss ($P = I^2 R_{DS(on)}$)**: ________ W
* **Comparison**: How much power would a Schottky diode ($V_f \approx 0.45\text{V}$) dissipate at $5\text{A}$?
  * *Calculation*: __________________________________________________

### 1.3 TVS Transient Suppressor
* **TVS Part Number**: ____________________
* **Reverse Standoff Voltage ($V_{RWM}$)**: ________ V
* **Breakdown Voltage ($V_{BR}$)**: ________ V
* **Maximum Clamping Voltage ($V_C$)**: ________ V

---

## 2. KiCad ERC Verification
* Attach screenshot of KiCad 8.0 **Electrical Rules Check (ERC)** dialog showing **0 errors, 0 warnings**.

---

## 3. Challenges & Bug Diagnosis Log
* What errors or warnings appeared during your initial ERC run, and how did you resolve them?
* Why is a Zener diode necessary across the P-MOSFET Gate and Source?
