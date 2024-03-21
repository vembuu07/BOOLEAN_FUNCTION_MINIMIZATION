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

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

module ex2(A,B,C,D,F1);
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
Developed by:P vembarasan
RegisterNumber:212223220123


**RTL realization**

![image](https://github.com/vembuu07/BOOLEAN_FUNCTION_MINIMIZATION/assets/150772461/2e9a6bce-b109-4751-ba14-7e3937b27786)

**Truth table**
![image](https://github.com/vembuu07/BOOLEAN_FUNCTION_MINIMIZATION/assets/150772461/7662c7af-0abe-4596-b567-9a9a1deab9cf)

**Timing Diagram**
![image](https://github.com/vembuu07/BOOLEAN_FUNCTION_MINIMIZATION/assets/150772461/3d356b06-ee67-4c64-a835-ca3d7d618212)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

