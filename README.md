# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**
To implement the given logic function verify its operation in Quartus using Verilog programming.
F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 
F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Truth table:**

![image](https://github.com/user-attachments/assets/db0496dc-d463-464c-9d42-d4c473ea3f56)

![image](https://github.com/user-attachments/assets/0f13d77d-7d40-44fd-b37f-98b12cd491f9)


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
```
Developed by: T.Hudaifa Mahzumia
RegisterNumber: 212224040119
````
```
module EXP2(a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
assign f1=((~b&~d)|(~a&b&d)|(a&b&~c));
assign f2=((~y&z)|(x&y)|(w&y));
endmodule
```


**Output:**
![image](https://github.com/user-attachments/assets/24c2d5ae-57ce-4596-93b4-8d725a164ea1)

**RTL**
![image](https://github.com/user-attachments/assets/08cb07e9-a853-4cea-a1cf-68b154ce0abf)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

