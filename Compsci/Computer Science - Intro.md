### Dedicated to our lord, Big C, The C, and without a doubt C, not associated with the language, but a god within himself and himthen upon the hil where the Big C resides..
#### Variables
- Are memory addresses in a computer used to store information so that the CPU may use it, for example, $i=0$
- Variables are temporary. They are usually collected by a garbage collector once their purpose is complete.
	- **Constants** are variables that are immutable - they do not change. For example, $pi=3.14$
	- **Global** and **Local** variables. **Globals** have a global scope (main module). **Local** variables are only acessible in their own module.
See below; code snippet.

``` javascript
const pi = 3.1415 //constant
let temp_local = 0 //variable - in js, let makes it local
var temp_global = 0 //global
```

#### Pseudocode
- **Make sure to include line numbers**
- Used to plan out a program logically (in our mind), breaking down complex programs into step by step logical thingos for human readable
###### Data types
- **For syllabus**
	- Int
	- Float
	- Str
	- Boolean

##### Types of operators
- Arithmetic - + * -*
- Conditional/relational - > < == !=
- Logical -  and or not

#### Pseudocode Example
###### #1
The 'Wilson' Standard (Y10, Mr Wilson)
```pseudocode
BEGIN
	INPUT(num1)
	INPUT(num2)
	total <= num1 + num2
	OUPUT(total)
END
```
The 'Chilson' Standard (Y11, Mr Chillapa)
```pseudocode
BEGIN
	Num1, Num2, Total are float
	INPUT <= Num1, Num2
	READ <= Num1, Num2
	Total <= Num1 + Num2
	Output <= Total
END
```
###### #2
```pseudocode
BEGIN
	num1, num2, num3 are float
	INPUT <= num1, num2, num3
	READ <= num1, num2, num3
	IF (num1 > num2) AND (num1 > num3) THEN
		OUTPUT <= 'The big boy number is the first one'
	ELSE IF (num2 > num1) AND (num2 > num3) THEN
		OUTPUT <= 'The big boy number is the second one'
	ELSE
		OUTPUT <= 'The big boy number is the first one'
	ENDIF
END
```
###### #3 - Python
```pseudocode
a = float(input('First: '))
b = float(input('Second: '))
c = float(input('Third: '))

if (a > b) and (a > c):
    print('First is the largest')
elif (b > a) and (b > c):
    print('Second is the largest')
elif (c > a) and (c > b):
    print('Third is the largest')
else:
	print('They are all of equal magnitude from the digit zero.')
```
