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

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by:J.JANANI

RegisterNumber:212223230085

module Boolean_min(a,b,c,d,w,x,y,z,f1,f2);

input a,b,c,d,w,x,y,z;

output f1,f2;

wire adash,bdash,cdash,ddash,ydash,p,q,r,s,t,u;

not(adash,a);

not(bdash,b);

not(cdash,c);

not(ddash,d);

and(p,bdash,ddash);

and(q,adash,b,d);

and(r,a,b,cdash);

or(f1,p,q,r);

not(ydash,y);

and(s,ydash,z);

and(t,x,y);

and(u,w,y);

or(f2,s,t,u);

endmodule

*/


**RTL realization**


![317130974-fe3258fd-94b7-4238-ad7b-f9e6d54ed3e1](https://github.com/Janani23014108/BOOLEAN_FUNCTION_MINIMIZATION/assets/146822085/ed0a02df-af06-4be3-a4cc-42bdf4377f7e)


**Output:**
![317131331-b64b8f56-f0b8-4107-bb74-5bd38397f894](https://github.com/Janani23014108/BOOLEAN_FUNCTION_MINIMIZATION/assets/146822085/34f46340-3542-4189-9fe1-5b9af8c9a065)

**RTL**


**Timing Diagram**

![317131214-7d7bb703-e9d8-42e7-83e6-b2056b92a088](https://github.com/Janani23014108/BOOLEAN_FUNCTION_MINIMIZATION/assets/146822085/c0c5a374-5717-4153-80eb-639333dc2d34)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

