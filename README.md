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
![Screenshot (12)](https://github.com/user-attachments/assets/544c317b-493b-4b5b-ab34-8efb8f5f7e9c)

![WhatsApp Image 2024-11-12 at 14 25 12_f946365c](https://github.com/user-attachments/assets/93f9792d-bd2c-4ffc-ade2-5da196c8bfc0)

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

module funct1(a,b,c,d,f1);

input a,b,c,d;

output f1;

assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));

endmodule

module funct2(w,x,y,z,f2);

input w,x,y,z;

output f2;

assign f2=((~y & z)|( w & y )|(x & y));

endmodule


/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by:Santhanam S RegisterNumber:24900166*/


**RTL realization**

**Output:**

**RTL**
![Screenshot (13)](https://github.com/user-attachments/assets/7d83c9fe-600d-4e17-8ca2-cc5735ecc6f3)

![WhatsApp Image 2024-11-12 at 14 25 13_95e32ba4](https://github.com/user-attachments/assets/a31f14e2-58f8-4fbc-9753-2a02a37d3627)

**Timing Diagram**

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

