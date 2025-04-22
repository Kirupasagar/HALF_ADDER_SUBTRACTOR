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

HALF ADDER
![431715661-954d6037-b3f4-4a4e-8db5-9a6bd1102317](https://github.com/user-attachments/assets/e8b9c8e6-1a4e-4dc3-b05d-92595cb7fde5)
HALF SUBRACTOR
![431715756-16d40871-8df9-47ee-a5a1-821e4307185b](https://github.com/user-attachments/assets/2a3495b0-e787-4233-bf18-c882ee7040af)

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
```
module exp3(a,b,C,D,S,B);
input a,b;
output C,D,S,B;
assign S=a^b;
assign C=a&b;
assign D=a^b;
assign B=~a&b;
endmodule
```
Developed by:KIRUPASAGAR RegisterNumber:212224230126

**RTL Schematic**
![430866242-a7f5d1ff-bcc9-4b16-9245-5e91a8cd92b0](https://github.com/user-attachments/assets/de10fac9-7d1f-489f-b985-e9b53d869bc9)

**Output/TIMING Waveform**
![430866395-d447525f-e92e-486e-86e0-6719799a9e07](https://github.com/user-attachments/assets/82aed74a-e857-48dc-9aae-5ca0bc3c0368)

**Result:**
Thus half adder and half subtractor circuit and its truth table in Quartus using Verilog programming is verified.
