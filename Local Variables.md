>[!SUMMARY]+ Table of Contents
>- [[Local Variables#Naming Variables|Naming Variables]]
>- [[Local Variables#Declaring Variables|Declaring Variables]]
>- [[Local Variables#Initializing Variables|Initializing Variables]]
>   - [[Local Variables#Size|Size]]
>- [[Local Variables#Initialize|Initialize]]
>- [[Local Variables#Declare|Declare]]



First we have to figure out what kind of data that we want to store. If it is a whole number we can use: `int`. However if we want to store a decimal number, an `int` cannot do this so we would need to use a `double`.





- Variables are allocated in memory and must have a type when declared.
- Variables names are also called identifiers.
- Semicolons are necessary to indicate the end of declaration.


> [!NOTE]
> We can only start to use a variable once it has been initialized!



# Naming Variables
- In choosing variable names you must use meaningful names to represent data.
	- The first character must be either:
		- a letter: `myVariable`
		- the underscore character: `_myVariable`
	- The remaining characters must be:
		- letters: `myVariable`
		- numbers: `my123Var`
		- underscore character: `my_var`

# Declaring Variables
- In C# all variables have a type that does not change.
	- In addition, all expressions have a type. For example 2+2 or 7/3 also have a type.
- **Variables must be declared before they are used.
	- This implies that we specify what its type is, along with its name. For example: `int limit`. Here, the type is `int` and the name is `limit`.
	- The best practice is to declare and initialize at the same time. For example: `int limit = 100;`.  Here, the type is `int` and the name is `limit`. We initialized it with `100`.

Creating a variable takes 2 steps (two separate lines of code). Here we declare a variable called `a` and then assign it a value on the next line.
```CPP
int a;
a = 10;
```

We may also declare variables and assign them a value in a single statement:
``` CPP
int a = 10;
```



### Loss of Information
- 2 and 2.0 are not the same type of number.
	- A whole number such as 2 is of type `int` (stored in memory as exact value).
	- A real number such as 2.0 is of type `double` or `float` (stored  in memory as an approximation).


- It is ok to "promote"
	- Put an integer (eg 3) into a float.
- You will be warned if you "demote"
	- Put a floating point number (eg 4.9) into an integer.







# Initializing Variables
- Initially variables may get a random value.
	- Once we assign the variable to some value, we will change its value. The variables location in memory will change according to the new value we have assigned to it. 

``` CPP
bool bcond1 = true;
bool bocond2(false);
```



## Size
- 1 bit is a single digit which can hold either 1 or 0.
- 8 bits = 1 byte



- Char uses only 8 bits = 1 byte



# Local Variables
- Variables declared in a function are local variables and have the function as their scope, cannot be used from outside the function.
``` CPP 
int aFunc(int a) {
	int b=1;
	return a+b;
}
```
- In this example, the local variable here is `b` and it is only accesible inside of the function `aFunc`.
- Variables declared in the main function are also local, have the main as their scope and cannot be used from outside the main.
``` CPP
int main(){
	int i,j;
	double val;
	...
	return 0;
}
```
- In this example, the local variables here are `i`, `j` and `val`. They are only accesible inside of the function `main`.