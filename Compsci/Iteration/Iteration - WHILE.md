1. A guessing game program is needed to test the intelligence of students. The Test first loop is ideal for this as the user may guess the number first off. Write a computer program that continues to ask the student to guess a number between 1 and 100 until the secret number is guessed. If they guess wrong, display a message "Bad Guess - Try again". When they guess the correct number, display the Message "You guessed it" and stop the program.
```pseudocode
BEGIN
	rand_num <-- random(1, 100)
	INPUT(guess)
	WHILE guess != rand_num
		OUTPUT("Bad Guess - Try again")
		INPUT(guess)
	ENDWHILE
	OUTPUT("You guessed it")
END
```