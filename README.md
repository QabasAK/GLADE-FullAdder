# GLADE-FullAdder

Design and implement a **full adder circuit** using **CMOS** technology in the **GLADE** environment leveraging 2 **XOR** gates, 2 **AND** gates, one **OR** gate and an **inverter**. Test the design using Design Rule Check **(DRC)**, Layout Versus Schematic **(LVS)** and
Layout Parasitic Extraction **(LPE)**.

## Circuit Design w/ GLADE
A full adder circuit takes three inputs, two operands and carry in, and produces two outputs, the
sum and carry out. To build the full adder, the schematic, stick diagram as well as the layout was done:
### Inverter 
The CMOS inverter is the simplest gate and consists of a PMOS and an NMOS transistor in series.
 <p float="center">
  <img src="https://github.com/user-attachments/assets/fa87eb55-37ea-489a-9013-bb28414428af" alt="Inverter Stick Diagram" width = 40% />
  <img src="https://github.com/user-attachments/assets/4d23b754-c343-42a6-9277-325f04479284" width=21% /> 
  <img src="https://github.com/user-attachments/assets/7301e619-54c0-4530-aa55-ad7c652511bd" width=30% /> 
</p>

### AND Gate 
 <p float="center">
  <img src="https://github.com/user-attachments/assets/0e386175-d050-45e9-9704-d71983bf6a17" alt="Inverter Stick Diagram" width = 40% />
  <img src="https://github.com/user-attachments/assets/0036b20c-b081-4f2b-ba1a-58f41c008d05" width=33% /> 
  <img src="https://github.com/user-attachments/assets/3d553384-46ab-4144-b15a-0bae03612621" width=25% /> 
</p>

### OR Gate 
 <p float="center">
  <img src="https://github.com/user-attachments/assets/129908fe-dbea-4e64-bb85-3dc5f24088be" width = 40% />
  <img src="https://github.com/user-attachments/assets/192c6fe9-f53e-4875-8e87-8ca58c066eed" width=26% /> 
  <img src="https://github.com/user-attachments/assets/685cbcb1-6082-4edc-9f16-8a5064920351" width=31% /> 
</p>

### XOR Gate 
 <p float="center">
  <img src="https://github.com/user-attachments/assets/fa87eb55-37ea-489a-9013-bb28414428af" alt="Inverter Stick Diagram" width = 40% />
  <img src="https://github.com/user-attachments/assets/4d23b754-c343-42a6-9277-325f04479284" width=21% /> 
  <img src="https://github.com/user-attachments/assets/7301e619-54c0-4530-aa55-ad7c652511bd" width=30% /> 
</p>

## Circuit Simulation w/ Spice3
