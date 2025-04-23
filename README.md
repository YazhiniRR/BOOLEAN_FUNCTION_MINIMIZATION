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

**Truth table**
![Screenshot 2025-04-23 212246](https://github.com/user-attachments/assets/8fde8996-cf9b-46cc-8723-bcd0e95c6193)

**Truth table**
![Screenshot 2025-04-23 212300](https://github.com/user-attachments/assets/756d62ba-6f9e-47e3-a989-1e5fbcbe0c1d)

**Program:**
```
1) module logic_function(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a&b&d)|(a&b&~c));
endmodule
```
```
2) module EXP2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y & z)|( w & y )|(x & y));
endmodule
```
/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: YAZHINI R R
RegisterNumber: 212224100063


**RTL realization**

![Screenshot 2025-04-23 212200](https://github.com/user-attachments/assets/b775cd80-a125-4b4a-a4f8-57a962bdff09)

**RTL**
![Screenshot 2025-04-23 212228](https://github.com/user-attachments/assets/1d493ed6-803e-4915-80ae-58d43c2245a6)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

