⚡ 3-Bit Signed Logic Gate Calculator

📝 Project Overview

This project is a discrete hardware calculator designed to perform arithmetic operations on two signed 3-bit inputs (X and Y). The system supports addition, subtraction, multiplication, and XOR operations, which the user can select via physical switches.

Rather than using a primary microcontroller, the computational logic is built entirely from the ground up using discrete 74-series logic gates: AND (7400), OR (7432), and NOT (7404).

Hardware Specifications:

    EDA Tool: KiCad 10.0

    Dimensions: 120 mm x 180 mm

    Layer Count: 2-Layer Board

    Libraries: Standard KiCad component libraries

📸 Schematics & Layout

 <img width="1790" height="1255" alt="image" src="https://github.com/user-attachments/assets/75363281-afc4-4d98-a97d-bf59b7ae0462" />


<img width="2616" height="1424" alt="image" src="https://github.com/user-attachments/assets/498dab5f-2e6c-457b-a0a1-c24644cecd59" /> 
🛠️ Key Hardware Features

The system is broken down into several core functional blocks:

    Power Supply: Utilizes a standard 7805 linear voltage regulator to step down the input voltage and provide a stable 5V logic HIGH for the circuit.

    Adder: A foundational 3-bit to 3-bit adder constructed using full adder logic.

    Two's Complement Subtraction: Inverts the sign of the 3-bit number and utilizes the main adder block to perform subtraction.

    Multiplier: Implements a 3x3 Baugh-Wooley multiplication architecture, specifically chosen for its efficiency in multiplying signed 2's complement binary numbers.

    Sign Extension: Because the multiplication operation yields a 6-bit output while other operations yield 3-bit outputs, standard sign-extension logic is applied to the 3-bit results. This ensures all final outputs sent to the display/output stage are uniformly 6 bits wide.

🔍 Viewing & Editing the Design

To explore the hardware files or modify the board:

    Clone this repository to your local machine.

    Open the main .kicad_pro project file using KiCad.
