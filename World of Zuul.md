- Creating the map

# Game.cs

## Play()
1. Create a new parser object `Parser parser = new();` What really happens when you call `new()`? We can consider `Parser` as the data type and `parser` as the object’s name. We are creating a new instance of the Parser class. Notice that we are not passing in any arguments inside the parenthesis.

While loop
1. `Console.Writeline(CurrentRoom?.ShortDescription)`
	- `ShortDescription` is part of the Room class in the Room.cs file. the ? indicates that this object is a nullable type. So at the start of the program it will hold null. The ? mark always goes in front of the data type or the object type.
	- The `CurrentRoom` by default is Outside.

The input is stored on a separate line. Then this input is used in order to determine which command it corresponds to (which one it matches) from the list of allowed commands.

# Parser.cs
The goal of the Parser class is to process user input and convert it into commands that can be understood and executed by the system
## GetCommand()
1. split is used to convert the input into sepearate words in an array. the words are split by space. for example “hello world” would be stored as words[0] = “hello”, words[1] = “world”.

returns null if the word is not on the list of valid commands.
# Program.cs
1. Create a new game object
# Room.cs


# Command.cs





# CommandWords.cs
The List<string> stores these commands, and the get accessor allows you to access the list but not modify it, ensuring that the valid commands remain constant throughout the game.
