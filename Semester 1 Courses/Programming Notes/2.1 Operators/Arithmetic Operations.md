- C/C#/C++ provides some simple primitive arithmetic operators such as:
	- + (sum)
	- - (subtraction)
	- * (multiplication)
	- / (division)
- C/C#/C++ provides other operators like modulus, and, or, negation (%,&,|,~)


# Increment and Decrement
- Unary operators require only one operand.
	- + in front of a number such as +5.
	- - in front of a number such as -5.


- There are other unary operators in C/C#/C++.
	- ++ increment operator.
		- Adds 1 to the value of the variable.
		- `x++;` is equivalent to `x=x+1;`
	- -- decrement operator.
		- Subtracts 1 from the value of a variable.
			- `x--;` is equivalent to `x=x-1;` 
- There is also pre and post increment as well as pre and post decrement.


# Operator Shorthand Notation
- C/C#/C++ contains shorthand operators for some common expressions. All arithmetic operators can be used this way.

```CS
// +=
count = count + 2 // becomes: 
count += 2;

// -=
count = count - 2; // bocmes:
count -= 2;

// *=
bonus = bonus * 2; //becomes:
bonus *= 2;

// %= 
remainder = remainder % (cnt1 + cnt2); //becomes
remainder %= (cnt1 + cnt2);
```
