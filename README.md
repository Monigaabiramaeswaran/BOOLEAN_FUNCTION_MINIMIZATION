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
module logic_functions(
input  a, b, c, d,
input  w, x, y, z,
output f1, f2
);

assign f1 = (~b & ~d) |
            (a & b & ~c) |
            (~a & b & d);

assign f2 = (~y & z) | (w & y);
endmodule



``` 

Developed by:A.MONIGA
RegisterNumber:25017526

**Logic symbol & Truthtable**

![logicgateabcd](https://github.com/user-attachments/assets/6d9a1aab-f3f5-436c-9ef1-7f66a5a985a7)
![logicgatewxyz](https://github.com/user-attachments/assets/13c4abed-c890-4297-8f7b-842eec41923e)


**RTL realization**

<img width="564" height="377" alt="Screenshot 2025-11-26 134930" src="https://github.com/user-attachments/assets/c10ef504-91fc-4709-90d8-a7e0c3df68c2" />


**Output:**
<img width="1920" height="1080" alt="Screenshot (62)" src="https://github.com/user-attachments/assets/ac93d76a-dd54-424c-84d5-09a037f4f0f5" />

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

