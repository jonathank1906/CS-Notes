# while Loop Syntax
- When an action must be repeated, a loop is used.
``` 
while (boolean expression is true)
{
	statements to repeat
}
```
- Semi-colons are used only to end the statements within the loop.
- If there is only a single statement in the loop, then we do not have to write the curly braces.
```
while (boolean expression is true)
	statement to repeat
```

- Remember an important difference between while and do-while loops:
	- A while loop checks the Boolean expression at the beginning of the loop.
		- A while loop might never be executed!
	- A do-while loop checks the Boolean expression at the end of the loop.
		- A do-while loop is always executed at least once.