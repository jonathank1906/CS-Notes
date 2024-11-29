- The condition may contain any of the comparison operators:
```CS
x == y  /* x equals y */
x != y  /* x is not equal to y */
x > y   /* x is greater than y */
x < y   /* x is less than y */
x >= y  /* x is greater than or equal to y */
x <= y  /* x is less than or equal to y */
```
- Note that we cannot change the order of the symbols:
	- =! is invalid
	- =< is invalid
	- => is invalid
- We should compare ints to ints and doubles to doubles.




# AND
- C++ allows combining 2 or more comparisons with the and operator.
	- `&&` -- the AND operator
		- True if both expressions are `true`
- Syntax: `(Comparison_1) && (Comparison_2)`
- Example: `if ( (2<x) && (x<7) )`
	- True only if x is between 2 and 7.
	- Inside parentheses are optional but makes it easier to understand.


- Be careful translating inequalities to C++.
- If you want to use `x<y<z`, you should translate it into:
``` CPP
if ((x<y) && (y<z))
```
And NOT `if (x < y < z)`. This is invalid in C/C++.

# OR

- `||` -- The OR operator (not space!)
	- True if either or both expressions are `true`
- Syntax: `(Comparision_1) || (Comparision_2)`
- Example: `if ((x == 1) || (x==y))`
	- True if x contains 1.
	- True if x contains the same value as y.
	- True if both comparisons are true.

# NOT
- `!` -- negates any boolean expression.
	- `!(x < y)`
		- True if x is NOT less than y.
	- `!(x == y)`
		- True if x is NOT equal to y.
- `!` Operator can make expressions difficult to understand so use it only when appropriate.


# Conditional Operator
- The conditional operator is represented by a question mark (?).
- The conditional operator is used in a conditional assignment if a condition is `true` or `false`.

This is the general formula
```
(condition) ? x : y
```
We have some sort of condition or expression. We add a question mark kind of like we are asking a question. Is this true, then do x, if not do y.

```CS
using System;

namespace MyFirstProgram
{
    class Program
    {
        static void Main(string[] args)
        {
            // conditional operator = used in conditional assignment if a condition is true/false

            //(condition) ? x : y

            double temperature = 20;
            String message;

            message = (temperature >= 15) ? "It's warm outside!" : "It's cold outside!";

            Console.WriteLine(message);

            Console.ReadKey();
        }
    }
}
```

# Precedence Rules


