---
Status: incomplete
Subject: CS
---
## Non Composite Data Types
###### Datatypes 
> [!tip]- What do datatypes do? 
> They store the amount and type of data depending on need of programmer
``` PSEUDOCODE
//Example of datatype usage INT//
DECLARE Num1: INTEGER
Num1 <-- 1
```
#### Enumerated Data type:
1. A non-composite data type defined by a given list of all possible values that has an implied order
2. Contains no references to other datatypes
3. Type name usually begins with the letter T
##### `TYPE` - create your own datatypes
###### Use cases:
1. Stores specific values only
2. 
``` PSEUDOCODE
TYPE Tweek = (1,2,3,4)
//created our datatypes//
DECLARE CurrentWeek: Tweek
Tweek <-- 2 //can only be the values specified above 1,2,3,4// 
```
#### Pointer Data Type: 
1. A non-composite data type that references the memory address of where the data is stored.
	- It used to refer to a memory location
>[!example]-  Example of pointer
> ``` PSEUDOCODE
DECLARE Num1: INTEGER
Num1 <-- 10``` 
So in this case a table is created to store the value of Num1
| Addr  | Value |
| ----- | ----- |
| x1010 |       |
| x1011 |       |
| x1012 | 10    |
A pointer value instead of containing `10` contains the address of the value `x1012` 
for example ```PointerName <-- ^Num1  ```

There are 2 types of pointers
1. Datatype _(Used much more often)_ 
2. Variable
```PSEUDOCODE
TYPE TweekPointer = ^Tweek
DECLARE CurrentWeekPointer: TweekPointer
CurrentWeekPointer <-- ^CurvWeek //Normal referencing//
CurrentValue <-- CurWeek^ //Dereferencing//
```

| Datatype pointer                           | Variable Pointer                 |
| ------------------------------------------ | -------------------------------- |
| ```Datatypepointer = ^Datatype ```         | <>                               |
| ```DECLARE PointerName:Datatype Pointer``` | <>                               |
| ```PointerName <-- ^VariableName```        | ```Value <-- VariableName^```    |
| References to the location                 | Dereferences to the value itself |

| Variable | Datatype | Location            | Value |
| -------- | -------- | ------------------- | ----- |
| CurrWeek | Tweek    | x1010, x1011, x1012 | 2     |

## Composite Datatypes
Composite Datatype: Datatype that refers to other data types in its defination

![[Compositedatatypes.excalidraw|450]]
#### Records
1. Uses a header and variable to keep data
>[!example] A record looks like: 
>```PSEUDOCODE
TYPE
StudentRecord
DECLARE Name:STRING
DECLARE Age:INTEGER
DECLARE Address:STRING
ENDTYPE```
#### Sets
Set :: List of worded elements that can use set theory operations such as union, intersection, etc.
>[!example] A Set looks like:
>```PSEUDOCODE
>DECLARE NEven = SET OF INTEGER
>//to declare a variable use define instead of declare and add a bracket with values//
>DEFINE EvenNums(2,4,6,8):NEven
>```

# File Organization and Access
## File Organization
![[File Organization.excalidraw|850]]
## File Access
![[File access.excalidraw|700]]
# Hashing Algorithms
# Floating-point numbers, representation and manipulation
## Floating-point Represention
![[floating point representaion .excalidraw]]


### Binary floating point representation
using 8 bits for Mantissa & 8 bits for exponent

| Header | -1  | 1/2 | 1/4 | 1/8 | 1/16 | 1/32 | 1/64 | 1/128 |
| ------ | --- | --- | --- | --- | ---- | ---- | ---- | ----- |
| Binary | 0   | 0   | 0   | 0   | 0    | 0    | 0    | 0     |

| Header | -128 | 64  | 32  | 16  | 8   | 4   | 2   | 1   |
| ------ | ---- | --- | --- | --- | --- | --- | --- | --- |
| Binary | 0    | 0   | 0   | 0   | 0   | 0   | 0   | 0   |

