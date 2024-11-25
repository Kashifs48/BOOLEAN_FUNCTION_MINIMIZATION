Name: SYED KASHIF S

Register Number: 24006084

EXP2: BOOLEAN FUNCTION MINIMIZATION
AIM:

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D

F2=xy’z+x’y’z+w’xy+wx’y+wxy

Equipment Required:

Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime

Theory

Logic function is implemented using Verilog, a hardware description language used to model electronic systems. Verilog enables the design and simulation of digital circuits efficiently. Quartus software is utilized to compile, synthesize, and verify the logic function through simulation. This process ensures the functionality aligns with the expected behavior of the logic design

Procedure

1.Type the program in Quartus software.

2.Compile and run the program.

3.Generate the RTL schematic and save the logic diagram.

4.Create nodes for inputs and outputs to generate the timing diagram.

5.For different input combinations generate the timing diagram.

Program:

Program to implement the given logic function and to verify its operations in quartus using Verilog programming.

module exp_2(A, B,C,D,W,X,Y,Z,F1,F2);
input A, B, C,D,W,X,Y,Z;
wire w1,w2,w3,w4,w5,w6,w7,w8,w9,w10;
output F1,F2;
assign w1=(~A)&(~B)&(~C)&(~D);
assign w2=(A)&(~C)&(~D);
assign w3=(~B)&(C)&(~D);
assign w4=(~A)&(B)&(C)&(D);
assign w5=(B)&(~C)&(D);
assign w6=(X)&(~Y)&(Z);
assign w7=(~X)&(~Y)&(Z);
assign w8=(~W)&(X)&(Y);
assign w9=(W)&(~X)&(Y);
assign w10=(W)&(X)&(Y);
assign F1=w1|w2|w3|w4|w5;
assign F2=w6|w7|w8|w9|w10;
endmodule 
RTL realization
![image](https://github.com/user-attachments/assets/fd0325d1-2a9a-4d38-a055-f6d37d154fa6)

Output:
![image](https://github.com/user-attachments/assets/dce35852-faa8-4419-ac2c-37a38c3abb60)

Result:

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

