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

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

```
module EX2(a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;

assign f1 = ((~b & ~d) | (~a & b & d) | (a & b & ~c));
assign f2 = ((~y & z) | (w & y) | (x & y));

endmodule
```

**RTL realization**

<img width="1920" height="1200" alt="Screenshot (57)" src="https://github.com/user-attachments/assets/773d18c5-13db-4343-b12b-48f908104432" />


**Output:**

<img width="1920" height="1200" alt="Screenshot (58)" src="https://github.com/user-attachments/assets/1fb3ee08-dd56-41aa-b701-e5c9154e266a" />

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

