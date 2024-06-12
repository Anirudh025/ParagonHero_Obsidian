#cs #code 
# Index
| sr  | Topic                                                             | Fin |
| --- | ----------------------------------------------------------------- | --- |
| 1   | [Constants vs Variables](#Constants-vs-Variables)                 | Y   |
| 2   | [Library Routines (Strings)](#Library-Routines(Strings))          | Y   |
| 3   | [Library Routines (Integer)](#Library-Routines(Integers))         | N   |
| 4   | [[Pseudocode#If Else pseudocode\|If Else]]                        | Y   |
| 5   | [[Pseudocode#For loop pseudocode\|Loops (for)]]                   | Y   |
| 6   | [[Pseudocode#Repeat Until loop pseudocode\|Loops (repeat)]]       | Y   |
| 7   | [[Pseudocode#While loop pseudocode\|Loops (while)]]               | Y   |
| 8   | [Procedures (default)](#Procedures-(default))                     | N   |
| 9   | [Procedures (parameterized)](#Procedures-(Parameterized))         | N   |
| 10  | [[Programming#Default function\|Functions (default)]]             | N   |
| 11  | [[Programming#Parameterized function\|Functions (parameterized)]] | N   |
| 12  | [[Programming#Return function\|Functions (return)]]               | N   |
# Constants-vs-Variables
#### ***Variable***s 
- It refers to a name assigned to a memory location that can hold a value.
- Values stored in variable can change through the execution of the program
#### ***Constants***
It refers to a name assigned to a memory location that can hold a value.
- Values stored in constant remain same throughout execution of program
# Library-Routines(Strings)
##### ***LENGTH(STRING)***
It allows to find the length of the string
``` PSEUDOCODE
a <-- "HELLO"
OUTPUT LENGTH(s)
'''Out
	5
'''
```
##### RIGHT(String,{Number of char})
``` PSEUDOCODE
a <-- "Hello"
OUTPUT RIGHT(a,3)
OUTPUT RIGHT("bye",1)
''' OUT
	llo
	e
'''
```
##### LEFT(String,{Number of char})
``` PSEUDOCODE
a <-- "Hello"
OUTPUT LEFT(a,3)
OUTPUT LEFT("bye",1)
''' OUT
	Hel
	b
'''
```
##### MID(String,{Index},{Number of Characters})
``` PSEUDOCODE
a <-- "Hello"
OUTPUT MID(a,1,2)
OUTPUT MID("bye",2,1)
''' OUT
	He
	y
'''
```
# Library-Routines(Integers)
##### ***INT(Value)***
``` PSEUDOCODE
a <-- 5.2
OUTPUT INT(a)
''' OUT
	5
'''
```
##### ***MOD(Dividend, Divisor)***
``` PSEUDOCODE
OUTPUT MOD(13,2)
''' OUT
	1
'''
```
##### ***DIV(Dividend, Divisor)***
``` PSEUDOCODE
OUTPUT DIV(13,2)
''' OUT
	6
'''
```
# Procedures-(default)
#### Procedures
- It refers to a *self contained* block of code that performs a specific task or set of related tasks
- It allows instructions to be re-usable and modular
- It allows to break down code into smaller manageable pieces
- Variables defined within a procedure have a limited scope
- That means *unlike* functions it cannot return a value
### Example of procedure
![[procedure.excalidraw| 250]]
``` PSEUDOCODE
CALL dhruv
CALL dhruv
CALL dhruv
''' OUT
	Hello
	Bye
	See ya
	Hello
	Bye
	See ya
	Hello
	Bye
	See ya
'''
```
##### Default procedure structure
``` PSEUDOCODE
PROCEDURE {Name}
	Statements 1
	Statements 2
ENDPROCEDURE
CALL {Name}
```

``` PSEUDOCODE
OUTPUT "What do you want to do"
INPUT ch
CASE OF ch
1: CALL dhruv
2: OUTPUT "hehehehehe"
ENDCASE
CALL dhruv
''' OUT
What do you want to do
1 {USER INPUT}|
Hello
Bye
See ya
'''
```

>[!question]- ***WAP*** a procedure to add 2 numbers
> 
> ``` PSEUDOCODE
> PROCEDURE Add
> 	OUTPUT "Enter num 1"
> 	INPUT Num1
> 	OUTPUT "Enter num 2"
> 	INPUT Num2
> 	Result <-- Num1+Num2
> 	OUTPUT Result
> ENDPROCEDURE
> ```

>[!question]- ***WAP*** a procedure to cube a number
>``` PSEUDOCODE
>PROCEDURE Cubie
> 	OUTPUT "Enter a number"
> 	INPUT Num
> 	RESULT <-- `Num**3`
> 	OUTPUT Result
>ENDPROCEDURE

>[!question]- ***WAP*** to ask a user a choice to perform various tasks ![[cs-hw-gdhjksl.excalidraw | 300]]
# Procedures-(Parameterized)
### Parameterized-procedure
It is often useful to pass a value to a procedure that can be used to modify the action(s) taken. For example, to decide how many stars would be output. This is done by passing a parameter when the procedure is called.
### Example
``` PSEUDOCODE
PROCEDURE stars (Number : INTEGER) 
	FOR Counter 1 TO Number 
		OUTPUT"*" 
		NEXT Counter 
ENDPROCEDURE
```

>[!question]- WAP using a parameterized procedure to perform square and one to cube a number
>
>``` PSEDUOCODE
>DECLARE a:INTEGER
>INPUT a
>PROCEDURE Cube(Num)
>	DECLARE b:INTEGER
>	b <-- a * a * a
>	OUTPUT "The cube is", b
>ENDPROCEDURE
>PROCEDURE Sqr(Num)
>	DECLARE b:INTEGER
>	b <-- a * a 
>	OUTPUT "The square is", b
>ENDPROCEDURE
>```


# Functions 
##### Default function
``` PSEUDOCODE
FUNCTION {Name}
	{STATEMENTS}
	{STATEMENTS}
END FUNCTION
CALL {Name}
```
##### Parameterized function
``` PSEUDOCODE
FUNCTION {Name}({variable}:{datatype})
	{STATEMENTS}
	{STATEMENTS}
END FUNCTION
CALL {Name}
```
##### Return function
``` PSEUDOCODE
FUNCTION {Name}({variable}:{datatype}) RETURNS {datatype}
	{STATEMENTS}
	{STATEMENTS}
	RETURN {value}
END FUNCTION

CALL {Name}
VARIABLE <- {Name}({Value})
```

##### Example:
>[!example]- WAP for a function to square number
>``` PSEUDOCODE
>FUNCTION Sqr
>	DECALARE a, result : INTEGER
>	INPUT a
>	result <- a * a
>	OUTPUT result
>END FUNCTION
>
>CALL Sqr
>```
>***OR***
>``` PSEUDOCODDE
>FUNCTION Sqr(a:INTEGER)
>	DECLARE result:INTEGER
>	result <- a * a
>	OUTPUT result
>END FUNCTION
>
>CALL Sqr(5)
>CALL Sqr(9)
>```
>***OR***
>``` PSEUDOCODDE
>FUNCTION Sqr(a:INTEGER) RETURNS INTEGER
>	DECLARE result:INTEGER
>	result <- a * a
>	RETURN result
>END FUNCTION
>
>Var <- Sqr(value)
>```
