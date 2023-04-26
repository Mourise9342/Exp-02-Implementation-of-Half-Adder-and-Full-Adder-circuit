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
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: Mourise jane 
RegisterNumber: 212222230085

HALF ADDER:
module halfadder(A,B,C,S);
input A,B;
output S,C;
xor(S,A,B);
and(C,A,B);
endmodule

FULL ADDER:
module fulladd(a,b,ci,s,co);
input a,b,ci;
output s,co;
wire d,e,f;
xor(d,a,b);
xor(s,d,ci);
and(e,ci,d);
and(f,a,b);
or(co,e,f);
endmodule
```
###output

RTL realization
## HALF ADDER:
![half 50](https://user-images.githubusercontent.com/120081893/234522773-7003050c-08d6-4322-960e-0df6123760a9.png)

##FULL ADDER:
![full 51](https://user-images.githubusercontent.com/120081893/234523497-630bd9f6-5c67-4832-aaee-1459a2286c8b.png)

### TIMING DAIGRAM:
## HALF ADDER:
![Screenshot 52](https://user-images.githubusercontent.com/120081893/234524747-765d55d2-0d80-4c8c-9172-eb4d7d5adf34.png)

## FULL ADDER:
![full 53](https://user-images.githubusercontent.com/120081893/234525410-da3236bf-ba42-417a-b927-8e74eec34b80.png)

### TRUTH TABLE 
##HALF ADDER
![half 54](https://user-images.githubusercontent.com/120081893/234526574-bf8ec66d-d37d-4189-a7e7-650cfbe9382e.png)

##FULL ADDER
![Full 55](https://user-images.githubusercontent.com/120081893/234527122-93baca3c-69a2-4653-8bdc-abe959df7bf8.png)


### Result:
Thus the half adder and full adder are studied and the truth table for different logic gates are verified.
