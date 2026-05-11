# ⚡ Digital Design Project

## 📝 Project Overview

Design a 3-bit signed (X) to 3-bit signed (Y) computer, which includes operations: add, subtract, multiply, and XOR. The user can select X, Y, and the operation to compute via physical switches. 

*   **EDA Tool:** KiCad 10.0
  
*   **Dimensions:** 120 x 180 mm
  
*   **Layer Count:** 2 layers
  
*   **Primary Logic:** Computes directly through discrete logic gates: AND (7400), OR (7432), and NOT (7404).
  
*   **Libraries Used:** Standard KiCad library.

### 📸 Schematics & Layout

<img width="800" alt="PCB Layout" src="https://github.com/user-attachments/assets/75363281-afc4-4d98-a97d-bf59b7ae0462" />

<img width="800" alt="Schematic Diagram" src="https://github.com/user-attachments/assets/498dab5f-2e6c-457b-a0a1-c24644cecd59" />

---

## 🛠️ Key Hardware Features
The main functional blocks of the schematic include:

*   **Power Supply:** Uses a 7805 voltage regulator to power up the circuit and provide the logic HIGH.
  
*   **Adder:** A simple 3-bit to 3-bit adder using full adders.
  
*   **Two's Complement:** Changes the sign of the 3-bit number, utilizing the adder block to also perform subtraction.
  
*   **Multiplier:** Uses **Baugh-Wooley multiplication** for multiplying the signed 3-bit numbers.
  
*   **Sign Extend:** Due to the difference between the output of the multiply operation (6 bits) and all other operations (3 bits), sign-extension logic is added to make all final outputs a uniform 6 bits wide.

---

## 🔍 Editing the Design
To view or modify the hardware files:

1. Clone this repository to your local machine.

2. Open the main `.kicad_pro` project file in **KiCad 10.0**.

