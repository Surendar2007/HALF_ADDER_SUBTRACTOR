# HALF_ADDER_SUBTRACTOR

Implementation-of-Half-Adder-and-Half Subtractor-circuit
NAME: S.D. SURENDAR, REG NO.24901073

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
HALF ADDER:
\\\
 ![tt half adder](https://github.com/user-attachments/assets/14bbb4c3-9b0c-49b6-af9d-4ca3361b46c1)


HALF SUBTRACTOR:
\\\
 ![Screenshot 2024-12-05 115406](https://github.com/user-attachments/assets/560a03e5-dda3-420c-8cb3-4773670b291c)



**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
\\
HALF ADDER:
\\\
module half_adder_structural(
input a,//Input'a'
input b,//Input'b'
output s,//Output's'(Sum)
output c//Output'c'(Carry)
);
xor gate_xor(s,a,b);//XOR gate for sum
and gate_xor(c,a,b);//AND gate for carry
endmodule
\\\
HALF SUBTRACTOR:
\\\
module halfsub(diff,borr,a,b);
input a,b;
output diff,borr;
wire w1;
xor g1(diff,a,b);
not g2(w1,a);
and g3(borr,w1,b);
endmodule
\\\

**RTL Schematic**
HALF ADDER:
\\\
   ![Screenshot 2024-12-05 114157](https://github.com/user-attachments/assets/bf72f284-aca8-44ce-aaac-fd12f94034e3)
   
   
HALF SUBTRACTOR:
\\\
 ![half subtracter rtl](https://github.com/user-attachments/assets/a6e825a3-9a8e-4631-b3de-304e5595f6d4)
 





**Output/TIMING Waveform**
HALF ADDER:
\\\
  ![Screenshot 2024-12-05 114210](https://github.com/user-attachments/assets/08cfbd0d-7f48-436f-afbc-55e722fabec5)
  
 HALF SUBTRACTOR:
 \\\
  ![half subtractor output](https://github.com/user-attachments/assets/26a33d4f-e0fc-48c8-a320-22d5d175cc00)

 
 


**Result:**
Thus we learned to design a half adder and half subtractor circuit and verify its truth table in quartus using verilog programming. 
