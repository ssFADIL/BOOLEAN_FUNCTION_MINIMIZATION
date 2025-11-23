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
![WhatsApp Image 2025-11-23 at 20 12 05_c5574a7b](https://github.com/user-attachments/assets/3ebf4730-f340-4c9c-b57f-bf2ea028366e)
![WhatsApp Image 2025-11-23 at 20 12 08_a768e512](https://github.com/user-attachments/assets/ddcd744a-ca86-4b69-9850-07c8b3efac8d)

**RTL**
![WhatsApp Image 2025-11-23 at 20 12 05_dcbb47d6](https://github.com/user-attachments/assets/287ac8cc-13bd-4fe5-8fc9-a72553cc469c)
![WhatsApp Image 2025-11-23 at 20 12 07_95ac6c72](https://github.com/user-attachments/assets/8244cf4c-fcee-4f2d-ac8b-bd9fc4bd1f2b)

**Timing Diagram**

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

