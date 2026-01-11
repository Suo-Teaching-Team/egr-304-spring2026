# **EGR 304 — Lab 1**
## **Power Supplies, Voltage Regulators, and Schematic Design**

> This lab combines **ICC1** and **HW1** into a **single integrated lab**.  
> You may work with **one partner** during construction and analysis, but **all demonstrations and schematics must be your own**.

---

## **Lab Objectives**

By completing this lab you will demonstrate proficiency in:

1. Designing an adjustable **5V linear voltage regulator** using the **LM317**
2. Using **datasheets** to determine safe operating conditions
3. Using a **benchtop power supply**
4. Using a **digital multimeter (DMM)** to measure voltage and current
5. Creating a **professional ECAD schematic** (KiCad or Cadence)
6. Creating a **custom symbol library and regulator symbol**

---

## **Tools & Software**

You may use:
- **KiCad** (recommended)
- **Cadence** (optional)

Install the EGR304 software stack:  
https://embedded-systems-design.github.io/egr304-software-stack/

---

## **Hardware & Parts**

| Item | Quantity |
|------|---------|
| Breadboard | 1 |
| Jumper wires | Many |
| LM317BT adjustable regulator | 1 |
| 1N4007 diodes | 2 |
| 0.1 µF ceramic capacitor | 1 |
| 10 µF electrolytic capacitor | 1 |
| 1 µF tantalum capacitor | 1 |
| 2 kΩ resistor | 1 |
| 10 kΩ potentiometer | 1 |
| 5.1 Ω 10 W power resistor | 1 |
| Fixed resistors (for final design) | as needed |

---

## **Pre-Lab Preparation**

Using the LM317 datasheet:

1. Find the **maximum allowed**  
   \( V_{in} - V_{out} \)

2. Using the **dropout voltage**, determine the **minimum input voltage** needed to maintain:
   \[
   V_{out} = 5V
   \]

3. Find the **minimum output current** and compute the resistor required from output to ground to guarantee it.

You will need this resistor in your circuit.

---

## **Part A — Build the Regulator**

1. Build the LM317 regulator on a breadboard based on the datasheet’s Figures 6 & 7.
2. Add:
   - Input and output capacitors
   - Two protection diodes
   - Minimum load resistor
3. Use a **potentiometer** to adjust the output to **5.00 V**

---

## **Part B — Electrical Measurements**

Using the **BK Precision Power Supply** and **Agilent DMM**:

1. Verify the power supply voltage with the DMM
2. Measure:
   - Regulator **input voltage**
   - Regulator **output voltage (no load)**
3. Adjust the potentiometer to get **5.00 V**
4. Turn off power
5. Add the **5.1 Ω load resistor**
6. Turn on power
7. Measure:
   - Loaded output voltage
   - Load current (briefly — parts will get hot)

---

## **Part C — Lock in 5V**

1. Measure the potentiometer resistance that produced 5.00 V
2. Remove the potentiometer
3. Replace it with **fixed resistors** that give the same resistance
4. Re-verify the output is still **5.00 V**

This is the circuit you will document in ECAD.

---

## **Part D — ECAD Schematic**

Create a professional schematic using **KiCad or Cadence**.

You must:

1. Create a **custom symbol library**
   - Must include **your initials** in the filename
2. Create a **custom LM317 symbol**
   - Must include **your initials** in the symbol name
3. Draw the full regulator circuit
   - Using **actual resistor values**
   - Including diodes, capacitors, and minimum load resistor
4. Use:
   - `R_US`, `C_US`, `C_Polarized_US`
   - **Earth ground**, not GND
5. Check against:  
   https://embedded-systems-design.github.io/schematic-checklist/

---

## **Part E — Live Demonstration**

Individually demonstrate to the teaching staff:

1. Completed breadboard
2. **5.00 V** no-load output
3. **5.00 V** loaded output (5.1 Ω)
4. Correct ECAD schematic and custom symbol

No late demonstrations accepted.

---

## **Canvas Submission**

Submit:

1. **PDF** of your schematic  
2. **ZIP file** containing:
   - Project files
   - Custom symbol library

Follow packaging instructions:  
- KiCad: https://embedded-systems-design.github.io/packaging-kicad-files-for-submission/  
- Cadence: https://embedded-systems-design.github.io/packaging-cadence-files-for-submission/

---

## **Grading (Total = 350 pts)**

| Item | Points |
|------|-------|
| Breadboard built correctly | 35 |
| 5V no-load measurement | 50 |
| 5V loaded measurement | 50 |
| Custom symbol library | 25 |
| Custom LM317 symbol | 25 |
| Accurate schematic | 140 |
| PDF submission | 25 |
| **Total** | **350** |

---
