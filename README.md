# 4-Bit-ALU

Designed and tested a simplified 4 Bit ALU on Cadence Virtuoso. 
Some highlights of the project:

A) Operations capable of performing-
 1) Addition
 2) Subtraction
 3) XOR
 4) Barrel Shift right.
    
 Addition and subtraction are in 2's compliment. Parallel Prefix adder used: Kogge-Stone adder.

B) Successfully performed DRC, LVS and quantus QRC extraction.

C) Final layout area within 150% of total cell area.

D) Calculated setup time and critical path delay for 700mV and 1.2V.

E) Calculated Maximum frequency of operation for 700 mV and 1.2V.

F) Steps taken to optimise :

 1) Area- Cells laid out in placement rows.
 2) Power- Data gating employed.
 3) Delay- Used buffers to bring down the fan-out from 8 to 4 and increase signal strength.
 
G) 4 metal layers used.

My contributions- 
1) Designing and testing the circuit on logisim.
2) Building schematic and layout of the adder block. 
3) Building schematic and layout of the ALU block (Combinational logic).
4) Performed DRC, LVS and functional testing on my designed blocks.
5) Contributed in Project Report Preparation.

Final Results: 

1) Layout realisation area = 440.08 um^2.
2) Critical path delay for 1.2V = 4.545 ns.
3) Critical path delay for 0.7V = 22.34 ns.
4) Setup time for 1.2V = 0.1214 ns.
5) Setup time for 0.7V = 0.2451 ns.
6) Maximum Frequency for 1.2V = 114.5 MHz.
7) Maximum Frequency for 0.7V = 24 MHz

Files containing the project details are attached for perusal.

Block diagram of the ALU:

 <p align="center">
  <img src="https://github.com/rahulsaxena8/4-Bit-ALU/blob/Images/ALU_BlockDiagram.png" width="800"/>
</p>

The ALU accepts a 5-bit opcode.

 <p align="center">
  <img src="https://github.com/rahulsaxena8/4-Bit-ALU/blob/Images/OpCode.png" width="800"/>
</p>

Op4 determines if there is a feedback. 0 for external input and 1 for feedback.

Op3 and Op2 determine the ALU operation. 00 for Addition, 01 for Subtraction, 10 for XOR, and 11 for Barrel-Shift.

Op1 and Op0 determine the shift produced by the Barrel-Shifter. 00 for shift 4, 01 for shift 1, 10 for shift 2, and 11 for shift 3. 

Testing the circuit on logisim:

 <p align="center">
  <img src="https://github.com/rahulsaxena8/4-Bit-ALU/blob/Images/Logisim_alu.png" width="800"/>
</p>

Inside the ALU block:

 <p align="center">
  <img src="https://github.com/rahulsaxena8/4-Bit-ALU/blob/Images/Logisim_alu-inside.png" width="800"/>
</p>

Complete floorplan:

 <p align="center">
  <img src="https://github.com/rahulsaxena8/4-Bit-ALU/blob/Images/FloorPlan.png" width="800"/>
</p>

4-bit register schematic and layout:

 <p align="center">
  <img src="https://github.com/rahulsaxena8/4-Bit-ALU/blob/Images/4_bit_xor.png" width="400"/>
  <img src="https://github.com/rahulsaxena8/4-Bit-ALU/blob/Images/4_bit_xor_Layout.png" width="400"/>
</p>

Full Layout of the 4-Bit ALU:

 <p align="center">
  <img src="https://github.com/rahulsaxena8/4-Bit-ALU/blob/Images/Full_Layout.png" width="800"/>
</p>



