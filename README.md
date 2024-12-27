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

Figure-02 HALF Subtractor


**Truthtable**
**Half Adder**

![WhatsApp Image 2024-12-21 at 09 38 15_b042039a](https://github.com/user-attachments/assets/a1613588-2ebf-4011-b2c9-3b415cb83e11)


**Half subtractor**'

![WhatsApp Image 2024-12-21 at 09 38 09_d248f48c](https://github.com/user-attachments/assets/9d0ed355-d058-47e7-8195-bbb8133ac82e)


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

 Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

Developed by:POTHU SUMANTH
RegisterNumber:24000831

    i)HALF ADDER
    
    module ha(a,b,sum,carry);
    input a,b;
    output sum,carry;
    assign sum= (a ^ b);
    assign carry= ( a & b);
    endmodule

    ii)HALF SUBTRACTOR
    
    module hs(a,b,difference,borrow);
    input a,b;
    output difference,borrow;
    assign difference= (a ^ b);
    assign borrow= ( ~a & b);
    endmodule


**RTL Schematic**

(i)half adder
![Screenshot 2024-11-15 132955](https://github.com/user-attachments/assets/c6cb2726-3c51-42fc-a148-8b92b798cf72)

(ii)half subtractor


![Screenshot 2024-11-15 134529](https://github.com/user-attachments/assets/7c789e4e-1bc7-4f12-a81c-8430105152a2)



**TIMING Waveform**


 (i) half adder
![WhatsApp Image 2024-12-27 at 14 05 24_34684f0a](https://github.com/user-attachments/assets/67db2d1e-455e-4c58-ab05-dcb52091dbd7)


 (ii) half subtractor
![Screenshot 2024-11-15 134929](https://github.com/user-attachments/assets/fc24f9da-1c4a-41b7-9efe-b765f02f5dee)




**Result:**
Thus the Half adder and half Subtractors are studied and the truth tables are verified.
Thus the Half adder and half Adders are studied and the truth tables are verified.

