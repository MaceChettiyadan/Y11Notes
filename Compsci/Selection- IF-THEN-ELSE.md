
1. You are to write a program that will test the eligibility of a person to receive a driving license. The system will ask the user for their name and age via an input box. If the person is 17 years or old the system will display a message “Your are eligible for a license”. If they enter 16 or younger, the system will display the message “You are not old enough for a license”. The system will also print the person’s name and age.

```
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