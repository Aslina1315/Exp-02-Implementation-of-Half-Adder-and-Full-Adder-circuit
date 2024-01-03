# Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit

# Implementation-of-Half-Adder-and-Full-Adder-circuit
### AIM:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.

### Equipments Required:
Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime

Theory:
Adders are digital circuits that carry out addition of numbers.

### Half Adder
Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.
Sum = A’B+AB’ =A ⊕ B Carry = AB

### Full Adder
Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin Carry = AB + ACin + BCin
![image](https://github.com/Aslina1315/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/155459437/4912c1d0-164d-49c9-86f0-25683d45d3d8)
#### Figure -01 HALF ADDER 
![image](https://github.com/Aslina1315/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/155459437/8bdcdb48-ca9f-4e81-a525-3808e66776b4)
#### Figure -02 FULL ADDER

### Procedure
Connect the supply (+5V) to the circuit Switch ON the main switch If the output is 1, then the led glows.

### Program:
HALF ADDER
module exp03(A,B,c,s);
input A,B;
output s,c;
assign s=A^B;
assign c=A&B;
endmodule

FULL ADDER
module exp03(A,B,c,sum,carry);
input A,B,c;
output sum,carry;
assign sum=A^B^c;
assign carry=((A&B)|(B&c)|(c&A));
endmodule
/*
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by:M.Noorul aslina
RegisterNumber:212223050033
*/
Logic symbol & Truthtable RTL realization:
Output:
HALF ADDER RTL
![image](https://github.com/Aslina1315/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/155459437/e5d664e0-e94c-425c-a7a2-b15a7d8567af)
HALF ADDER WAVEFORM
![image](https://github.com/Aslina1315/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/155459437/4bc5813d-6232-47af-84a8-c0b5259ec6da)
HALF ADDER TRUTH TABLE
![image](https://github.com/Aslina1315/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/155459437/a25afbe7-dcb7-4986-93af-bfaeaaf7f795)

FULL ADDER RTL
![image](https://github.com/Aslina1315/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/155459437/d4f6baf9-aad1-4c43-8a3a-21fda25acfdf)
FULL ADDER WAVEFORM
![image](https://github.com/Aslina1315/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/155459437/5dc4d19b-d9f4-43dd-b26b-fe6b6082a04b)
FULL ADDER TRUTH TABLE
![image](https://github.com/Aslina1315/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/155459437/735b997f-02d3-423f-a551-bc025cd33b4f)


## Result:
Thus the half adder and full adder circuits are designed and the truth tables is verified using quartus software.


