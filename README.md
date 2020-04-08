# VerilogCPU
ARMv8 Processor written in Verilog

NOTE: Certain files are missing and unrecoverable due to being in my university's student VM, which is now gone. This project was a college assignment and I am very unlikely to revisit it. The files that are present are complete.

* Doubleword registers
* Supports data forwarding
* Detects data hazards and stalls

Opcodes Supported:
ADD
ADDI
SUB
SUB
AND
ORR
CBZ
CBNZ
B
LDUR
STUR

Primary Files Included:
* CPU.v -- Main data pipeline
* ControlUnit.v -- Interprets opcode control signals
* ALUcontrol.v -- Produces control signals for main ALU
* ALU.v -- Executes arithmetic and logical operations for R, I, and D-type instructions
* HazardDetectionUnit.v -- Detects data hazards and outputs stall signal if necessary
* SignExtensionUnit.v -- Performs sign extension for B, CB, I, and D-type instructions

Test Benches:
* CPU_tb.v
* ALUControl_tb.v
* SignExtension_tb.v
