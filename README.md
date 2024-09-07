# 4-Bit-ALU

Designed and tested a simplified 4 Bit ALU on Cadence Virtuoso. 
Some highlights of the project:

A) Operations capable of performing-
 1) Addition
 2) Subtraction
 3) XOR
 4) Barrel Shift right.
 Addition and subtraction are in 2's compliment. Kogge-Stone Adder used.

B) Successfully performed DRC,LVS and quantus QRC extraction.

C) Final layout area within 150% of total cell area.

D) Calculated setup time and critical path delay for 700mV and 1.2V.

E) Calculated Maximum frequency of operation for 700 mV and 1.2V.

F) Steps taken to optimise :
 1)Area- Cells laid out in placement rows.
 2)Power- Data gating employed.
 3)Delay- Used buffers to bring down the fan-out from 8 to 4 and increasing signal strength.
 
G) 4 metal layers used.

My contributions- 
1) Designing and testing entire circuit on logisim.
2) Building schematic and layout of adder block. 
3) Building schematic and layout of the ALU block (Only combinational logic included).
4) Performing DRC and LVS tests on my designed blocks. Also performed testing.
5) Contributed in Project Report Preparation.

Final Reaults: 

1) Realisation area = 440.08 um^2.
2) Critical path delay for 1.2V = 4.545 ns.
3) Critical path delay for 0.7V = 22.34 ns.
4) Setup time for 1.2V = 0.1214 ns.
5) Setup time for 0.7V = 0.2451 ns.
6) Maximum Frequency for 1.2V = 114.5 MHz.
7) Maximum Frequency for 0.7V = 24 MHz

Files containing the project details are attached for perusal.
