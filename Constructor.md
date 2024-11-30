# Constructors

- Constructor is the method that constructs your class.
- It has the name of the class and no data type. The constructor can allow arguments (they go inside the () ).
- Constructors allow you to specify the initial values
- Every class will have a constructor, even if you don’t specify one. Your IDE will automatically generate a default empty constructor in this situation.

- Inside the constructor, we have to assign our properties. Notice how they share the same naming including the case. When we assign they have to be different.

```csharp
class Human
{
	// Properties should start with a capital letter 
	// These are normally called fields
	public int Height;
	public int Weight;
		
	// The arguments of the constructor should start with a lowercase letter
	public Human(int height, int weight)
	{
		Height = height; // Capital variable on the left and lowercase variable on the right
		Weight = weight;
	}
}
```

So it follows a 4 step procedure in which the value travels:

![image.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/b46a692d-4430-463b-be4f-b9cff6f46679/453d9167-cdf2-4c2c-8d15-ba8e41d8d5aa/image.png)

- There are 2 approaches in defining the values:
    - We can define them outside of the class (nothing will be in the arguments of the constructor)
    - We can define them in the constructor (we use arguments).

- We are allowed to create multiple constructors for one class. We can for example create an empty constructor that takes no arguments and another one that takes two arguments.