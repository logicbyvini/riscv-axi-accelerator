# riscv-axi-accelerator
RISC-V AXI Accelerator
This project implements an ASIC architecture designed to accelerate matrix inversion operations and convolutional neural networks (CNNs), fully integrated with a RV32 RISC-V processor.
The communication between the processor and the hardware accelerators is achieved through an AXI4/AXI4-Lite bus, allowing seamless integration within a SoC (System-on-Chip) environment.
Main Components:
Matrix Inversion Unit optimized for hardware implementation.
CNN Accelerator with configurable parameters.
Functional Control and Cost Unit for resource management.
AXI4-Lite Interface for control and data access.
Development Flow:
Reference modeling in Python for algorithmic validation.
Translation to C/C++ for software-level simulation and performance analysis.
Final implementation in Verilog for RTL synthesis and ASIC/FPGA integration.
Software and Toolchain:
Ripes and RARS for RISC-V architecture exploration and simulation.
xPack and GCC Toolchains for RISC-V cross-compilation.
Lattice Diamond for FPGA prototyping and synthesis.
Cadence Xcelium and Cadence Genus for RTL simulation and synthesis.
Vivado for FPGA testing and verification.
Technologies and Objectives:
The goal of this project is to design a modular and efficient hardware acceleration platform capable of executing mathematical and AI workloads directly on silicon.
It combines principles of digital microelectronics, computer architecture, and signal processing to create a scalable ASIC/FPGA-ready solution for future RISC-V SoC designs.
