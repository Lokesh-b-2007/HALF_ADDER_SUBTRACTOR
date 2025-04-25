HALF_ADDER_SUBTRACTOR
Implementation-of-Half-Adder-and-Half Subtractor-circuit

AIM:

To design a half adder and half subtractor circuit and verify its truth table in Quartus using Verilog programming.

Equipments Required:

Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime Theory Adders are digital circuits that carry out the addition of numbers.

Half Adder

Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

![300513057-bd4a0b2c-cdbc-4184-ab08-81578f121e1f](https://github.com/user-attachments/assets/fe440fb8-5d22-458a-986d-bb977bd256c7)


Figure -01 HALF ADDER

Half Subtractor

The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed.

Diff = A’B+AB’ =A ⊕ B Borrow = A’B

![300513222-d76b099c-513f-4e7c-843a-e2fd028a531a](https://github.com/user-attachments/assets/52ebf6e4-08b3-4fa3-9bf0-7951496eaffb)


Figure -02 HALF Subtractor

Truthtable

HALF ADDER TRUTHTABLE

![385144707-ee0c7cc4-4b0f-462c-bf97-eecfacb7c1ee](https://github.com/user-attachments/assets/b35503d8-1fa2-4ce8-a8ee-080802f812a8)


HALF SUBTRACTOR TRUTHTABLE

![388824561-ec06694e-4c6b-43bf-90a7-aca635af6b94](https://github.com/user-attachments/assets/69fac568-b983-4c6e-b41d-cf8710d1ceba)


Procedure

Type the program in Quartus software.

Compile and run the program.

Generate the RTL schematic and save the logic diagram.

Create nodes for inputs and outputs to generate the timing diagram.

For different input combinations generate the timing diagram.

Program:
~~~
module ex03(a,b,cy,sm,df,bo);
input a,b;
output sm,cy,df,bo;
xor (sm,a,b);
and (cy,a,b);
xor (df,a,b);
and (bo,~a,b);
endmodule
~~~
/* Program to design a half adder and half subtractor circuit and verify its truth table in quartus using Verilog programming.

Developed by: Lokesh B reg.no:-212224040172

RTL Schematic

![385143417-0667ce93-345a-4bec-8c25-a2cf7cf47731](https://github.com/user-attachments/assets/49f02346-bcc3-41eb-a55b-a17f2199b2be)


Output/TIMING Waveform
![385143495-0564f8a4-97da-4ce7-8740-eb97c0f35d0a](https://github.com/user-attachments/assets/79c32928-8d31-4327-a625-689def88275f)


Result: The half adder and half subtractor circuit and its truth table in Quartus are verified using Verilog programming.

 
