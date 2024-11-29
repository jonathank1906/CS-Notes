# Input
## Separate line
- `Console.ReadLine();` statement is used in C# to input any primitive data type (`int`, `double`, `char`, `string`) from the keyboard.
## One line
Here we assume the user will enter a some input of type `String`.
`String name = Console.ReadLine()`

If we want read user input and type cast in a single statement.

```CS
Console.WriteLine("What is your age?");
int age = Convert.ToInt32(Console.ReadLine());

Console.WriteLine("You are " + age + " years old");
```


# Output
## Printing strings
`Console.Write("hello");` This will print the statement on the same line. Basically it does not hit the enter key. It does not create a newline.


`Console.WriteLine("Hello");` This will move the cursor to the next line. Similar to endl in c++.


## Printing strings + variables
Here age is a variable of type `int`.
`Console.WriteLine("Your age is " + age);`


## Printing the data type
Here `a` is a variable of type `double`.
`Console.WriteLine(a.GetType());`
The output is: `System.Double`