# HALF_ADDER_SUBTRACTOR

Implementation-of-Half-Adder-and-Half Subtractor-circuit

**AIM:**

To design a half adder and half subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher 

Software – Quartus prime Theory Adders are digital circuits that carry out the addition of numbers.

**Half Adder**

Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/bd4a0b2c-cdbc-4184-ab08-81578f121e1f)

Figure -01 HALF ADDER

**Half Subtractor**

The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed. 

Diff = A’B+AB’ =A ⊕ B
Borrow = A’B

 ![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/d76b099c-513f-4e7c-843a-e2fd028a531a)

Figure -02 HALF Subtractor

**Truthtable**
![WhatsApp Image 2024-12-12 at 11 26 55 PM](https://github.com/user-attachments/assets/0988105a-5861-474e-bd0c-7d4c60bc51d9)HALF ADDER

![WhatsApp Image 2024-12-12 at 11 26 54 PM](https://github.com/user-attachments/assets/e8833c46-b424-42d0-a8f2-3389e6ea847c)HALF SUBTRACTOR



**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
```
/* Program to design a half adder and half subtractor circuit and verify its truth table in quartus using Verilog programming.

Developed by:VEMBARASI.A.R
 RegisterNumber:24900729  */
```
```
HALF ADDER:
module EP3(a,b,sum,carry);
input a,b;
output sum,carry;
assign sum= (a ^ b);
assign carry= ( a & b);
endmodule
```
```
HALF SUBTRACTOR:
module EP3(a,b,difference,borrow);
input a,b;
output difference,borrow;
assign difference= (a ^ b);
assign borrow= ( ~a & b);
endmodule
```




**RTL Schematic**

HALF ADDER
![Screenshot (121)](https://github.com/user-attachments/assets/37eca01c-ec3c-476e-a9ad-e35afc238e90)


HALF SUBTRACTOR
![Screenshot (88)](https://github.com/user-attachments/assets/47705a52-e0e1-4ded-8a8d-da0e44a50da4)



**Output/TIMING Waveform**
HALF ADDER
![Screenshot (120)](https://github.com/user-attachments/assets/ed6e3b72-6331-4f22-92de-9b261d76dc6d)


HALF SUBTRACTOR
![Screenshot (119)](https://github.com/user-attachments/assets/c6a21eb4-d156-482d-b23e-34d516e575ae)





**Result:**
Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

