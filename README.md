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
```
1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.
```

**Program:**
```
/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by:Infancia Felcy p
RegisterNumber:*212223040067
module exp22(A,B,C,D,F1);
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
![experiment 2 gates](https://github.com/Infanciafelcy/BOOLEAN_FUNCTION_MINIMIZATION/assets/155411010/5a15c276-6cb9-45ef-9bb7-4aba9b1d4a12)
**Truth Table**
![EXP2 EXCEL](https://github.com/Infanciafelcy/BOOLEAN_FUNCTION_MINIMIZATION/assets/155411010/ee2fd841-7a98-4ded-9637-76f31327d8b3)
**Waveform**
![exp 2 waveform](https://github.com/Infanciafelcy/BOOLEAN_FUNCTION_MINIMIZATION/assets/155411010/bce7ad1d-dd00-451f-b1b0-8797ea332973)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

