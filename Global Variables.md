
### Global Variable
Global Variable -- used when more than one function must use a common variable.
	- Declared outside main function.
	- It is better to avoid them as they generally make programs more difficult to understand and maintain.
In the code snippet below `rad` will be available to function volume and main.
``` CS
double rad;
double volume(double);
int main(){...}
```

### Global Named Constant
- Declared outside any function body.
- Declared before any function that uses it.
Example:
``` CS
const double PI = 3.14159;
double volume(double);
int main(){...}
```
- `PI` is available to the main function and to function volume (anywhere in the program).


### Formal Parameters are Local Variables
- Formal Parameters (or arguments) are variables that are local to the function definition.
	- Do NOT re-declare the formal parameters in the function body, they are declared in the function declaration.
``` CS
int area(double sides, int num)
{
	...
}
```
- The pass by value or call-by-value mechanism.
	- When a function is called, the formal parameters are initialized to the values of the arguments in the function call i.e. they are copied.

# Block Scope
- The scope of local variables is the code block (generally defined by the {}) where they are declared.
- The scope of global variables is the whole program.
``` CPP
#include <iostream>
using namespace std;
int main( ){
	int number;
	int a = 2;
	cout << "Enter a number: ";
	cin >> number;
	if (number > 0)
	{
		int a = 1;
		cout << "a=" << a << endl;
	}
	cout << "a=" << a++ << endl;
	return 0;
}
```
The output is:
![[Pasted image 20231107181208.png]]
Explanation:
There are two variables with the same name `a`, however they have different values and are accessible in different parts of the program. The variable `a` which is initialized on line 5 is local to the main function. On line 13 it is a post increment so that means that the value of `a` will be increased AFTER it is printed to the screen or that line is finished.

