- A simpler way to iterate over an array, but it’s <u>less flexible</u> compared to an ordinary for loop.
	- With a for loop, we can iterate forwards, backwards, or even skip iterations.


```CS
String[] cars = {"BMW", "Mustang", "Convette"};

foreach (String car in cars)
{
	Console.WriteLine(car);
}
```
Output: 
BMW
Mustang
Convette