# GLADE-FullAdder

This repository contains the design and simulation of a **CMOS-based full adder circuit**. The circuit is built using **XOR, AND, OR gates, and an inverter**. The design has been verified through **DRC, LVS, and LPE tests**, ensuring correctness and manufacturability. Simulations were performed using **Spice3**, including an additional all-NAND implementation for comparative analysis.

## Circuit Design w/ GLADE
A full adder circuit takes three inputs, two operands and carry in, and produces two outputs, the sum and carry out.
Each gate follows three design stages: schematic, stick diagram, and layout.

**Inverter (NOT Gate)**
 : A simple CMOS circuit with a PMOS and an NMOS. When input is high, output is low, and vice versa. The stick diagram visualizes gate connections, and the layout arranges active regions, poly, and metal layers.
<p float="center">
  <img src="https://github.com/user-attachments/assets/fa87eb55-37ea-489a-9013-bb28414428af"  width = 25% />
  <img src="https://github.com/user-attachments/assets/4d23b754-c343-42a6-9277-325f04479284" width=15.5% /> 
  <img src="https://github.com/user-attachments/assets/7301e619-54c0-4530-aa55-ad7c652511bd" width=22% /> 
</p>

**AND Gate**
 : Implemented directly using CMOS logic with the PUN having same function with inverted inputs (series connection) and PDN having inverted function (parallel connection). The layout ensures minimal delay and optimized power consumption following the stick diagram.
<p float="center">
  <img src="https://github.com/user-attachments/assets/0e386175-d050-45e9-9704-d71983bf6a17" width = 25% />
  <img src="https://github.com/user-attachments/assets/0036b20c-b081-4f2b-ba1a-58f41c008d05" width=20.6% /> 
  <img src="https://github.com/user-attachments/assets/3d553384-46ab-4144-b15a-0bae03612621" width=15% /> 
</p>

**OR Gate** 
 : Designed using standard CMOS logic with the inputs connected in parallel in the PUN and in series for the PDN. Stick diagrams show how PMOS and NMOS transistors are arranged for correct logic operation.
<p float="center">
  <img src="https://github.com/user-attachments/assets/129908fe-dbea-4e64-bb85-3dc5f24088be" width = 25% />
  <img src="https://github.com/user-attachments/assets/192c6fe9-f53e-4875-8e87-8ca58c066eed" width=15.7% /> 
  <img src="https://github.com/user-attachments/assets/685cbcb1-6082-4edc-9f16-8a5064920351" width=18.3% /> 
</p>

**XOR Gate**
 : Constructed using the expansion of an XOR gate opposed to a combination of AND, OR, and inverters. The layout is optimized for speed and power by using stick diagram opposed to previously designed gates.
<p float="center">
  <img src="https://github.com/user-attachments/assets/8c9f6cfd-1f17-47e8-bcad-e0662d811a6b"  width = 25% />
  <img src="https://github.com/user-attachments/assets/8a89f0aa-5e77-43e0-93b8-f5d708fb378b" width=20% /> 
  <img src="https://github.com/user-attachments/assets/eaa11412-da08-46ab-8c99-6b9bf0dbb772" width=19.5% /> 
</p>

### Full Adder Circuit Schematic and Layout 
The previous gates were connected together to emulate the function of a full adder. Debugging included ensuring all sources and grounds are connected together and there is no metal overlapping by using different metals at intersection points. 
<p float="center">
  <img src="https://github.com/user-attachments/assets/1cf294a6-22e2-406b-ae3b-8902333abfac" width=40% /> 
  <img src="https://github.com/user-attachments/assets/96bde3d4-4d88-4040-b2b0-c9478e1de512" width=36% /> 
</p>
DRC ensures compliance with manufacturing rules. LVS confirms the layout matches the schematic. LPE analyzes parasitic effects on circuit performance. Each gate passed all three tests individually and then the full adder was tested with all three as well after the connection was done. 


## Circuit Simulation w/ Spice3
The full adder was simulated using Spice3, with a standard CMOS implementation. An additional all-NAND simulation was performed for comparison, but the primary design does not rely on NAND-based gates.
