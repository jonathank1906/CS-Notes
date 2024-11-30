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







# Compilers
- Computer languages have a syntax. Syntax is the set of rules that are used to write correct programs.
- The compiler is in charge of converting the program into machine code. The computer can only understand machine code (1's and 0's).
- The compiler will check the syntax, and if the syntax is correct, it translates the code into machine code (0,1). Otherwise, it generates error(s) messages and stops. The compiler will also try and generate machine code which is as efficient and optimal as possible.


### The process of compilation
![[Pasted image 20231105160538.png|300]]
- The source code is given by the C++ program.
- Preprocessor: Process directives, definitions
- Compiler:
- Linker: The linker will take the program as well as additional code that may be part of the libraries.


# Interpreter (for Python not C++)
- It takes the source code written in Python and uses the compiler to convert it into something called bytecode.
- Interpreters analyze and translate statement by statement. Here we don't have to compile the whole source code, but instead by can interpret it statement by statement.
- Bytecode is an intermediate language that is understood by the virtual machine.


# Programming Environment aka Integrated Development Environment (IDE)
- It is a software program that provides all we need to write and execute computer programs.


