# Namespaces
- Namespaces can be created in two different ways:
1. Block level namespaces. The namespace is given by a pair of curly braces and what is inside them is defined by the namespace. This way is less modern and not preferred compared to file scoped namespaces.
2. File scoped namespaces. These apply to everything in that particular file. The only difference in terms of syntax is the removal of the curly braces and a semicolon at the end of the namespace.


What are the uses of namespaces?
1. Imagine we have two classes with the same name in a project. If we don’t separate these two classes in their own namespace then there will be an error. We cant have two classes with the same name in the same namespace. 
- We are allowed to have multiple namespaces in a single .cs file.


# Namespace

- Namespaces can have subnamespaces, just like directories have subdirectories. This improves the organizationability.
- One approach is to have the class containing the main method + any other classes in the same file then namespaces are not strictly required. Also, it is not strictly required if the classes are in the same directory.
    - However, it is recommended to use a namespace for better code organization. Furthermore, it helps to avoid naming conflicts and makes the code more maintainable, especially as the project grows.
- However, if we move the other classes (leaving main behind) to another FOLDER then it would be necessary to use a namespace.
    - The namespace is necessary for allowing the classes to reference each other without fully qualifying their names.
- When classes are in different namespaces or no namespace is used, you may need to fully qualify their names to avoid ambiguity and ensure the correct class is referenced.

- This is also when when we want to print out to the console we need to type `System.Console.WriteLine()` . What we are essentially doing is accessing the `Console` class which is inside the System namespace. The System namespace has several different classes and one of those