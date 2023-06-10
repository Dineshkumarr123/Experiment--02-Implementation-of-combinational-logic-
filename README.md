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

```
Program to implement the given logic function and to verify its operations in quartus using Verilog programming.
Developed by: R.Dineshkumar.
RegisterNumber:  212222050010
```





## Program:
```
module combinational(a,b,c,d,w,x,y,a,f1,f2);
input a,b,c,d w,x,y,z;
output f1,f2;
wire g1=((~a)&(~b)&(~c)&(~d));
wire g2=((~a)&(~c)&(~d));
wire g3=((~b)&(~c)&(~d));
wire g4=((~a)&(b)&(c)&(d));
wire g5=((b)&(~c)&(d));
assign f1=g1|g2|g3|g4|g5;
wire g6=((x)&(~y)&(z));
wire g7=((~x)&(~y)&(z));
wire g8=((~w)&(x)&(y));
wire g9=((w)&(~x)&(y));
wire g10=((w)&(x)&(y));
assign f2=g6|g7|g8|g9|g10;
endmodule
```


## RTL realization

## Output:![WhatsApp Image 2023-04-26 at 14 00 53](https://user-images.githubusercontent.com/130551452/234518143-fc4904f4-3b9e-42fa-b40b-415a32a587d9.jpg)

## RTL![WhatsApp Image 2023-04-26 at 14 00 54](https://user-images.githubusercontent.com/130551452/234518026-91c66ba2-fd52-4009-a773-15c7839ea208.jpg)

## Timing Diagram
## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
