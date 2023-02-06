### Problem
- Draw the flowchart and then write the code for a program that will add 3 numbers entered by the user and then determine if the sum of the numbers is greater than 15. If it is, the prgram will display a relevant message.

```pseudocode
BEGIN
	INPUT(num1) //entering first, second, third numbers by user
	INPUT(num2)
	INPUT(num3)
	IF (num1 + num2 + num3) > 15 THEN //adding the numbers, then checking if the sum is greater than 15
		OUTPUT("It is bigger den da 15")
	ELSE //otherwise;
		OUTPUT("No it not big 15")
	ENDIF
END
```

```python
num1 = float(input("Enter your first number: "))
num2 = float(input("Enter your second number: "))
num3 = float(input("Enter your third number: "))


if (num1 + num2 + num3) > 15:
	print("Big")
else:
	print("Small")
```