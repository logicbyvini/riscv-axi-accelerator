# RISC-V AXI Accelerator

**RISC-V AXI Accelerator** is an ASIC-oriented hardware design project that integrates a **RV32 RISC-V processor** with specialized **AXI4/AXI4-Lite accelerators** for computationally intensive tasks such as **matrix inversion** and **convolutional neural networks (CNNs)**.

This project explores the co-design of digital hardware and software to create a scalable and efficient hardware acceleration framework for mathematical and AI workloads, following an end-to-end development flow — from high-level modeling to RTL implementation and FPGA prototyping.

---

## 🔧 Architecture Overview

The architecture is composed of the following main modules:

- **RV32 RISC-V Core** — a 32-bit custom RISC-V processor serving as the system controller and host interface.
- **AXI4/AXI4-Lite Interconnect** — handles communication between the RISC-V core and hardware accelerators, supporting high-throughput data transfer and lightweight control registers.
- **Matrix Inversion Accelerator** — a dedicated hardware unit optimized for real-time matrix inversion using parallel arithmetic pipelines and reduced latency datapaths.
- **CNN Accelerator** — a modular processing engine for convolutional layers, supporting configurable kernel sizes, stride, and activation functions.
- **Functional Control Unit** — manages synchronization, cost evaluation, and scheduling between compute units.
- **Memory Subsystem** — AXI-compatible RAM and buffer modules designed for high-speed data access and low-power operation.

---

## 🧠 Development Flow

The design process follows a progressive abstraction methodology:

1. **Algorithmic Modeling (Python)**  
   - Functional validation of matrix inversion and CNN kernels.  
   - Floating-point and fixed-point arithmetic analysis.  

2. **Software-Level Simulation (C/C++)**  
   - Algorithm refinement for hardware translation.  
   - Integration testing using RISC-V toolchains (xPack, GCC, RARS, Ripes).  

3. **RTL Design (Verilog)**  
   - Implementation of arithmetic datapaths, AXI interfaces, and control logic.  
   - Verification through behavioral and gate-level simulation (Cadence Xcelium).  

4. **Synthesis and Prototyping**  
   - Logic synthesis using **Cadence Genus** and **Lattice Diamond**.  
   - FPGA-level verification and timing analysis using **Vivado**.  

---

## ⚙️ Tools and Environments

| Category | Tools |
|-----------|-------|
| **EDA / Simulation** | Cadence Xcelium, Cadence Genus, Lattice Diamond, Vivado |
| **RISC-V Toolchains** | xPack GCC, RARS, Ripes |
| **Languages** | Verilog (RTL), Python (modeling), C/C++ (software co-simulation) |
| **Prototyping** | Lattice FPGA boards for hardware validation |

---

## 📐 Design Objectives

- Develop a **fully synthesizable ASIC prototype** integrating RV32 core and accelerators.  
- Implement **hardware-level AXI4 communication** with minimal latency overhead.  
- Achieve **parallel computation** for matrix inversion and CNN layers.  
- Support **scalable architectures** for future expansion (FFT, DSP, ML kernels).  
- Enable **hardware/software co-design** and RISC-V integration testing via open toolchains.

---

## 📊 Expected Outcomes

- High-performance hardware accelerator for AI and numerical computation.  
- Open-source RTL modules ready for SoC integration.  
- Reference designs for educational and research use in **RISC-V based hardware acceleration**.  

---

**Keywords:** ASIC Design · RISC-V · AXI4 · Hardware Accelerator · CNN · Matrix Inversion · Verilog · SoC · FPGA Prototyping · Hardware/Software Co-Design
