# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

**Logic Diagram**
![Screenshot 2024-11-11 091646](https://github.com/user-attachments/assets/4197afc8-3d2d-4259-8d3d-96274ca76850)



**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

module function2(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule


/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by:Junjar U RegisterNumber:24008873


**RTL realization**


**Output:**


**RTL**
![Screenshot 2024-11-11 092045](https://github.com/user-attachments/assets/29a07398-6032-4f67-b462-8c856eb92b72)


**Timing Diagram**
a	b	c	d	~b	~d	~a	~c	(~b & ~d)	(~a & b & d)	(a & b & ~c)	f1 
0	0	0	0	1	1	1	1	1	0	0	1
0	0	0	1	1	0	1	1	0	0	0	0
0	0	1	0	1	1	1	0	1	0	0	1
0	0	1	1	1	0	1	0	0	0	0	0
0	1	0	0	0	1	1	1	0	0	1	1
0	1	0	1	0	0	1	1	0	1	0	1
0	1	1	0	0	1	1	0	0	0	0	0
0	1	1	1	0	0	1	0	0	1	0	1
1	0	0	0	1	1	0	1	1	0	0	1
1	0	0	1	1	0	0	1	0	0	0	0
1	0	1	0	1	1	0	0	1	0	0	1
1	0	1	1	1	0	0	0	0	0	0	0
1	1	0	0	0	1	0	1	0	1	1	1
1	1	0	1	0	0	0	1	0	1	0	1
1	1	1	0	0	1	0	0	0	0	0	0
1	1	1	1	0	0	0	0	0	1	0	1
![image](https://github.com/user-attachments/assets/1a058786-4378-48ea-b4e0-77fa897ffeed)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

