## Name:Hariharan A
## Register number:23012392

# Exp 02 Implementation of Half Adder and Full Adder circuit


### AIM:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.

### Equipments Required:
Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime
## Theory
Adders are digital circuits that carry out addition of numbers.

### Half Adder
Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

#### Figure -01 HALF ADDER
 ![image](https://user-images.githubusercontent.com/36288975/163552156-a13e5a56-c638-4110-97d9-8896907c8d25.png)

 ## Procedure
 Connect the supply (+5V) to the circuit Switch ON the main switch If the output is 1, then the led glows.

 ## Program
```
module project_3(sum,carry,a,b); 
input a,b; 
output sum,carry; 
xor sum1(sum,a,b); 
and carry1(carry,a,b); 
endmodule
```

## RTL Realization
![d e1](https://github.com/hariharana59/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/144980130/71817b12-8be0-435a-86c4-975e08b69c04)

## Timing Diagram
![d e2](https://github.com/hariharana59/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/144980130/22fde24c-2842-4f9d-b14d-e47d1ad877dd)


## Truth table

![d e3](https://github.com/hariharana59/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/144980130/5e59b1a7-3a11-4bf2-8bcf-16af5565be6b)

### Full Adder
Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin Carry = AB + ACin + BCin



 #### Figure -01 FULL ADDER


![image](https://user-images.githubusercontent.com/36288975/163552057-b3547877-6d07-45b4-b7e0-bcfebfad9e1d.png)



### Procedure

Connect the supply (+5V) to the circuit.Switch ON the main switch.If the output is 1, then the led glows.

## Program:
```
module project_3_2(a,b,c,sum,carry);
input a,b,c;
output sum,carry;
xor(sum,a,b,c);
assign carry=a&b | b&c | a&c;
endmodule
```


## RTL realization
![d e 1](https://github.com/hariharana59/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/144980130/85af7192-3c80-4ce4-b82b-71909d3cfc15)


### TIMING DIAGRAM
![d e 2](https://github.com/hariharana59/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/144980130/2e1aa2ca-9ee0-4d4e-8678-4c5a8fb7c0b4)


### TRUTH TABLE 
![d e 3](https://github.com/hariharana59/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/144980130/a321ec86-3881-4dab-8c4b-b72a9b07c7af)

### Result:
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
