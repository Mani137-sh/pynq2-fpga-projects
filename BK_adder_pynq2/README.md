# BK Adder (Brent–Kung Adder) on Pynq-Z2

This project implements a **32-bit Brent–Kung (BK) parallel prefix adder** optimized for FPGA deployment on the **Pynq-Z2** board.  
The design is lightweight, fast, and synthesizable in Vivado.

## 🚀 Project Contents
- Verilog implementation of 32-bit Brent–Kung Adder
- Optional Add/Sub wrapper logic
- Constraint file (XDC) for Pynq-Z2
- Vivado project setup for synthesis & implementation
- Bitstream (.bit) and hardware definition (.hwh)
- Documentation and design notes

## 📁 Folder Structure
```
BK_adder_pynq2/
│── src/          # Verilog RTL, top module, and XDC file
│── bitstreams/   # .bit and .hwh files for Pynq-Z2
│── docs/         # Notes, diagrams, block architecture
└── README.md
```

## 🧩 Design Overview
The **Brent–Kung adder** is a parallel-prefix adder designed for:
- Logarithmic delay
- Reduced fan-out
- Low FPGA resource usage
- Balanced prefix tree structure

It computes:
- Propagate: p = A ^ B
- Generate: g = A & B
- Carries through a multi-level prefix network

## 🛠 How to Use in Vivado
1. Open Vivado  
2. Create a new RTL project  
3. Add all Verilog files from `src/`  
4. Add the Pynq-Z2 `.xdc` constraint file  
5. Run Synthesis  
6. Run Implementation  
7. Generate Bitstream  
8. Export `.bit` and `.hwh` to the `bitstreams/` folder

## 📌 Summary
This project provides:
- A clean 32-bit Brent–Kung adder implementation  
- FPGA-ready RTL  
- Constraints and bitstreams for Pynq-Z2  
- Modular, extensible design suitable for learning and experimentation

