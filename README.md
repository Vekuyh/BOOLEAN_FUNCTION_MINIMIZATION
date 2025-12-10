# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Logic Diagram**

<img width="320" height="193" alt="Screenshot 2025-11-20 185008" src="https://github.com/user-attachments/assets/e043bf8b-1f22-443e-97c5-3db4ed763deb" />


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
 Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 
~~~
module ex2 (a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
assign f1 = ~a&~b&~c&~d | a&~c&~d | ~b&c&~d | ~a&b&c&d | b&~c&d;
assign f2 = x&~y&z | ~x&~y&z | ~w&x&y | w&~x&y | w&x&y;
endmodule
~~~

Developed by:VENKATESH P
RegisterNumber:25011427


**RTL realization**
<img width="1920" height="1080" alt="Screenshot (31)" src="https://github.com/user-attachments/assets/a3aa1c52-e868-44a3-ac2a-45ebdbbbe26c" />


**Output:**

**RTL**
**Timing Diagram**
<img width="1920" height="1080" alt="Screenshot (32)" src="https://github.com/user-attachments/assets/eefad412-b938-4d59-8d78-abb568554b6f" />




**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.
