Tags: #cs #pseudocode #code
# Components of pseudocode

## Variables
it refers to name, assigned to a memory location that would allow to store data and process accordingly.
### Memory locations

| Address | Value |
| ------- | ----- |
| ax101   | 10    |
| bx102   | 20    |
| cx103   | 30    |

a = 10
b = 20

***WAP*** to create a variable and print it on your screen-
```//PSEUDOCODE//
DECLARE Num:INTEGER                                      
NUM <-- 10
OUTPUT "The value is", Num
```
```Python
a = 10
print(a)
```
### Datatypes:
**INTEGER**:  a = 10
**REAL**:  a = 10.5
**STRING**:  a = "10.5"
**CHAR**:  a = "abc"
**BOOLEAN**:  a = TRUE


## Input/Output
***Input*** - It refers to statement that allows the user to input values that can be further used for processing
***Output*** - It refers to a statement that allows to print or display the required information on the screen

>[!question]- ***WAP*** to take an input and output square on screen in pseudocode
>```//PSEUDOCODE//
DECLARE NUM:INTEGER
OUTPUT "Enter a number"
INPUT Num
OUTPUT Num**2

>[!question]- ***WAP*** to take an input and output square on screen in python
>```Python
Num = int(input("Enter a number"))
print(Num^2)


***WAP*** to take a number and print the square in various formats
```//PSEUDOCODE//
DECLARE NUM:INTEGER
OUTPUT "Enter a number"
INPUT Num
OUTPUT "The Square",Num**2
OUTPUT num**2,"is the square"
OUTPUT "The value",Num**2,"is the square"
```
``` Python
Num = int(input("Enter a number"))
print("The square is",Num^2)
print(Num^2,"is the square")
print("The value",Num**2,"is the square")
```

## Conditional Statements
### If pseudocode:
``` //PSEUDOCODE//
IF {CONDITION}
	THEN
		{STATEMENT}
ENDIF

DECLARE Num: INTEGER
Num <- -6
IF Num > 0 
	THEN OUTPUT "Positive"
ENDIF
```
### If python
``` python
if {condition}:
	{statement}
```
### If Else pseudocode
``` //PSEUDOCODE//
IF {CONDITION}
	THEN 
		{STATEMENT}
	ELSE
		{STATEMENT}
ENDIF

DECLARE Num: INTEGER
Num <- -6
IF Num > 0 
	THEN 
		OUTPUT "Positive"
	ELSE
		OUTPUT "Negative"
ENDIF
```
### If Else python
``` python
if {condition}:
	{statement}
elif {condition}:
	{statement}
else:
	{statement}

num = -6
if num>0:
	print("positive")
elif num==0:
	print("Zero")
else:
	print("negative")
```

### Case of pseudocode
``` //PSEUDOCODE//
CASE OF variable
	VALUE 1: {STATEMENT}
	VALUE 2: {STATEMENT}
	VALUE 3: {STATEMENT}
	OTHERWISE: {STATEMENT}
ENDCASE

DECLARE Num:INTEGER
Num <- 2
CASE OF Num
	1: OUTPUT "1"
	2: OUTPUT "2"
	3: OUTPUT "3"
	OTHERWISE: "INVALID"
ENDCASE
```

>[!info]- Case of statement is pseudocode only and is not there in python
>Use if else and elif in python to emulate case of in python




## Iterative Statements
### Components of Iterative Statements
Initialization {start}
condition {end}
increment/decrement {factor}
### For loop pseudocode
```//PSEUDOCODE//
FOR Variable <- {START} TO {END}
	{STATEMENT}
NEXT Variable

DECALRE Const:INTEGER
FOR Const <- 1 TO 10
	OUTPUT "HELLO"
	OUTPUT "HI"
NEXT Const
```
### For loop python
```python
for {variable} in range({start},{end-1}):
	{statement}

for x in range(0,9):
	print("hello")
	print("hi")
```
### Repeat Until loop pseudocode
```//PSEUDOCODE//
VARIABLE <- {START}
REPEAT
	{STATEMENT}
	{CHANGE TO VARIABLE}
UNTIL {COMPARISON BETWEEN VARIABLE AND A CONDITION}

DECLARE Count:INTEGER
Countt <- 1
REPEAT
	OUTPUT "HELLO"
	Count <- Count + 1
UNTIL Count>10
```
### While loop pseudocode
``` //PSEUDOCODE//
Variable <- {START}
WHILE Variable <= 0 DO
	{STATEMENTS}
	Variable <- 
ENDWHILE

DECLARE DECLARE Count:INTEGER
Count <- 0
WHILE Count <= 10
	OUTPUT "HELLO"
	Count <- Count + 1
ENDWHILE
```

### While loop python
``` python
Count = 0
while count <= 10
	print("hello")
	count += 1
```