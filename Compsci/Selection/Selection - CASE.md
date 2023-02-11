### Problems
- A CD manufacturing company charges Multimedia companies $6.50 per CD if they create less than 1000 copies. If the company requires more than 10000, they only pay $5.00 a copy. Otherwise, they pay $5.70 a copy. Write a program that will allow the company to calculate how much to charge for different jobs they do. Use the extended If..Then..Else statement.
```pseudocode
BEGIN
	INPUT(copies)
	price <-- 0
	IF copies < 1000 THEN
		price <-- 6.5
	ELSE IF copies > 10000 THEN
		price <-- 5
	ELSE
		price <-- 5.7
	ENDIF
	OUTPUT(price)
END
```
- Write a program that will display 6 different comments based on the results of random numbers from 1 to 6. Use the Select Case statement.
```pseudocode
BEGIN
	num <-- random(1,6)
	CASE num OF
		1: OUTPUT("It is 1")
		2: OUTPUT("It is 2")
		3: OUTPUT("It is 3")
		4: OUTPUT("It is 4")
		5: OUTPUT("It is 5")
		6: OUTPUT("It is 6")
	ENDCASE
END
```
- Most countries use a sliding scale income tax program based on the amount of money earned. Write a CASE program for the Tax Office that accepts an income and calculate the tax payable.
```pseudocode
BEGIN
	INPUT(income)
	tax_payable <-- 0
	CASE income OF
		<200: tax_payable <-- 0
		>=200 and <900: tax_payable <-- 28 * (income - 100)
		>=900 and <1800: tax_payable <-- 112 + (32 * (income - 500))
		>=1800 and <3000: tax_payable <-- 196 + (46 * (income-1000))
		>3000: tax_payable <-- 656 + (60 * (income-2000))
	ENDCASE
	OUTPUT(tax_payable)
END
```
