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

![436370854-a1ba1ddc-ddae-4d0f-95ba-6e123cc59f97](https://github.com/user-attachments/assets/49a0b6c9-b823-4a7b-8c83-da1ef043db8f)

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
```
Half Adder

module hadd(a, b, sum, cout);
input a,b;
output sum, cout;
xor g1(sum,a,b);
and g2(cout,a,b);
endmodule

Half Adder

module hadd(a, b, sum, cout);
input a,b;
output sum, cout;
xor g1(sum,a,b);
and g2(cout,a,b);
endmodule
```
Developed by: Manoj R
RegisterNumber:212224230152
**RTL Schematic**

![436372450-fb89dd15-7575-4d28-a4c7-ab80db8a609c](https://github.com/user-attachments/assets/4f548ca3-bc42-4225-a3fb-fef30cff0fb7)

![436372479-a4bb5c81-276b-46b9-baf6-0d7df74f9515](https://github.com/user-attachments/assets/8b4f79c8-014e-46ce-8ecc-4b6e6084c90d)

**Output/TIMING Waveform**

![436371530-b004f868-2b66-44a5-8b23-dbe623495162](https://github.com/user-attachments/assets/72b9468e-36d0-489a-87ad-642ab057c332)

![436371597-2798f668-f8eb-44cb-94cd-1a29e3aa26d9](https://github.com/user-attachments/assets/ccbb95f1-2714-4ffb-ade9-0cd82d70c2bc)

**Result:**

Thus the truth table of half adder and half subtractor in Quartus II using Verilog programming is verified
