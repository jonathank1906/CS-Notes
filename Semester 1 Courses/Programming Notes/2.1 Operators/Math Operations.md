# Raised to a Power
```CS
double x = 3;
double a = Math.Pow(x, 2);

Console.WriteLine(a);
```
Here we are raising $3^2$. `x` is the base and 2 is the exponent.
Output: 9
# Square Root
```CS
double x = 3;
double b = Math.Sqrt(x);

Console.WriteLine(b);
```
Output: 1.73205.........
# Absolute Value
```CS 
double x = -3;
double c = Math.Abs(x);

Console.WriteLine()

```
Output: 3

# Rounding to closest whole number
```CS
x = 3.14;
double d = Math.Round(x);

Console.WriteLine(d);
```
Output: 3
# Rounding up
Using the ceiling method, we can round up. This always rounds up.
```CS
x = 3.14;
double e = Math.Ceiling(x);

Console.WriteLine(e);
```
Output: 4

# Rounding down
```CS
x = 3.99;
double f = Math.Floor(x);

Console.WriteLine(f);
```
Output: 3

# Finding the largest of two numbers
Here we want to compare two numbers and find the largest number out of the two. It will store the maximum number within another variable called `g`.
```CS
double x = 3.99;
double y = 5;

double g = Math.Max(x, y);
Console.WriteLine(g);
```
Output: 5

# Finding the smallest of two numbers
```CS
double x = 3.99;
double y = 5;

double h = Math.Min(x, y);
Console.WriteLine(h);
```
Output: 3.99