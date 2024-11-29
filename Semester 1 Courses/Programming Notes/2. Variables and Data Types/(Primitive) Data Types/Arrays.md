- An array is a collection of data of the same type. Examples:
	- A list of temperature values (doubles).
	- A list of discrete robot positions in a 2D space (int).
	- A list of positions for a drone in 3D space (double).
- Why do we need arrays?
	- To keep tracks of tenths or hundreds of data in memory.
		- How would you name all the variables?
		- How would you process each of the variables?

# Declare and assign an array in 1 line
Creating an array
```CS
String[] cars = {"BMW", "Mustang", "Corvette"};
Console.WriteLine(cars[0]);
```
Output: BMW


Access/Updating an index in an array
```CS
String[] cars = {"BMW", "Mustang", "Corvette"};
cars[0] = "Tesla";
Console.WriteLine(cars[0]);
```
Output: Tesla


# Declare and assign an array in 2 lines
How to declare an array and assign values later. NOTE: 3 is the size of the array which is fixed. This means it can hold 3 indexes. 
```CS
String[] cars = new String[3];

cars[0] = "Tesla";
cars[1] = "Mustang";
cars[2] = "Convette";
```