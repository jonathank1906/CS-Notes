# Overloading Method Names
- C/C#/C++ allows more than one definition for the same function name. This is called overloading.
	- Very convenient for situations in which the "same" function is needed for different number or types of arguments.
- Overloading a function name means providing more than one declaration and definition using the same function name.
### Example
``` CPP
double ave(double n1, double n2)
{
	return ((n1 + n2) / 2);
}
double ave(double n1, double n2, double n3)
{
	return ((n1 + n2 + n3) / 3);
}
```
- The compiler checks the number and types of arguments in the function call to decide which function to use.
- `cout << ave(10, 20, 30);` uses the second definition because it has 3 arguments.

# Overloaded Method Check
  - Overloaded functions (functions with same name).
	- Must have <u>different</u> number of formal parameters (arguments).
	  AND / OR
	- Must have at least one different type of parameter.

	- Must return a value of the same type.


