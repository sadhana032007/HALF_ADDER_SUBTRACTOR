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
Half adder

<img width="474" height="357" alt="Screenshot 2025-11-25 232921" src="https://github.com/user-attachments/assets/3fab1db0-4435-47d9-ae78-e9414b3d5d02" />
Full adder

<img width="676" height="479" alt="Screenshot 2025-11-25 232929" src="https://github.com/user-attachments/assets/1442cc4a-26ab-4c74-b438-7e1d63a1508f" />

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
i)HALF ADDER
 module ha(a,b,sum,carry); input a,b; output sum,carry; assign sum= (a ^ b); assign
 carry= ( a & b); endmodule
 ii)HALF SUBTRACTOR
module hs(a,b,difference,borrow); input a,b; output difference,borrow; assign
 difference= (a ^ b); assign borrow= ( ~a & b); endmodule

**RTL Schematic**
<img width="933" height="474" alt="Screenshot 2025-11-25 232352" src="https://github.com/user-attachments/assets/001d7a7b-c16a-4298-957c-fa08950d46f8" />
<img width="919" height="463" alt="Screenshot 2025-11-25 232404" src="https://github.com/user-attachments/assets/61d3d394-ce94-4288-8e37-1915cbc45ea4" />

**Output/TIMING Waveform**
<img width="926" height="469" alt="Screenshot 2025-11-25 232210" src="https://github.com/user-attachments/assets/c2f9adc8-9a3f-4823-9e19-33f500b676bc" />
<img width="928" height="471" alt="Screenshot 2025-11-25 232220" src="https://github.com/user-attachments/assets/baf3fa05-3f49-4387-898e-bcca279cdbab" />

**Result:**
 Thus ,the half adder and half subtractor are studied and the truth table , logic diagram
 and waveform are verified
