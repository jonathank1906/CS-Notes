# Where are access-specifiers used?
Can both classes and objects have access specifiers? 
- Classes can have access-specifiers, objects do not. Objects are instances of a class and access the members of the class according to the access rules defined by the class.


- Objects do not have a defined access specifier, they obtain it from the class itself. 
- Attributes and operations have their own access specifiers.

# public
- When we set the access specifier to public, then we are able to <u>access</u> and <u>modify</u> our attributes or methods.
	- 
# private
- When we set the access specifier to private, then we are not able to access our attributes .
	- This also means that we are not able to access this class in any other class or subclass.








- Inside public is where we create all of our member functions (function prototypes).


- Outside of the class (underneath it) should go the actual functions.

# protected


Other
# abstract class

# static
- When we mark a class as static, we intend for only ONE of these to exist. 
- If we consider a class called `RecipeManager` or it could be anything ending with the word Manager, it needs to be set as static because you should only have one of those. 



