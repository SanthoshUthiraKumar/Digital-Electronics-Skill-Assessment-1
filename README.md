# Digital-Electronics-Skill-Assessment-1
### AIM:
To design and simulate the logic diagram using Verilog and validate its output
![Assignment1Question](https://user-images.githubusercontent.com/119477975/212844070-9dae3f6b-217b-44b4-bef7-909eaddb23de.jpg)

### HARDWARE REQUIRED: –
PC, Cyclone II , USB flasher

### SOFTWARE REQUIRED:
Quartus prime

### THEORY
### Introduction
Logic gates are the basic building blocks of any digital system. Logic gates are electronic circuits having one or more than one input and only one output. The relationship between the input and the output is based on a certain logic. Based on this, logic gates are named as

AND gate, OR gate, NOT gate ,NAND gate, NOR gate, Ex-OR gate ,Ex-NOR gate

### Logic Diagram
![Assignment1LG](https://user-images.githubusercontent.com/119477975/212844214-c0113a36-c154-445b-b3ce-97f10e16ef49.jpg)

### Logic Expression 
F=(A'+B').(C'+D').(B'+D)

### Block Diagram
![Assignment1BD](https://user-images.githubusercontent.com/119477975/212849022-9f8fdb09-3ab9-4c40-8c3f-257af990abd7.jpg)

### Produre
### 1. Using AND gate and wires construct the circuit.
### 2. Find RTL Logic for the circuit
### 3. Find Timing Diagram for the Circuit
### 4. End the program

### Program
```
Program to verify the truth table in quartus for the logic gate using Verilog programming.
Developed by: Santhosh U
RegisterNumber: 22009224
module assignment1(A,B,C,D,F);
input A,B,C,D;
output F;
wire Abar,Bbar,Cbar,Dbar,x,y,z;
not(Abar,A);
not(Bbar,B);
not(Cbar,C);
not(Dbar,D);
or(x,Abar,Bbar);
or(y,Cbar,Dbar);
or(z,Bbar,D);
and(F,x,y,z);
endmodule
```

### OUTPUT
### RTL LOGIC
![Assignment1RTL](https://user-images.githubusercontent.com/119477975/212839837-53cc0388-2e23-46e4-b3f0-8c0082b97e8c.png)

### TIMING DIGRAMS
![Assignment1Simulation2](https://user-images.githubusercontent.com/119477975/212840051-19fb7300-2b1c-437c-8286-074db38cd4a7.png)

### TRUTH TABLE
![Assignment1TT](https://user-images.githubusercontent.com/119477975/212840092-85f97624-9fa7-49f5-993a-2445faf793c9.png)

### RESULTS
Thus the given circuit is designed and the truth table is verified using quartus software
