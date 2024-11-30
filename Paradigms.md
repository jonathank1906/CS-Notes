- Until now we have been doing something called procedural programming. This means that programs are built around the idea in which they follow a sequence of instructions.
- With OOP we are able to create our very own data types.
- An example of an object in OOP could be car. If you think of a car, it can be considered as an object and it is composed of many parts. For example, it has an entire, a transmission, wheels, and an interior.
- So far you have been creating procedural programs. So what is a procedural program? In procedural programming you create variables using the basic data types and these variable are then manipulated by functions. 
	- Let’s suppose that you want to keep track of all of the classes you are taking at BHS. More precisely you want to keep track of all your assignments, quizzes, and tests. Now let’s suppose that you want to get the averages for your homework, in class assignments, quizzes, and tests. You then want to calculate the weights for each category in order to determine the grade you have. Using procedural programming you would probably create many variables including arrays to store multiple subjects, and assignments. You would then have to create functions in which you can pass in the grades you received for the different assignments. The function would then add up all the scores, divide the sum by how the amount of assignments you have completed and then return the average. By using this approach your program would become large and difficult to maintain.
- Now let’s take a look at Object Oriented Programming: With OOP you can recreate the program above by creating an object (an object of type student). If you sit down and think of your surroundings you will find out that an object is composed of several parts. In our example we can think of the object as a Gradebook. A gradebook has different categories such as:
1. Homework
2. In class assignments
3. Quizzes
4. Tests
- Each category in turn has a point value whether it is a homework assignment or a test. By grouping all of these categories into one we can create variables and member functions that can set, get, and manipulate the information as one object.



All programs can be created by using the following three basic structures:
1. Procedural (also called sequence). This is when our code executes from top to bottom, or in other words, one statement after another. These type of programs are not very smart or useful as they are not able to make any decisions.
2. Decision (also called selection). This is where we are able to control the flow of our program by using for example if statements. At this point, our programs appear to be a bit smarter because they have the ability to make decisions.
3. Repetition (also called looping)



# Top-Down Design
- Computer programming is about problem solving.
- The problem you are trying to solve can be complex, therefore it is always better to divide the problem into subproblems. It will be easier to implement the subproblems and if the subproblems are still difficult then we can sub divide it into subproblems. We can keep on doing this subdivision until the problem is simple to solve. 
- We will then start solving the subproblems and working our way to the original problem.
In other words:
- The "art" of computer programming using the top-down approach consists in:
	- Finding a good decomposition of a problem into subproblems.
		- Subproblems can be decomposed further into smaller subproblems.
		- You keep decomposing until subproblems are small enough that could be implemented as functions.
- Subproblems will be implemented as functions in C++.

![[Pasted image 20231107114109.png]]

- Breaking a problem into subproblems or functions, has many advantages, it makes programs easier to:
	- understand
	- change
	- write
	- test
	- debug
	- for teams to develop


