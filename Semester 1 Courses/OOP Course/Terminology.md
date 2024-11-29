Attribute(Variable,property,field):
- From an OOP perspective, attribute is the correct term to use.
- Note when referring to a “variable”, this is a location in memory.

Methods/Behavior/Operation:
- In the context of UML class diagrams, we prefer to use the word “operations” to refer to a class’s behaviors.
- In other contexts we can use the word methods or behaviors.


Members: This term is often used broadly to refer to everything that belongs to a class or object, including both attributes (also called fields or properties) and methods (functions).

Member functions: These are functions or methods defined within a class that define its behaviors. They allow objects to perform actions, often by accessing or modifying the object’s attributes. In the Car class, a function like drive() could be a member function, representing the behavior of driving.

# Field vs. property
Attributes(variables) can be either fields or properties. 

- Fields are <u>private</u> and are used just within the class. Like if you need to do a small calculation which no other class needs to see then you use a field.
- By default, an attribute (or member variable) in a class is a field if you declare it directly without any special methods or accessors.
Key Points of Fields:
- Field: If you simply declare a variable inside a class, it acts as a field. It can store data directly and is accessed without any additional logic.
- Default Behavior: There’s no automatic encapsulation or validation unless you implement that functionality manually.
- No Getters/Setters: If you don’t define any get or set accessors, it remains a field.



- A class’s attributes and behaviors are referred to as <u>operations</u> in UML class diagrams.