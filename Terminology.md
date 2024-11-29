>[!SUMMARY]- Table of Contents
>- [[Semester 1 Courses/Programming Notes/Other/Terminology#Compilers|Compilers]]
>- [[Semester 1 Courses/Programming Notes/Other/Terminology#Interpreter|Interpreter]]

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


