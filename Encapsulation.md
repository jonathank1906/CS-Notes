- Encapsulation refers to the concept of bundling data (attributes or fields) and methods that operate on that data into a single unit.
- Hiding the internal state and functionality of an object and only allowing access through a public set of functions.


# Getters and Setters
[Get and set video](https://www.youtube.com/watch?v=8FmE_-QXg3Y&t=175s)
## Properties 
- Properties are like special operations that allow you to control how a field’s value is accessed or modified.
- Properties in C# are a way to encapsulate fields within a class and provide controlled access to them.
- Properties allow you to define different access levels for getting and setting data, which provides an essential way to implement encapsulation. 
- They allow us to define custom logic for reading (get) and writing (set) the values of fields.


Example of a `LibraryBook` class:
- You might have a public getter method for title and author to allow users to read these values.
- You could provide a setter method for title and author to control how changes are made. This can include validations or checks before making changes.
