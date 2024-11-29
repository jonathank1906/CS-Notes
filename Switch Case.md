- A switch statement's controlling expression must return one of these types:
	- A boolean value.
	- An integer type.
	- A character.
	- An enumeration.
- Note: float or double are not allowed in a switch statement.

- The value returned when the controlling expression is evaluated, is compared to the constant values after each "case".
	- When a match is found, the code for that case is used.

### default:
- Executed when no case is matched.



### The break Statement
- The break statement ends the switch-statement.
	- Omitting the break statement will cause the code for the next case to be executed!.
	- Omitting a break statement allows the use of multiple case lables for a sectoin of code. For example this code snippet below runs the same code for either 'A' or 'a':
``` 
case 'A':
case 'a':
	cout << "Excellent.";
	break;
```


- When should we use multiway if statements or switch statement?
	- There is no general rule, but some recommendations are:
		- Use multibranch if statement when the number of if-else statements is few (less than 4).
		- When there is more than 4 then it is better to use s switch statement.
	- The goal is to make the code easier to read.