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
Program to implement the given logic function and to verify its operations in quartus using Verilog programming.
Developed by: JEEVITHA.E
RegisterNumber: 212222230054

module Verilog1(a,b,c,d,w,x,y,z,F1,F2);
input a,b,c,d,w,x,y,z;
output F1,F2;
wire  A1,A2,A3,A4,A5,B1,B2,B3,B4,B5;
assign A1= (~a&(~b)&(~c)&(~d));
assign A2= (a&c&(~d));
assign A3= ((~b)&c&(~d));
assign A4= (~a&b&c&d);
assign A5= (b&(~c)&d);
assign F1= A1|A2|A3|A4|A5;
assign B1= (x&(~y)&z);
assign B2= (~x&(~y)&z);
assign B3= (~w&x&y);
assign B4= (w&(~x)&y);
assign B5= (w&y&z);
assign F2= B1|B2|B3|B4|B5;
endmodule
```
## RTL realization

## Output:
## RTL
![image](https://user-images.githubusercontent.com/118708245/234779151-145287ef-5681-4a03-afa2-b5b635339db5.png)
![image](https://user-images.githubusercontent.com/118708245/234779222-f63d5402-9471-4404-b264-9a6829925451.png)

## Timing Diagram
![image](https://github.com/Jeevithaelumalai/Experiment--02-Implementation-of-combinational-logic-/assets/118708245/142c239d-1813-4b23-b520-58c42a51d251)

## Truth Table:
![image](https://github.com/Jeevithaelumalai/Experiment--02-Implementation-of-combinational-logic-/assets/118708245/e6994a3d-2ce6-44a5-b05d-ffdf103d3feb)

## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
