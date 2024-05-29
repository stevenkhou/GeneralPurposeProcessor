# General Purpose Processor

### About The Project:
FPGA based ALU design and implementation in a VHDL environment.
<br />
<br />
The processing unit consists of: 
- Control unit for fetching instructions and generating control signals (4:16 decoder and Moore-Type FSM)
- Bus manages access to data values throughout the processing unit
- Latches served as storage units
- ALU core executes arithmetic and logical operations on inputs and generates outputs

### First ALU Modification:
Modified ALU to correctly execute appropriate boolean operations between 8-bit A and B values when given microcode.
Operations included combinations of AND, OR, NOT, NAND, NOR, and XOR. Results displayed on seven segment display and verified with waveform simulation on Quartus Simulator.
<br />
Block Diagram Schematic:
![image](https://github.com/stevenkhou/GeneralPurposeProcessor/assets/131317174/9e5b194f-155a-4dbf-bb37-826f3dada788)

### Second ALU Modification:
Block Diagram Schematic carries over, however specific sets of boolean functions are assigned to inputs A and B to align them with designated microcode. Results displayed on seven segment display and verified with waveform simulation on Quartus Simulator.

This design implementation correctly operates and functions to address:
1. Swapping lower and upper 4 bits of input A
2. Producing the result of OR-ing inputs A and B
3. Decrementing the value of input B by 5
4. Inverting all bits of input A
5. Inverting the bit-significance order of input A
6. Finding the greater value of inputs A and B and producing the results (Max(A,B))
7. Producing the difference between inputs A and B
8. Producing the result of XNOR-ing inputs A and B
9. Rotating input B to the left by three bits

### Third ALU Modification: 
Modified the ALU to correctly determine if inputs were even or odd for more than 9 clock cycles, then displayed result on the seven segment display.
<br />
Block Diagram Schematic:
![image](https://github.com/stevenkhou/GeneralPurposeProcessor/assets/131317174/d12b896f-d2ce-4454-b421-6c5052a5708c)


