# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

**Logic Diagram**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:
```module ex2 (a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
assign f1 = ~a&~b&~c&~d | a&~c&~d | ~b&c&~d | ~a&b&c&d | b&~c&d;
assign f2 = x&~y&z | ~x&~y&z | ~w&x&y | w&~x&y | w&x&y;
endmodule
```**

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by:Aathishwaran K RegisterNumber:25009618
*/


**RTL realization output**

<img width="1918" height="1012" alt="Screenshot 2025-11-20 141925" src="https://github.com/user-attachments/assets/022ddbbf-25a0-4c96-860f-365516e71076" />
**

**RTL
<img width="1919" height="1008" alt="Screenshot 2025-11-20 142526" src="https://github.com/user-attachments/assets/8ffb99d6-0d35-4b64-b97d-39747dfa88a1" />
**

**Timing Diagram ![WhatsApp Image 2025-11-20 at 14 33 57_68c31c1d](https://github.com/user-attachments/assets/4f17322d-dd17-4498-8914-22853aa57670)

**

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

