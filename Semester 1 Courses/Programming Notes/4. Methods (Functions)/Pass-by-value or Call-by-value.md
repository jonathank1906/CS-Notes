- When we create functions, we pass in our variables/arguments into the function. When we pass a variable into a function, what we are doing is passing-by-value. We are creating a copy of the variable (value of the variable) that we are passing into the function. 
	- The variables/parameters that are in the function, those now have a copy inside to work with the information.
	- If you modify the variable inside of the function, you are not actually modifying the function inside of main.

- This is one way in which we do this is, there is also another way called 
 
 
 Pass-by-value (call-by-value) copies the values in the function call to the arguments in the called function.
 - Pass-by-value creates a copy of the variable being passed in.
	- The function will return only a single value.



In this example below, we would like to increase the value of num1 by 1 by using the `ReturnValue` function.
``` CPP
#include <iostream>
using namespace std; 

int ReturnValue(int num1) //pass by value
{
	cout << "In function: " << num1 << endl;
	num1++;
	cout << "In function after modified: " << num1 << endl;
	return num1;
}

int main()
{
	int num1 = 5;
	cout << "In main: " << num1 << endl;
	ReturnValue(num1);
	cout << "Back in main: " << num1 << endl;
	system("pause");
	return 0;
}
```
Output:
```
In main: 5
In function: 5
In function after modified: 6
Back in main: 5
```

Explaination of the example code:
- Even though the two variables on lines 4 and 14 have the same name, `num1`, they are not the same variable, they are two different variables. Each variable is local to its respective function. The variable does not exist 
- You cannot access one of these variables from another function, unless you have created a global variable, but that is not the recommended way to do it.
	- The `num1` variable created on line 14 is local to main only. If we wanted to access this `num1` inside of the `ReturnValue` function then we would