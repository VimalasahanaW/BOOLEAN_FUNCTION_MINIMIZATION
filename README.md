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


**Program:**

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming.*/ 

Developed by:vimala sahana W RegisterNumber:212223040241
```
module program2(A,B,C,D,F1);
input A,B,C,D;
output F1;
wire x1,x2,x3,x4,x5;
assign x1=(~A)&(~B)&(~C)&(~D);
assign x2=(A)&(~C)&(~D);
assign x3=(~B)&(C)&(~D);
assign x4=(~A)&(B)&(C)&(D);
assign x5=(B)&(~C)&(D);
assign F1=x1|x2|x3|x4|x5;
endmodule
```
**RTL realization**

**Output:**


![image](https://github.com/VimalasahanaW/BOOLEAN_FUNCTION_MINIMIZATION/assets/144870812/a137aa35-b1c7-46ae-88e9-ff59337e3a94)



**Timing Diagram**
![image](https://github.com/VimalasahanaW/BOOLEAN_FUNCTION_MINIMIZATION/assets/144870812/1e266027-1a03-4730-9d29-633a0f4383fd)

![image](https://github.com/VimalasahanaW/BOOLEAN_FUNCTION_MINIMIZATION/assets/144870812/503e923b-899a-4a84-a04d-af94b18ca1e3)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

