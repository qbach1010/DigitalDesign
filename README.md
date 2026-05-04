⚡ [Project Name]: Digital Design project
📝 Project Overview

Design a 3 bits signed (X) to 3 bits signed (Y) computer, which include operation add, subtract, multiply and XOR. User can select X, Y and operation to compute via switch. 

    EDA Tool: KiCad 10.0

    Dimensions: 120 x 180 mm

    Layer Count: 2 layers

    Primary MCU: Compute directly throughout logic gate AND (7400), OR (7432) and NOT (7404)

<img width="2616" height="1424" alt="image" src="https://github.com/user-attachments/assets/498dab5f-2e6c-457b-a0a1-c24644cecd59" />

📂 Repository Structure
KiCad library: Using standard library from KiCad

Plaintext

├── fab/                # Manufacturing files (Gerbers, Drill files, Pick & Place, CPL)
├── docs/               # PDF schematics, board renders, and datasheets
├── bom/                # Bill of Materials (.csv) and Interactive HTML BOM
├── [project].kicad_pro # KiCad project file
├── [project].kicad_sch # Main schematic file
└── [project].kicad_pcb # PCB layout file

🛠️ Key Hardware Features

Main functional blocks of your schematic.

    Power Supply: Using 7405 voltage regulator to power up the circuit, also is logic HIGH

    Adder: A simple 3 bits to 3 bit adder using full adder

    Two's Compliment: Changing sign of the 3 bit number, utilizing the adder to also do subtract

    Multiplier: Using Baugh-Wooley multiplication for multiplying signed 3 bits to signed 3 bits

    Sign Extend: Due to different between output of multiply operation (6 bits) and all other operation (3 bits), we add sign bit to make all the output 6 bits
    
🔍 Viewing the Design

    Quick View: A static PDF of the schematic is available in docs/schematic.pdf.

    Editing: Clone this repository and open the .kicad_pro file in KiCad.
