# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

Boolean function minimization is the process of simplifying a Boolean expression to its most basic form, using the fewest logic gates, variables, and operators. This is critical for digital circuit design as it leads to more efficient, faster, and cheaper circuits by reducing complexity, power consumption, and manufacturing costs. Key methods for achieving minimization include algebraic manipulation and the use of a Karnaugh map (K-map). 

**Logic Diagram**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

module ex2(a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
assign f2=((~y & z)|(w & y)|(x & y));
endmodule

**RTL realization**

<img width="670" height="659" alt="exp2" src="https://github.com/user-attachments/assets/683b3775-c702-4ddc-ba2d-2f99c6f474a5" />


**Output:**

<img width="1920" height="1080" alt="exp 2" src="https://github.com/user-attachments/assets/b5d3937f-d937-41e0-be37-4297282ba10a" />


**RTL**

**Timing Diagram**

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

