#### Functions
- **Functions** are reusable chunks of code that can be referenced throughout the code in order to reduce repetition
	- **User-defined** functions are for specific tasks
	- **Inbuilt** functions (reserved namespaces) exist in most languages, i.e `print` in python
- In a function, there are **arguments** and **parameters**
	- **Arguments** are the actual values passed when a function is invoked
	- **Parameters** are the values that are requested when a function is created


#### Procedures
- **Procedures** are code blocks which peform many tasks, and can be done many times
	- This is different from functions, as procedures can return **multiple** values, with **multiple** arguments, unlike functions
```pseudocode
BEGIN
	FUNCTION Celsius_Convert(temp)
		farenheit <-- (9/5 * temp) + 32
		return farenheit
	END Celsius_Convert

	INPUT(celsius)
	OUTPUT(Celsius_Convert(celsius) + " is the degreeslefoul").

END
```


```
BEGIN
	array <-- []

	FUNCTION binary_search_recursive(array, n)
		length <-- len(array)
		middle = ceil(length / 2)
		IF array[middle] == n THEN
			return True
		ENDIF
		left = array[:middle]
		right = array[middle:]
		return binary_search_recursive(left) and binary_search_recursive(right)
	END binary_search_recursive

	INPUT(n)
	ab <-- binary_search_recursive(array, n)
	IF ab == True THEN
		OUTPUT("It was found.")
	ELSE
		OUTPUT("It was not found.")
	ENDIF
END
```
