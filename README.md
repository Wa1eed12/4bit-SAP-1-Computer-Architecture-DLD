#  SAP-1 Computer Architecture (Digital Logic Design)

## Project Overview
This project implements a 4-bit SAP-1 (Simple-As-Possible-1) computer architecture using fundamental digital logic components.

The system demonstrates how a basic CPU works internally, including:
- Instruction Fetch–Execute Cycle
- Hardwired Control Unit
- ALU-based arithmetic operations
- Shared system bus architecture

---

##  Architecture Components

###  Datapath
- Register A (Accumulator)
- Register B
- Memory Address Register (MAR)
- Program Counter (74LS161)
- Instruction Register
- Output Register
- Shared 4-bit Bus
- Tri-state Buffers (74LS244)

###  Processing Unit
- 4-bit ALU (74HC181)
- ADD and SUB operations

###  Memory System
- 6116 Static RAM (Used as 16×4 memory)
- Manual opcode loading (current stage)

###  Control Unit
- Hardwired Control Logic
- Program Sequencer (T-States)
- Opcode Decoder (74LS138)

---

## Implemented Instructions

| Instruction | Operation |
|------------|-----------|
| ADD | A ← A + B |
| SUB | A ← A − B |

---

##  Instruction Cycle

### Fetch Cycle
T1 – PC → MAR  
T2 – PC Increment  
T3 – RAM → Instruction Register  

### Execute Cycle
T4 – Load Operand  
T5 – ALU Operation  
T6 – Store Result  

---

##  Simulation

- Designed and simulated in Proteus
- Verified:
  - Correct timing states
  - No bus contention
  - Accurate ALU results
  - Stable output display

---

##  Cost Analysis
Estimated hardware cost ≈ 6,950 PKR

---

## Technologies Used
- Digital Logic Design
- TTL / CMOS ICs
- 74HC181 ALU
- 6116 SRAM
- 74LS161 Counter
- 74LS138 Decoder
- 74LS74 Flip-Flops
- Proteus Simulation

---

## Learning Outcomes
- CPU architecture understanding
- Datapath & Control separation
- Hardwired control design
- Bus-based system design
- Timing state management
- Digital system debugging

---

##  Author
Waleed Asif  
Mechatronics Engineering Student  
Air University
