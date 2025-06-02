# FULL ADDER SUBTRACTOR

## NAME:- JAIYANTAN S
## REG_NO:-  212224100021

Implementation-of-Full-Adder-and-Full-subtractor-circuit

**AIM:**

To design a Full Adder and Full Subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime


**Full Adder and Full Subtractor**

**Full Adder**

Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin 

Carry = AB + ACin + BCin

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/0f30ba51-5ffb-4198-845f-18e054f675e7)

**Figure -1 FULL ADDER**

**Full Subtractor**

A full subtractor is a combinational circuit that performs subtraction involving three bits, namely minuend, subtrahend, and borrow-in . It accepts three inputs: minuend, subtrahend and a borrow bit and it produces two outputs: difference and borrow.

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/02b24f51-ab51-4304-9ad6-7b81ffc1ead5)

Diff = A ⊕ B ⊕ Bin 

Borrow out = A'Bin + A'B + BBin

**Truthtable**

![435919808-3e1620d1-e2a9-![435919903-0d1a306f-1de5-49b2-a6a9-6f9da6816c1a](https://github.com/user-attachments/assets/1522aab0-f0e9-4964-b328-8f717c4e50c4)
4387-be27-54bdfb65c856](https://github.com/user-attachments/assets/517f4a08-c2b4-4378-93ed-ceeb8f89c9ba)*
![435919903-0d1a306f-1de5-49b2-a6a9-6f9da6816c1a](https://github.com/user-attachments/assets/0fbd03c3-de15-41bf-83c8-76785193d1bd)

**Procedure**
1. Type the program in Quartus software.

2. Compile and run the program.

3. Generate the RTL schematic and save the logic diagram.

4. Create nodes for inputs and outputs to generate the timing diagram.

5. For different input combinations generate the timing diagram.

**Program:**
```python
/* Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming.
Developed by: Jaiyantan S
 RegisterNumber: 212224100021

module exp3(a,b,cin,bin,sum_a,cout,diff_s,borr_s);
input a,b,cin,bin;
output sum_a,cout,diff_s,borr_s;
assign sum_a=a^b^cin;
assign cout=(a^b)&cin |(a&b);
assign diff_s=a^b^bin;
assign borr_s=(~a&~b&~bin)|(~a&b&~bin)|(~a&b&bin)|(a&b&bin);
endmodule
*/
```
**RTL Schematic**
![435920541-0d03043d-4aa8-4a7a-bc7a-546b3e658188](https://github.com/user-attachments/assets/15f1aa65-f53b-4851-b8e7-a4833743db09)



**Output Timing Waveform**

![435921325-e083f2b0-aa7f-410e-beeb-bd6d2bc3898e](https://github.com/user-attachments/assets/667a6740-9cf8-4a45-92c4-7605d9d8fde2)


**Result:**

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.



