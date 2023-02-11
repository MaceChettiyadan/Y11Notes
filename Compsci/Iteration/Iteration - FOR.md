- Print the numbers from 1 to 100
```pseudocode
BEGIN
	BEGIN
	FOR n <-- 1 to 100
		OUTPUT(n)
	ENDFOR
END
```
- You have been contracted to write a program that will accept from the user the rainfall (in Millimeters) for each day of the week and then show total and average rainfall for that week.
```pseudocode
BEGIN
	total <-- 0
	FOR day <-- 1 to 7
		INPUT(rainfall)
		total <-- total + rainfall
	ENDFOR
	OUTPUT('Total rainfall was ' + total + ', with an average of ' + (total/7))
END
```
- Write a program that will show a list of the temperatures from 0-20 degrees celcieus in farenheit
```pseudocode
BEGIN
	For celsius <-- 1 to 20
		OUTPUT(celsius + " degrees celsius becomes " + ((celsius * 9/5) + 32) + " farenheit.")
	ENDFOR
END
```
- Factorial values of a number are calculated by multiplying the number, and all the numbers before it, together. So 5!=5x4x3x2x1. Write a program that will calculate the factorial numbers from 2 to 10 and display them in a text box.
```pseudocode
BEGIN
	For n <-- 2 to 10
		OUTPUT(n + ":" + n!)
	ENDFOR
END
```
*alternatively, if the factorial operator is not available to us (nested for, brute force :( but it works);*
```pseudocode
BEGIN
	For n <-- 2 to 10
		output <-- 1
		For i <-- 1 to n
			output <-- output * i
		ENDFOR
		OUTPUT(n + ":" + output)
	ENDFOR
END
```