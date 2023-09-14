# Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit

# Implementation-of-Half-Adder-and-Full-Adder-circuit
### AIM:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.

### Equipments Required:
Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime
Theory
Adders are digital circuits that carry out addition of numbers.

### Half Adder
Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

### Full Adder
Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin Carry = AB + ACin + BCin

 ![image](https://user-images.githubusercontent.com/36288975/163552156-a13e5a56-c638-4110-97d9-8896907c8d25.png)

#### Figure -01 HALF ADDER 


![image](https://user-images.githubusercontent.com/36288975/163552057-b3547877-6d07-45b4-b7e0-bcfebfad9e1d.png)

#### Figure -02 FULL ADDER 

### Procedure

Connect the supply (+5V) to the circuit
Switch ON the main switch
If the output is 1, then the led glows.
### 
Program:
```
##c Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
## Developed by: SAKTHIVEL R
## RegisterNumber:  212222100044
## HALF ADDER:
module exp33(a,b,s,c);
input a,b;
output s,c;
assign s=a^b;
assign c=a&b;
endmodule
## FULL ADDER:
module ass3(a,b,c,sum,carry);
input a,b,c;
output sum,carry;
assign sum=a^b^c;
assign carry= ((a&b)|(b&c)|(c&a));
endmodule
```
## Logic symbol & Truthtable RTL realization
## Output:
## RTL
## HALF ADDER:
![Screenshot 2023-09-14 182125](https://github.com/sakthivel005/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/120550359/102cd944-2825-442a-a120-f7207350ca7d)


## FULL ADDER:
![Screenshot 2023-09-14 182136](https://github.com/sakthivel005/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/120550359/357cf724-c06f-4c94-9d14-2bb08416d416)


## TIMING DIAGRAM:
## HALF ADDER:

![Screenshot 2023-09-14 182149](https://github.com/sakthivel005/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/120550359/3a8101e6-174f-4367-ac0c-98a5171b6f8a)

## FULL ADDER:
![Screenshot 2023-09-14 182207](https://github.com/sakthivel005/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/120550359/ca611199-43da-4b4d-9cac-1a1f1aed4112)


## TRUTH TABLE :
## HALF ADDER:
![Screenshot 2023-09-14 182219](https://github.com/sakthivel005/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/120550359/f99a7dff-1c74-4343-8385-22fb4a842baa)


## FULL ADDER:
![Screenshot 2023-09-14 182229](https://github.com/sakthivel005/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/120550359/207d506b-db9b-4e6a-9090-c7573b422cac)


## Result:
Thus the half adder and full adder are studied and the truth table for different logic gates are verified.
