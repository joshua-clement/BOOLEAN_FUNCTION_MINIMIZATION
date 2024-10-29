# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**
![WhatsApp Image 2024-10-29 at 10 50 38_e1b8e139](https://github.com/user-attachments/assets/7af85aa9-09ce-4499-b551-283a3fa1e3cd)



**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
```
module exp_2(a,b,c,d,f1,w,x,y,z,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
assign f1=((~b&~d)|(~a&b&d)|(a&b&~c));
assign f2=((~y&z)|(x&y)|(w&y));
endmodule
```
/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: RegisterNumber:*/24004630  



**RTL**
![exp_2](https://github.com/user-attachments/assets/e843b406-0362-45ba-a7a6-cdf676a1ca16)

**Timing Diagram**
![Waveform](https://github.com/user-attachments/assets/0233b9fa-b574-4306-9d6f-fda8c7da2583)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

