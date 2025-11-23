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
~~~
module funct1(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule
~~~
~~~
module funct2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y & z)|( w & y )|(x & y));
endmodule
~~~


**Output:**
![WhatsApp Image 2025-11-23 at 20 25 25_95c4be3c](https://github.com/user-attachments/assets/acddf5a0-32ac-467e-a9b8-3836345af0f9)

![WhatsApp Image 2025-11-23 at 20 25 25_241e814e](https://github.com/user-attachments/assets/71d72c25-0df5-4503-ab40-aa1fb6bacf1a)


**RTL**
![WhatsApp Image 2025-11-23 at 20 25 26_31b9e323](https://github.com/user-attachments/assets/9b845c0d-30a5-46a1-804f-163e7c4f8e13)
![WhatsApp Image 2025-11-23 at 20 25 27_4da14673](https://github.com/user-attachments/assets/ec39baf8-e734-41bd-b1e8-92969ce6ba5e)

**Timing Diagram**

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

