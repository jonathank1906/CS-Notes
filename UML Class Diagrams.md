# What is UML?
UML (Unified Modeling Language)
- It is not a programming language, but instead it is a graphical used to represent object-oriented systems.
- UML can be used to describe and define different types of diagrams. 
	- A class diagram is a graphical representation of the classes in our system and the relationships they have.
- The purpose of using these class diagrams is that we can get a visual representation of the structure/design before we get into coding (implementation).

## Encapsulation
- Encapsulation controls what is accessible and modifiable in a class, keeping certain parts private to ensure that users can interact with the class safely and as intended, without causing vital data to be exposed, manipulated, or lost. 

# Class Diagrams Parts
## Main Sections
Each class diagram has three sections:
1. The <u>name</u> of the class is in the top section. This name represents a category or type of object, like how Ball might represent all kinds of balls in general. The class name is typically written in **bold** to make it easily distinguishable. 
2. The middle section lists the <u>attributes</u> of the class. These attributes describe the properties or characteristics of the class.
3. The bottom section lists the <u>operations</u> of the class. Operations, also called behaviors, describe the actions that the class can perform. 
# Details
## Accessibility/Visibility
- These symbols help us understand which parts of a class are accessible to other parts of the system or even other systems, and which parts are protected. 
- Written to the left of the name of the attributes and behaviors, the accessibility can be either public(+) or private(-). 


## Name
- For only the methods at the bottom section, include ()
## Data Type
After the colon is:
- For the attributes section is the data type (int, string, etc.).
- For the methods section is the return type (bool, void, etc.).

## Stereotype
Examples of valid stereotypes:
- `<<static>>`
- `<<enumeration>>`
- `<<record>>`

## Get and Set


## Association
The different relationships between classes are shown by different types of arrows.
### Arrow
- A solid filled arrow represents a <u>unidirectional association</u> relationship. The base of the arrow is the .....and the tip (what it is pointing at) is the 

### Line
- A line connecting two (UML classes) represents a <u>bidirectional association</u> relationship.

## Composition
### Diamond
- A solid filled diamond represents a <u>composition</u> relationship.


## Aggregation
### Diamond
- A hollow diamond represents an <u>aggregation</u> relationship.

## Inheritance
### Hollow Arrow

- A hollow line with an arrow represents an <u>inheritance</u> relationship.
















