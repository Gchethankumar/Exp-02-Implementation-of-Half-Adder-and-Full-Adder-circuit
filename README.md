# Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit

# Implementation-of-Half-Adder-and-Full-Adder-circuit
### AIM:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.

### Equipments Required:
Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime
Theory
Adders are digital circuits that carry out addition of numbers.

### HALF ADDER
Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

### FULL ADDER
Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin Carry = AB + ACin + BCin

 ![image](https://user-images.githubusercontent.com/36288975/163552156-a13e5a56-c638-4110-97d9-8896907c8d25.png)

#### Figure -01 HALF ADDER 


![image](https://user-images.githubusercontent.com/36288975/163552057-b3547877-6d07-45b4-b7e0-bcfebfad9e1d.png)

#### Figure -02 FULL ADDER 

### Procedure

Connect the supply (+5V) to the circuit
Switch ON the main switch
If the output is 1, then the led glows.
### 
Program:
```
Program to design a half adder and full adder circuit and verify its truth table in quartus using 
Verilog programming.
Developed by: G Chethan kumar
RegisterNumber: 22005596

HALF ADDER program:

module experimentthree(a,b,sum,carry);
input a,b;
output sum,carry;
xor(sum,a,b);
and(carry,a,b);
endmodule

FULL ADDER program:

module experimenttwo(a,b,c,sum,carry);
input a,b,c;
output sum,carry;
assign sum = ((a^b)^c);
assign carry = ((a&b)|(b&c)|(c&a));
endmodule
```
### Output:
Logic symbol & Truthtable

### TRUTH TABLE:
HALF ADDER:

![Screenshot_20230104_091652](https://user-images.githubusercontent.com/118348224/210482076-b3893768-c4b3-447d-a058-d286fc81de7a.png)


FULL ADDER:

![Screenshot_20230104_092852](https://user-images.githubusercontent.com/118348224/210482104-06e96790-fccb-46dc-b832-0154f20603d1.png)


### TIMING DIAGRAM:
HALF ADDER:

![halfadder2](https://user-images.githubusercontent.com/118348224/210093482-00ca17a0-aed9-4118-8052-220e6ca63b8b.jpg)

FULL ADDER:

![fulladder1](https://user-images.githubusercontent.com/118348224/210093509-3d9b8514-735a-4213-bc10-ad70d9c40750.jpg)

### RTL realization:
HALF ADDER:
![DE_exp02](https://user-images.githubusercontent.com/118348224/210095676-86427dc8-e9fc-4a75-b367-03533b7c5963.png)

FULL ADDER:
![DE_exp002](https://user-images.githubusercontent.com/118348224/210096057-29d39ab2-ad0f-4064-9570-391e087dd7bc.png)

### Result:
Thus, the different digital IC's are studied and the truth table for different logic gates are verified.
