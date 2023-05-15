# Experiment--02-Implementation-of-combinational-logic
Implementation of combinational logic gates
 
## AIM:
To implement the given logic function verify its operation in Quartus using Verilog programming.
 F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
F2=xy’z+x’y’z+w’xy+wx’y+wxy
 
 
 
## Equipments Required:
## Hardware – PCs, Cyclone II , USB flasher
## Software – Quartus prime


## Theory
 

## Logic Diagram
## Procedure
## Program:
```
/*
Program to implement the given logic function and to verify its operations in quartus using Verilog programming.
Developed by: SANDHIYA R
RegisterNumber: 212222230129
*/
module combinational (a,b,c,d,w, x, y, z, f1, f2);
input a,b,c,d,w, x, y, z;
output fl, 12;
wire gl=((-a) & (~b) & (~C) & (~d));
wire g2=((a) & (~c) & (~d));
wire g3-((-b) & (c) & (~d))
; wire g4-((~a) & (b) & (c) & (d));
wire g5=((b) & (~c) & (d));
assign fl-gl|g2|g3|g4|g5;
wire g6=((x) & (~y) & (z)); 
wire g7=((~x) & (~y) & (z));
wire g8=((~w) & (x) & (y)); 
wire g9=((w) & (~x) & (y)); 
wire g10=((w) & (x) & (y)); 
assign f2=g6|g7|g8|g9|g10; 
endmodule
```
## RTL realization
![image](https://github.com/SandhiyaR1/Experiment--02-Implementation-of-combinational-logic-/assets/113497571/55852475-cf74-46fd-98cc-9b3b9adfd8bb)
![image](https://github.com/SandhiyaR1/Experiment--02-Implementation-of-combinational-logic-/assets/113497571/fbc4d616-f503-4e30-880e-f9666a5569d5)


## Output:
![image](https://github.com/SandhiyaR1/Experiment--02-Implementation-of-combinational-logic-/assets/113497571/6073d9e1-5013-4425-985d-379278276474)

## RTL
## Timing Diagram
![image](https://github.com/SandhiyaR1/Experiment--02-Implementation-of-combinational-logic-/assets/113497571/da628853-42b5-49ea-aa98-6db89eb26db9)

## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
