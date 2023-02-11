
1. You are to write a program that will test the eligibility of a person to receive a driving license. The system will ask the user for their name and age via an input box. If the person is 17 years or old the system will display a message “Your are eligible for a license”. If they enter 16 or younger, the system will display the message “You are not old enough for a license”. The system will also print the person’s name and age.

```pseudocode
BEGIN
	INPUT(name)
	INPUT(age)
	IF age >= 17 THEN
		OUTPUT("You are eligible for a license")	
	ELSE IF age <= 16 THEN
		OUTPUT("You are not old enough for a license")
	ENDIF
	OUTPUT("Output for " + name + ", aged " + age)
END
```
1. You have been contracted to write a Wages Calculator in Visual Basic by Freddy’s Fast Food. Juniors under 18 get $5.60 and hour and the rest get $7.80 and hour. Write a program that asks for the employee’s name, their age, how old they are and how many hours they worked in the past week. It then calculates the wage of the employee based on the age and number of hours worked in a week and displays all relevant information on the screen.

```pseudocode
BEGIN
	wage <-- 0
	INPUT(age)
	INPUT(hours)
	IF age < 18 THEN
		wage <-- (hours * 5.60)
	ELSE
		wage <-- (hours * 7.80)
	ENDIF
	OUTPUT("The wage for " + hours + " hours is " + wage + ".")
END
```