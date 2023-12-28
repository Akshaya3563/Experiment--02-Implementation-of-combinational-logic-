# Experiment--02-Implementation-of-combinational-logic
Implementation of combinational logic gates
 
# AIM:
To implement the given logic function verify its operation in Quartus using Verilog programming.
 F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
F2=xy’z+x’y’z+w’xy+wx’y+wxy
 
 
 
# Equipments Required
```
 Hardware – PCs, Cyclone II , USB flasher 
 Software – Quartus prime
```


# Theory 
A combinational circuit is a circuit in which the output depends on the present combination of inputs. Combinational circuits are made up of logic gates. The output of each logic gate is determined by its logic function. Combinational circuits can be made using various logic gates, such as AND gates, OR gates, and NOT gates.
 
# Program:

Program to implement the given logic function and to verify its operations in quartus using Verilog programming.
Developed by: AKSHAYA N
RegisterNumber: 212223050003
/* 
```
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
```
/*

# RTL realization
![image](https://github.com/Akshaya3563/Experiment--02-Implementation-of-combinational-logic-/assets/155092474/88a7bd90-c71b-46fb-bd0c-20a472317645)

# Output:
# RTL 
![image](https://github.com/Akshaya3563/Experiment--02-Implementation-of-combinational-logic-/assets/155092474/995682e9-519e-408c-a460-80342b729a98)

## Timing Diagram 
![image](https://github.com/Akshaya3563/Experiment--02-Implementation-of-combinational-logic-/assets/155092474/c48876fb-36e4-4f02-afa3-a5692132fe81)

# Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
