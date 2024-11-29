# What is a Method?
- Methods, also known as functions, perform a section of code whenever it’s called (invoked).
	- The benefit of using a method is that it lets us reuse code without writing it multiple times.

- Code blocks group together one or more statements enclosed by a pair of curly braces.
- Functions are code blocks that have 3 properties (name associated with it, argument(s) and possibly a return value).


```CS file:"Code block"
{
	statement1;
	statement2;
	...
}
```
```CS file:"Function"
int function_name(args) {
	statement1;
	statement2;
	...
	return value;
}  
```

- C/C#/C++ come with libraries of predefined functions that are very useful.
- Syntax to call a function:
```
function_name(argument_list);
```
`argument_list` is a single or comma separated list:
```
(argument_1, argument_2,..., argument_last)
```

### Parenthesis
- C++ uses parenthesis and a name to identify functions. Remember that parenthesis have several uses.
```
int myfunction(argument) // a function
while(condition) // a loop
for(...) // a loop
int myvar(10) // variable init in C++
(a*b+C/2) // arithmetic expressions
```


# Method Syntax
- When no function is available in libraries, we need to define our own functions.
- First the function has to be declared before it can be used. Then the function can be defined afterwards.
## Method Declaration
- A function declaration is also called as a function prototype.
- Gives a name, a return type and a list of arguments that the function use, it should end with a semicolon ;
- Declarations do not have a body (i.e. no statements)
``` file:"Function Declaration Syntax"
Type_Returned Function_Name(Parameter_List);
```
- The parameter list is also known as an argument list.

### Return Type
- The `return` keyword returns data back to the place where a method is invoked.
- We need to put the data type that we are returning in front of the function name.


Here is an example of a function declaration below. Here we have an example of a function declaration for a function named findMax. It has two arguments of type integer. Notice that we have not given any name to the two arguments, we have only specified the type. We have also specified the return type as integer in the beginning.
```
int findMax(int, int); // function prototype
```







## Function Definition
- Describes how the function does its task.
- This is where the code of the function is actually implemented.
- The function header should have the exact same layout as the function declaration. 
![[Pasted image 20231107134530.png]]




# Method Layout Ordering
- There are two possible ways to write the code for a function in two different ways. 
	- One way includes function prototypes and the second way avoids using function prototypes based where the function is included in relation to the main function.

- In the first way, we include the function prototype before the main function and the function definition after the main function. This is a good programming style.
``` CPP file:"With function prototypes"
int findMax (int, int);//prototype
int main(){
	int x=2, y=5;
	int max = findMax (x, y);
}

int findMax (int x, int y)
{ // start of function body
	int maxnum;
	if (x >= y)
		maxnum = x;
	else
		maxnum = y;
	return maxnum;
}
```
- The other valid way to write the code is to write the function definition before the main function. In this way we do not need to include any function prototype.
``` CPP file:"No function prototypes"
int findMax (int x, int y)
{ // start of function body
	int maxnum;
	if (x >= y)
		maxnum = x;
	else
		maxnum = y;
	return maxnum;
}
int main(){
int x=2, y=5;
int max = findMax (x, y);
}
```



# Method Call Details
- In C++ we have two ways to pass the values of the arguments to the function.
	- The first way is: The values of the arguments are plugged (copied) into the formal parameters (it is called pass-by-value mechanism).
	- The second way is called pass by reference.



