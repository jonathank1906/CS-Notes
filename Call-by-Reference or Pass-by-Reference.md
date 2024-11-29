


- In many cases we need a sub-task that produce several output values.
	- In pass-by-reference (call-by-reference) parameters allow us to change the variables used in the function call.

- We use the address of operator (ampersand) in order to
# Example 1
- Example of arguments passed by reference.
``` C++ 
void getInput( double& );
void getInput( double& fVariable )
{
	cout << " Convert a Fahrenheit temperature" << " to Celsius.\n" << " Enter a temperature in Fahrenheit: ";
	cin >> fVariable;
}
```
- `&` symbol (ampersand) identifies `fVariable` as a call-by-reference parameter (it means the address of the variable).
	- The ampersand should be used in both declaration and definition! On line 1 we have the declaration of the function and on line 2 we have the definition of the function.

# Example 2 - Moreno
Now lets say that we actually want to modify the actual variable that we are passing into main. We want to manipulate it inside the function and make sure that it is updating inside of main.


``` CPP
#include <iostream>
using namespace std; 

int ReturnValue(int &num1) //pass by value
{
	cout << "In function: " << num1 << endl;
	num1++;
	cout << "In function after modified: " << num1 << endl;
	return num1;
}

int main()
{
	int num1 = 5;
	cout << "Address of num1: " << &num1 << endl;
	cout << "In main: " << num1 << endl;
	ReturnValue(num1);
	cout << "Back in main: " << num1 << endl;
	system("pause");
	return 0;
}
```
Output:
```
Address of num1: FDA
In main: 5
In function: 5
In function after modified: 6
Back in main: 6
```


# Call-by-Reference vs Pass-by-Value


- In the middle column, the memory location of each variable is shown.
- If we use call-by-value

![[Pasted image 20231115112925.png]]