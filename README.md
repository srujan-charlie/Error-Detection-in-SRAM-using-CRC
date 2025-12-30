🧠 Project Overview

This project presents a hardware-level error detection architecture for SRAM using Cyclic Redundancy Check (CRC) integrated with a Finite State Machine (FSM) and content validation logic.
The design focuses on data integrity assurance during memory write and read operations on an FPGA platform.

🧩 Architecture Highlights

CRC Module for detecting data corruption before memory access

FSM Controller to manage sequencing of CRC check, write, and read operations

SRAM Interface that allows memory access only for CRC-validated data

Parallel Validation Logic to ensure correctness of stored and retrieved data

🖥️ FPGA Validation

The design is functionally verified and synthesized using Xilinx Vivado with:

Correct CRC validation across write/read cycles

Accurate FSM state transitions

Successful behavioral and post-implementation timing verification

Efficient utilization of FPGA resources (LUTs, FFs, I/O)

(Waveform and utilization snapshots are provided in this repository for reference.)

🛠️ Tools & Technologies

HDL: Verilog

FPGA Toolchain: Xilinx Vivado

Target Board: Basys-3 FPGA

Verification: Behavioral & post-synthesis timing simulation

🖼️ Demonstration

This repository includes:

📊 Timing waveform screenshots showing CRC validation and memory control flow

📈 FPGA utilization reports highlighting efficient hardware mapping

📌 Note: Source code is not publicly shared by default.

🔒 Code Access

The complete RTL and project files are available upon request.

If you are interested in:

Studying the architecture

Reusing the design for academic or research purposes

Extending the system (ECC, multi-bank SRAM, low-power techniques)

📩 Please raise an issue or contact via GitHub with a brief description of your use case.

⚠️ Most Challenging Aspect

Ensuring synchronous coordination between CRC validation, FSM control, and memory access without introducing false writes or read hazards required careful state sequencing and timing analysis, especially during post-implementation verification.

🌱 Possible Extensions

Error correction mechanisms (ECC)

Parameterized SRAM and data width

Power optimization using clock gating

Integration with larger memory subsystems