##### Convert Binary to floating point number into denary
>[!example]- Mantissa Solving Example:
>Mantissa:
>
>| Header | -1  | 1/2 | 1/4 | 1/8 | 1/16 | 1/32 | 1/64 | 1/128 |
>| ------ | --- | --- | --- | --- | ---- | ---- | ---- | ----- |
>| Binary | 0   | 1   | 0   | 1   | 1    | 0    | 1    | 0     |
>
>Exponent:
>
>| Header | -128 | 64  | 32  | 16  | 8   | 4   | 2   | 1   |
>| ------ | ---- | --- | --- | --- | --- | --- | --- | --- |
>| Binary | 0    | 0   | 0   | 0   | 0   | 1   | 0   | 0   |
>
>$M= \frac{1} 2+ \frac{1} 8 +\frac{1}{16} + \frac {1}{64}$
>$M= \frac{32+8+4+1}{64}$
>$M = \frac{45}{64}$
>$M = 0.703125$
>- Add Exponents values when 1 bit appears
>	- $E=4$
>	- $M \times 2^E$
>$M = {0.703125}  \times  {2^4}$
>$=11.02$

##### Solved Examples

>[!question]- Mantissa question 1
>Mantissa:
>
>| -1  | <>  | 1/2 | 1/4 | 1/8 | 1/16 | 1/32 | 1/64 | 1/128 |
>| --- | :-: | --- | --- | --- | ---- | ---- | ---- | ----- |
>| 0   | <>  | 0   | 1   | 0   | 1    | 0    | 0    | 0     |
>Exponent:
>
>| -128 | 64  | 32  | 168 | 8   | 4   | 2   | 1   |
>| ---- | --- | --- | --- | --- | --- | --- | --- |
>| 0    | 0   | 0   | 0   | 0   | 0   | 1   | 1   |

>[!answer]- Answer 1
>
>$M= \frac{1}{4} + \frac{1}{16}$
>$M=\frac{5}{16}$
>$E=2+1$
>$E=3$
>$M \times 2^E$
>$\frac{5}{16} \times 2^3$
>$\frac{5}{16} \times 8$
>$=2.5$

>[!question]- Mantissa question 2
>Mantissa:
>
>| -1  | <>  | 1/2 | 1/4 | 1/8 | 1/16 | 1/32 | 1/64 | 1/128 |
>| --- | :-: | --- | --- | --- | ---- | ---- | ---- | ----- |
>| 1   | <>  | 1   | 0   | 0   | 1    | 1    | 0    | 0     |
>Exponent:
>
>| -128 | 64  | 32  | 16 | 8   | 4   | 2   | 1   |
>| ---- | --- | --- | --- | --- | --- | --- | --- |
>| 1    | 1   | 1   | 1   | 1   | 1   | 0   | 0   |

>[!answer]- Answer 2
>$M= - 1 + \frac{1}{2} + \frac{1}{16} + \frac{1}{32}$ 
>$M = -1  + \frac{16+2+1}{32}$
>$M=-1 +\frac{19}{32}$
>$M = \frac{-13}{32}$
>$E = -128+64+32+16+8+4$
>$E = -4$
>$M \times 2^E$
>$=\frac{-19}{32} \times 2^{-4}$
>$= \frac{-13}{512}$
>$= -0.0254$

###### Convert  denary numbers into binary floating-point numbers
>[!example]- Convert $4.5_{10}$ to binary floating point
>$4_{10}$ to binary is $0100$
>but for 0.5 we do 
>$0.5\times 2$ 

>[!example]- Convert $89.3043_{10}$ to binary floating point
>$89.3043_{10}$ --$Binary$--> $01011001_{2}$
>![[binary-floating-point-explainer.excalidraw]]
>![[Mantissa and exponent.excalidraw]]
>

>[!question]- Convert $73.2062_{10}$ to binary floating point
>$73_{10}$ --$Binary$--> $01001001_{2}$
>multiplication of 0.2062 gives 0010
>01001001.0010
>0.10010010010 $\therefore$ Exponent of 0111 (7 shifts)
>010010010010
>





