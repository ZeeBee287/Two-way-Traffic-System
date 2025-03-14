# 🚦 Two-Way Traffic System (Multisim Design)

## 📌 Overview
This project implements a **two-way traffic signal control system** using **logic gates** and **D flip-flops** in **Multisim**. The design simulates a traffic signal controlling two roads at an intersection, ensuring smooth traffic flow through alternating red, yellow, and green signals.

## 🎯 Objective
The goal is to design a **traffic signal system** using **combinational logic circuits** and **flip-flops** to regulate traffic flow efficiently at an intersection.

## 🛠️ Equipment & Software
- **Multisim Software**
- **Logic Gates:** NOT, XOR, NAND, AND gates
- **Flip-Flops:** D flip-flops (7474N)
- **Traffic Light Indicators**
- **Switches & Power Sources**

## 🔧 Design & Implementation
The traffic system follows a **four-phase sequence**:
1. **Road 1 Green, Road 2 Red** → Road 1 is open while Road 2 is stopped.
2. **Road 1 Yellow, Road 2 Red** → Warning before Road 1 stops.
3. **Road 1 Red, Road 2 Green** → Road 1 stops, Road 2 opens.
4. **Road 1 Red, Road 2 Yellow** → Warning before Road 2 stops.

### **Logic Expressions Used:**
Boolean expressions were used to determine traffic light behavior:
- **A̅ = A̅B + AB̅ = A ⊕ B**
- **B̅ = B̅t + A̅B̅ x̅y + AB̅xy̅**
- **Output Logic:**
  - Red1 = A̅B̅, Yellow1 = A̅B, Green1 = A
  - Red2 = AB̅, Yellow2 = AB, Green2 = A̅

## 📌 Procedure in Multisim
1. Open **Multisim** and place components:
   - Logic gates (74LS04N, 74LS86N, 74LS00N, 74LS10N, 74LS08N)
   - Flip-flops (7474N)
   - Traffic light signals
2. Connect **power sources** (VCC, GND, Clock Voltage).
3. Configure **switches** for manual input.
4. Implement **logic circuit wiring** based on Boolean expressions.
5. Attach **probes** to traffic light signals for output verification.
6. **Run the simulation** to test traffic light transitions.

## 🔬 Observations
- The system successfully controls traffic flow as expected.
- Inputs trigger **correct light transitions** based on **flip-flop states**.
- Traffic lights function in a **cyclic manner**, ensuring smooth alternation between roads.

## 🏁 Conclusion
The **two-way traffic system** was successfully implemented using **logic gates and flip-flops** in **Multisim**. The system accurately followed the four-phase sequence, validating the Boolean expressions and logical design.

📂 **Project Files Included:**
- **Multisim Design File (`.ms12`)** – Full circuit schematic.
- **Simulation Screenshots** – Captures of the working model.
- **Project Report (`.pdf`)** – Detailed documentation.

🚀 Feel free to explore and modify the design! 😊
