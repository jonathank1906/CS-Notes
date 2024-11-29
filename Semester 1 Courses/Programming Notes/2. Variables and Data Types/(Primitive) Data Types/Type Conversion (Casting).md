# (Implicit) Automatic Type Conversion
- Given the definition
``` CPP
double mpg(double miles, double gallons)
{
	return (miles/gallons);
}
```
What will happen if mpg is called in this way?
`Console.WriteLine((mpg(45, 2) + "miles per gallon");`
The values of the arguments will automatically be converted to type double `(45.0 and 2.0)`.

# (Explicit) Manual Type Casting
- Converting a value to a different data type.
- Useful when we accept user input as different data types can do different things.

## double to int
```CS
double a = 3.14;
int b = Convert.ToInt32(a);

Console.WriteLine(b);
Console.WriteLine(b.GetType());
```
The decimal part is truncated since we are converting from a `double` to an `int`.

## int to double
```CS
int c = 123;
double d = Convert.ToDouble(c);

Console.WriteLine(d);
Console.WriteLine(d.GetType());
```



## int to string 

```CS
int e = 321;
String f = Convert.ToString(e);

Console.WriteLine(f)
Console.WriteLine(f.GetType());
```
Since we have converted this `e` to a string, we can no longer use `f` for any math operations.


## string to char

```CS
String g = "$";
char h = Convert.toChar(g);

Console.WriteLine(h);
Console.WriteLine(h.GetType());
```

## string to bool
```CS
String i = "true";
bool j = Convert.ToBoolean(i);

Console.WriteLine(j);
Console.WriteLine(j.GetType());
```
