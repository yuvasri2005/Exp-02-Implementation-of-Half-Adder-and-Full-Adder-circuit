# Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit

# Implementation-of-Half-Adder-and-Full-Adder-circuit
### AIM:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.

### Equipments Required:
Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime
Theory
Adders are digital circuits that carry out addition of numbers.

### Half Adder
Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

### Full Adder
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

Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.


Developed by: K.YUVASRI

RegisterNumber:  212222050061

HALFADDER:

module halfdder(a,b,sum,carry);

input a,b;

output sum,carry;

xor (sum,a,b);

and(carry,a,b);

end module

FULL ADDER:

module fulladder(a,b,c,sum,carry);

input(a,b,c);

output sum,carry;

assign sum=((a^b)^c);

assign carry=((a&b)|(b&c)|(c&a));

endmodule




Logic symbol



![WhatsApp Image 2023-04-20 at 11 25 34 AM](https://user-images.githubusercontent.com/129949620/233272502-cf85b42d-b318-49e8-8629-23626794cec4.jpeg)


 Truthtable
 
 
 


 FULL ADDER
 
 ![WhatsApp Image 2023-04-20 at 11 24 23 AM](https://user-images.githubusercontent.com/129949620/233272015-959e0c99-f284-46d9-84a7-9f65205215be.jpeg)
 
 HALF ADDER
 
 
![WhatsApp Image 2023-04-20 at 11 24 09 AM](https://user-images.githubusercontent.com/129949620/233272038-fe81cc98-af07-4d48-a55e-1c7a3352ac96.jpeg)

 
 

RTL realization

![WhatsApp Image 2023-04-19 at 14 22 54](https://user-images.githubusercontent.com/129949620/233025409-50c0ab34-6135-4233-b9b9-be6f1d028ff8.jpg)
![WhatsApp Image 2023-04-19 at 14 23 03](https://user-images.githubusercontent.com/129949620/233025636-504edc94-032e-426d-8145-682cb10a0de9.jpg)

### Output:
### RTL

### TIMING DIAGRAM

![WhatsApp Image 2023-04-19 at 14 23 34](https://user-images.githubusercontent.com/129949620/233026179-cf0f283e-baea-4f13-9458-45581dd49303.jpg)
![WhatsApp Image 2023-04-19 at 14 23 47](https://user-images.githubusercontent.com/129949620/233026414-bfb4a318-8318-47e5-aa48-ea72ee3f2991.jpg)




### Result:
 Thus the implementation of Halfadder Fulladder Circuit are studied and the truthtable for different logic gates are verified.. 
