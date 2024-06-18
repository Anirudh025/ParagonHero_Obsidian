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
# Hashing Algorythms
# Floating-point numbers, representation and manipulation
## Floating-point Represention
![[floating point representaion .excalidraw]]


### binary floating point representation
using 8 bits for Mantissa & 8 bits for exponent

| Header | -1  | 1/2 | 1/4 | 1/8 | 1/16 | 1/32 | 1/64 | 1/128 |
| ------ | --- | --- | --- | --- | ---- | ---- | ---- | ----- |
| Binary | 0   | 0   | 0   | 0   | 0    | 0    | 0    | 0     |

| Header | -128 | 64  | 32  | 16  | 8   | 4   | 2   | 1   |
| ------ | ---- | --- | --- | --- | --- | --- | --- | --- |
| Binary | 0    | 0   | 0   | 0   | 0   | 0   | 0   | 0   |

##### Convert Binary to floating point number into denary
| Header | -1  | 1/2 | 1/4 | 1/8 | 1/16 | 1/32 | 1/64 | 1/128 |
| ------ | --- | --- | --- | --- | ---- | ---- | ---- | ----- |
| Binary | 0   | 1   | 0   | 1   | 1    | 0    | 1    | 0     |

| Header | -128 | 64  | 32  | 16  | 8   | 4   | 2   | 1   |
| ------ | ---- | --- | --- | --- | --- | --- | --- | --- |
| Binary | 0    | 0   | 0   | 0   | 0   | 1   | 0   | 0   |
$$ M= \frac{1} 2+ \frac{1} 8 +\frac{1}{16} + \frac {1}{64}$$
$$ M= \frac{32+8+4+1}{64} $$
M = 45/64
M = 0.703125
- Add Exponents values when 1 bit appears
	- E=4
	- M x  2<sup>E</sup>
M = 0.703125 x 2<sup>4</sup>
=11.02

