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
/*
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: s.vasanth
RegisterNumber: 212222110052

module ha(x,y,s,c);
input x,y;
output s,c;
xor(s,x,y);
and(c,x,y);
endmodule

module full_adder(x, y, z, s, c, x1, x2, x3);
input x,  y,z;
output s ,c, x1, x2, x3;
xor(x1, x, y);
xor(s, x1, z);
and(x2, x, y);
and(x3, x1, z);
or(c, x2, x3);
endmodule
   
*/
Logic symbol & Truthtable
RTL realization

### Output:
### RTL
![fa1](https://github.com/vasanth0908/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/122000018/fe0fc8fe-42b6-4a3b-8aa6-05462e979b32)

![ha1](https://github.com/vasanth0908/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/122000018/409afb76-e6b1-4eea-90c0-b6360033b9e2)

### TIMING DIAGRAM

![fa2](https://github.com/vasanth0908/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/122000018/429a0598-612c-4c5c-9868-ce402c0d1a86)

![ha2](https://github.com/vasanth0908/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/122000018/275554ff-a4aa-4228-b9b4-3105b68a9942)



### TRUTH TABLE 
![FATT](https://github.com/vasanth0908/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/122000018/48a99b7d-2a07-4749-9dfb-6e59dd75c4c2)

![HATT](https://github.com/vasanth0908/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/122000018/2858857e-d1f2-4f5e-8762-aabc353bb8f6)


### Result:
