# FULL_ADDER_SUBTRACTOR

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

**Procedure**
1.Open Quartus Software
2.Create a New Project
3.Create a New Design File
4.Compile the Program
5.Generate RTL Schematic
6.Create Nodes for Inputs/Outputs
7.Generate Timing Diagram
8.Simulate Different Input Combinations
9.Save Your Work
**Program:**

/* Developed by: jenil pio j
RegisterNumber:212223220040
Full adder: 

module proj_41(a,b,cin,sum,carry);
input a,b,cin;
output sum, carry;
assign sum=(a^b^cin);
assign carry=((a&b)|(b&cin)|(cin&a));
endmodule

##Full Subtractor:

module proj_42(a,b,bin,borr,diff);
input a,b,bin;
output diff, borr;
assign diff=(a^b^bin);
assign borr=((~a&b)|(b&bin)|(bin&~a));
endmodule
*/

##  FULL ADDER:
![image](https://github.com/user-attachments/assets/403d7f51-25b9-415b-b9ce-6d612cdb48c3)

## Full subtractor:
![image](https://github.com/user-attachments/assets/6a6203ae-82ab-4153-bccb-ca0526c95308)

**Output Timing Waveform**
##  FULL ADDER:
![image](https://github.com/user-attachments/assets/f418d904-6ed9-4980-b473-dc23774973b1)
## full subtractor:
![image](https://github.com/user-attachments/assets/e37bebcd-1011-4e67-9ae0-28f0dbc54ccd)


**Result:**

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.



