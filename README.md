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
```
Developed by: PRIYA DHARSHINI R
RegisterNumber:212224050033*/
```
```
module exp_2a (a,b,c,d,f1);
input (a,b,c,d);
output (f1);
assign f1=((~a&b&d)|(a&b&~c)|(~b& ~d));
endmodule
```
```
module exp_2b(w,x,y,z,f2);
input(w,x,y,z);
output f2;
assign f2=((x&y)|(~w&y)|(~y&z));
endmodule
```


**RTL realization**

![WhatsApp Image 2025-03-27 at 23 44 57_e323bc49](https://github.com/user-attachments/assets/024a6f4c-1b7a-4663-a48b-0031f49d4d3a)

![WhatsApp Image 2025-03-27 at 23 44 48_d721f65b](https://github.com/user-attachments/assets/c22c9819-1e06-4478-88b3-550ee4533a44)


**RTL**

![exp_2a LG](https://github.com/user-attachments/assets/d410bfb5-6089-4b1f-835e-56da622955dc)

![exp 2-b LG](https://github.com/user-attachments/assets/e0f26477-6d92-493a-b6f2-1012fb945146)


**Timing Diagram**

![exp_2a WF](https://github.com/user-attachments/assets/3043bd4f-fc67-4d78-89cc-f3fa9058724e)
![exp_2b WF](https://github.com/user-attachments/assets/9bf8e1b8-8713-4c49-9911-39f956b3dd68)




**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

