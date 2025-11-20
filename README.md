# EXPERIMENT--01-ALP-FOR-8086
# Name :  Deepika R
# Roll no : 212223230038
# Date of experiment : 29/08/2025





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
MOV [3007H],CL
HLT
```



## Output  
 <img width="2876" height="1798" alt="Screenshot 2025-08-22 153906" src="https://github.com/user-attachments/assets/5663c0c5-3c58-4fff-8e03-78ec4968dd05" />

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
<img width="2879" height="1799" alt="Screenshot 2025-08-22 160807" src="https://github.com/user-attachments/assets/912b0228-c2a4-40d5-bb9c-139de3ddc308" />

## Multiplication alp 
```
MOV AX,[3001H]
MOV BX,[3003H]
MUL BX
MOV [3005H],AX
MOV [3007H],DX
HLT
```
 ## Output  
 
<img width="2879" height="1799" alt="Screenshot 2025-08-22 162120" src="https://github.com/user-attachments/assets/7bc3af38-f8d7-4eb4-b1fd-3d010c9a1272" />


## Division alp 
```
MOV AX,[3001H]
MOV BX,[3003H]
DIV BX
MOV [3005H],AX
MOV [3007H],DX
HLT
```


## Output  
<img width="2879" height="1799" alt="Screenshot 2025-08-29 152118" src="https://github.com/user-attachments/assets/02bf1fa9-bb95-4eef-a424-9f9ade7da4d7" />

## Programs for logical  operations

## AND
```
MOV AX,[3001H]
MOV BX,[3003H]
AND AX,BX
MOV [3005H],AX
HLT

```
## Output

<img width="2875" height="1799" alt="Screenshot 2025-08-29 152630" src="https://github.com/user-attachments/assets/11ef3c33-fa82-4370-b74d-10b0cdba5f0a" />

## OR
```
MOV AX,[3001H]
MOV BX,[3003H]
OR AX,BX
MOV [3005H],AX
HLT

```
## Output
<img width="2879" height="1799" alt="Screenshot 2025-08-29 153032" src="https://github.com/user-attachments/assets/7341cc37-f4f0-4f9b-89ba-cb08ac1b6b64" />

## NAND
```
MOV AX,[3001H]
MOV BX,[3003H]
AND AX,BX
NOT AX
MOV [3005H],AX
HLT

```
## Output
<img width="2879" height="1799" alt="Screenshot 2025-08-29 153517" src="https://github.com/user-attachments/assets/7176cbf9-2128-4e8e-9602-e7162250ee5a" />

## NOR
```
MOV AX,[3001H]
MOV BX,[3003H]
OR AX,BX
NOT AX
MOV [3005H],AX
HLT

```
## Output
<img width="2879" height="1799" alt="Screenshot 2025-08-29 153412" src="https://github.com/user-attachments/assets/85a70965-09ca-4e9f-9e9f-37ae076c19ac" />

## NOT
```
MOV AX,[3001H]
NOT AX
MOV [3003H],AX
HLT

```


## Output
<img width="2879" height="1799" alt="Screenshot 2025-08-29 154448" src="https://github.com/user-attachments/assets/1b2775c4-e55c-4af3-8cec-05d0a99e4fe4" />


## XOR
```
MOV AX,[3001H]
MOV BX,[3003H]
XOR AX,BX
MOV [3005H],AX
HLT


```


## Output
<img width="2876" height="1799" alt="Screenshot 2025-08-29 154825" src="https://github.com/user-attachments/assets/d7019d8a-8ab0-4df2-8b57-48e83f6cf752" />


## XNOR
```
MOV AX,[3001H]
MOV BX,[3003H]
XOR AX,BX
NOT AX
MOV [3005H],AX
HLT
```

## Output
<img width="2879" height="1795" alt="Screenshot 2025-08-29 155003" src="https://github.com/user-attachments/assets/dc893205-7ff2-42ec-9d91-15e396021e6d" />







## Result :
We have executed ALP on fundamental arithmetic and logical operations successfully!!!

 








