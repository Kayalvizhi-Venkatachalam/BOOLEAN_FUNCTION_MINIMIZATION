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
/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by:Kayalvizhi.V.M 
RegisterNumber:25018055*/
F(A,B,C,D)=AB+CD+AD

module boolean_function_4var (
    input  wire A,
    input  wire B,
    input  wire C,
    input  wire D,
    output wire F
);

assign F = (~A & B) | (C & D) | (A & ~D);

endmodule
~~~


**RTL realization**
<img width="1539" height="805" alt="Screenshot 2025-11-27 224914" src="https://github.com/user-attachments/assets/7f9a128b-184e-4726-bea9-9d9fe4399591" />



**Timing Diagram**
<img width="1889" height="927" alt="Screenshot 2025-11-27 230335" src="https://github.com/user-attachments/assets/a35fbf7b-a13f-4b65-8ad6-43cd550ddcfc" />


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

