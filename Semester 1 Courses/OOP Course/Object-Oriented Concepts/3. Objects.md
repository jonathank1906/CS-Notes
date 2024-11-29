# What is an Object?
- Each object has two main components: attributes and behaviors. Keep in mind that it is the class that sets up the general template of this object and the object holds the specific attributes and behaviors.
- Every object belongs to a specific class or type. In other words, an object is an <u>instance</u> of a class.
- An object represents a real-world entity(physical or abstract) and encapsulates data and behavior.



## Attributes (Variables)
- Attributes define the details of a particular object.
- To manage access to attributes, you often use getter and setter methods.


Example attributes of a car:
- The make 
- The model
- The color

Example attributes of a microwave:
- Power level
- Timer setting
- Brand
## Behaviors/Methods
- Behaviors describe the actions that can be performed on the object, or by the object.
- Behaviors are typically more complex than attributes because they can include rules and logic for interacting with a class. For instance, while color is a simple attribute of a ball, the behavior of rolling a ball involves multiple factors like friction and force. 

Methods consist of two main parts: the method signature and the method body:  
- Method Signature: This is the line that declares the method, including the access modifier, return type, method name, and any parameters. For example, the method signature for the Throw() method is formatted like the following: public void Throw(float speed, float angle). 
- Method Body: The method body is enclosed in curly braces {} and contains the code that performs the actions defined by the method.

Example behaviors of a microwave: 
- Start
- Stop
- Make popcorn 

# Abstract Objects
- OOP lets us model abstract concepts or things that don't have a physical form which we cant physically touch. 
- Our goal is to be able to represent and manage this real-world system.

Example of an online ordering system in a web shop: 
- It's not something that we can hold, but it's still an object with attributes like an order number, the total price, and the customer's name.
- It has behaviors like processing the payment, canceling the order, or issuing a refund. 




# How to Create an Object?
- An object or instance of a class is created by using the `new` keyword.

```CS "test"
Burger cheeseburger = new Burger();
// If a class is a recipe, then an object is a single meal made from that recipe.

House familyhome = new House();
// If a class is a blueprint, then an object is a house made from that blueprint.
```

# Creating and Manipulating an Object
- You can create multiple objects of one class.
- When you create an object, each object will have it’s own set of members and member functions.
	- Members refers to variables that belong to the class.
	- Member functions refers to the methods that belong to the class.
- The object can be manipulated by using the membership operator or dot operator `.`.




- Inside of the main loop is where we can access our attributes and change their values and print them out.
- Only the member functions will have access to the variables created inside private.
- When we declare our variables inside the class -> private, then we do not initialize them.
