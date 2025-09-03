# EXPERIMENT--01-ALP-FOR-8086
# Name : DEEPIKA R
# Roll no: 212223230038 
# Date of experiment : 29-08-25





## Aim: To Write and execute ALP on fundamental arithmetic and logical operations
## Components required: 8086  emulator 
## Theory 
Running The Emulator (emu8086) Intro 8086 Microprocessor Emulator, also known as EMU8086, is an emulator of the program 8086 microprocessor. It is developed with a built-in 8086 assembler. This application is able to run programs on both PC desktops and laptops. This tool is primarily designed to copy or emulate hardware. These include the memory of a program, CPU, RAM, input and output devices, and even the display screen. There are instructions to follow when using this emulator. It can be executed into one of the two ways: backward or forward. There are also examples of assembly source code included. With this, it allows the programming of assembly language, reverse engineering, hardware architecture, and creating miniature operating system (OS). The user interface of 8086 Microprocessor Emulator is simple and easy to manage. There are five major buttons with icons and titles included. These are “Load”, “Reload”, “Step Back”, “Single Step”, and “Run”. Above those buttons is the menu that includes “File”, “View”, “Virtual Devices”, “Virtual Drive”, and “Help”. Below the buttons is a series of choices that are usually in numbers and codes. At the leftmost part is an area called “Registers” with an indication of either “H” or “L”. The other side is divided into two, which enables users to manually reset, debug, flag, etc. What is 8086 emulator emu8086 is an emulator of Intel 8086 (AMD compatible) microprocessor with integrated 8086 assembler and tutorials for beginners. Emulator runs programs like the real microprocessor in step-by-step mode. it shows registers, memory, stack, variables and flags.


 ## Running the Emulator :
1.	Download and install emu8086 (www.emu8086.com) It is usually installed in C:\EMU8086 subfolder in the “Windows” directory
2.	  Run  emu8086 icon (on the desktop or in the c:\EMU8086 folder of window) It has green color 
 
 
3.		write the code for the appropriate program for ADDITION,SUBTRACTION, MULTIPLICATION,  DIVISION operations 

4.	 Compile the program and check for the errors 
5.	Run (once there is no syntax error) 

6.	Click OK to see/view the output of your program on the Emulator screen. 


7.	After running the program, another menu screen will be displayed, where you have the option to “View” symbol table,
8.	 


![image](https://user-images.githubusercontent.com/36288975/189273263-d65baae9-4b8f-4723-afb3-c0ffa4052b04.png)











9.	Click on emulate to start emulation 








![image](https://user-images.githubusercontent.com/36288975/189273273-9bb36ec1-e2e8-4892-8d35-37707332bfdc.png)








10.	If no errors are found click on run the program and check the status of various flags in the flags tab as shown below 






![image](https://user-images.githubusercontent.com/36288975/189273277-113a2a33-4a40-4ff8-95a5-ecd3a1f504fe.png)







## Programs for arithmetic  operations

## Addition  of 8 bit ALP 
```
MOV CL,00
MOV AX,[3001H]
MOV BX,[3003H]
ADD AX,BX
JNC Loop
INC CL
Loop:
MOV [3005H],AX
MOv [3007H],CL
HLT
```
## Output  
<img width="1919" height="1023" alt="Screenshot 2025-08-22 153640" src="https://github.com/user-attachments/assets/d0524c53-2a0f-4632-a46b-16575bd556e2" />
 
## Subtraction   of 8 bit numbers  ALP 
```
MOV CL,00
MOV AX,[3001H]
MOV BX,[3003H]
SUB AX,BX
JNC Loop
INC CL  
NOT AX
INC AX
Loop:
MOV [3005H],AX
MOV [3007H],CL
HLT
``` 
## Output  
<img width="1919" height="1010" alt="Screenshot 2025-08-22 160747" src="https://github.com/user-attachments/assets/3f8e7862-2a0e-454c-9f59-cacbdb080c7e" />

## Multiplication alp 
MOV AX,[3001H]
MOV BX,[3003H]
MUL BX
MOV [3005H],AX
MOV [3007H],DX
HLT
## Output  
<img width="1919" height="1004" alt="Screenshot 2025-08-22 161940" src="https://github.com/user-attachments/assets/51ab719d-a7c8-44ef-8efd-f63312b93eb5" />

## Division alp 
```
MOV AX,[3001H]
MOV BX,[3003H]
DIV BX
MOV [3005H],AX
MOV [3007H],DX
HLT
```
## Output  
<img width="1920" height="1080" alt="Screenshot (46)" src="https://github.com/user-attachments/assets/fe953789-ca72-4ae4-863a-24587b193cd3" />

## Program for logical operators
## AND:
```
MOV AX,[3001H]
MOV BX,[3003H]
AND AX,BX
MOV [3005H],AX
HLT
```
## OUTPUT

<img width="1920" height="1080" alt="Screenshot (52)" src="https://github.com/user-attachments/assets/cff6fa13-9567-4a06-982c-d19ce141d252" />

## NAND:

```
MOV AX,[3001H]
MOV BX,[3003H]
AND AX,BX
NOT AX
MOV [3005H],AX
HLT
```
## OUTPUT

<img width="1920" height="1080" alt="Screenshot (53)" src="https://github.com/user-attachments/assets/67318254-8f7b-4bc0-b5c7-41b7c9f477d8" />


## OR
```
MOV AX,[3001H]
MOV BX,[3003H]
OR AX,BX
MOV [3005H],AX
HLT
```
## OUTPUT

<img width="1920" height="1080" alt="Screenshot (48)" src="https://github.com/user-attachments/assets/19bbbdcd-894f-40e4-88e4-233724f77302" />

## NOR 
```
MOV AX,[3001H]
MOV BX,[3003H]
OR AX,BX
NOT AX
MOV [3005H],AX
HLT
```
## OUTPUT

<img width="1920" height="1080" alt="Screenshot (48)" src="https://github.com/user-attachments/assets/a48b4019-70b5-4308-bfbf-4bca4da1943d" />

## NOT 
```
MOV AX,[3001H]
NOT AX
MOV [3003H],AX
HLT
```
## OUTPUT 

<img width="1920" height="1080" alt="Screenshot (49)" src="https://github.com/user-attachments/assets/cf0a118b-3397-45b0-8796-04a375b4c43b" />

## XOR
```
MOV AX,[3001H]
MOV BX,[3003H]
XOR AX,BX
MOV [3005H],AX
HLT
```
## OUTPUT

<img width="1920" height="1080" alt="Screenshot (50)" src="https://github.com/user-attachments/assets/0e1f9dc8-f252-4103-a5d1-86a925ad3c82" />

## XNOR
```
MOV AX,[3001H]
MOV BX,[3003H]
XOR AX,BX
NOT AX
MOV [3005H],AX
HLT
```
## OUTPUT

<img width="1920" height="1080" alt="Screenshot (51)" src="https://github.com/user-attachments/assets/30460296-3f89-4027-a3f2-119a5b03ed39" />





## Result :
 The program is executed successfully








