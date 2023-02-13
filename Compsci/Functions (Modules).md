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
Function Celsius_Convert(temp)
	farenheit <-- (9/5 * temp) + 32
	return farenheit
```