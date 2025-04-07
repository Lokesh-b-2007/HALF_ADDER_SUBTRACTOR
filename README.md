NAME: Lokesh B

REG NO: 24900370

EXP NO 3 : IMPLEMENTATION OF HALF ADDER AND HALF SUBTRACTOR

AIM:

To design a half adder and half subtractor circuit and verify its truth table in Quartus using Verilog programming.

Equipments Required:

Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime Theory Adders are digital circuits that carry out the addition of numbers.

Half Adder

Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

![300513057-bd4a0b2c-cdbc-4184-ab08-81578f121e1f](https://github.com/user-attachments/assets/aa1e0b79-1c30-4023-ac4a-67edfd4c2ca9)


Figure -01 HALF ADDER

Half Subtractor

The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed.

Diff = A’B+AB’ =A ⊕ B Borrow = A’B

![300513222-d76b099c-513f-4e7c-843a-e2fd028a531a](https://github.com/user-attachments/assets/b3ab6e84-939b-4f46-8d80-da06a0b8b73b)


PROCEDURE

Type the program in Quartus software.

Compile and run the program.

Generate the RTL schematic and save the logic diagram.

Create nodes for inputs and outputs to generate the timing diagram.

For different input combinations generate the timing diagram.

Program:

![400645442-86fa317c-d317-4e8a-8b05-5d1db398a450](https://github.com/user-attachments/assets/d67eaabb-bd18-4023-8c5b-bb93a684532d)


TRUTH TABLE:

HALF ADDER

![395010934-44550a0b-1260-4df2-8f9f-e8f1513b6969](https://github.com/user-attachments/assets/2a8fa6ff-0801-46cd-8dd4-4514456d7e1a)

HALF SUBTRACTOR

![395011124-f18592db-9e1e-4f90-9701-8ed2d0ebc5f3](https://github.com/user-attachments/assets/ed3825f0-d691-4517-8822-04e0d4ea9695)

RTL REALIZATION OUTPUT:

![400645724-de7e5514-b487-4c39-bf0c-4fd7778508e4](https://github.com/user-attachments/assets/ca62fbfe-49ab-4ea9-8b45-e68bfd110f9b)


![400645775-dd29871a-2a1a-457a-8066-12ba82d31e7f](https://github.com/user-attachments/assets/50d8f3ae-7dbf-46a3-a892-24cab8ad3f32)


TIMING DIAGRAM:

![400645858-d1b14557-50d9-4d6d-b129-7cfbd253697b](https://github.com/user-attachments/assets/f8afa534-1cb0-45c3-ba67-002c8e3af780)


![400645912-a8c72561-fd6f-4271-85b0-983517616754](https://github.com/user-attachments/assets/634d006c-424c-4a08-9c7e-d6e2bb8ba538)


RESULT

Designed and verified the half adder & half subractor circuit and its truth table in quartus Il using Verilog programming successfully.
