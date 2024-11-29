# To uppercase

```CS
String fullname = "Bro Code";

fullname = fullname.ToUpper();
Console.WriteLine(fullname);
```
Output: BRO CODE

# To lowercase
```CS
String fullname = "Bro Code";

fullname = fullname.ToLower();
Console.WriteLine(fullname);
```
Output: bro code

# Replace all
Here we want to convert all of the - that appear in the phone number to /.
```CS
String phoneNumber = "123-456-7890";
phoneNumber = phoneNumber.Replace("-","/");

Console.WriteLine(phoneNumber);
```
Output: 123/456/7890

# Insert method
We can insert a character or a string at a given index within a preexisting string. Note that this does not necessarily have to be a single character, it can be a string as well.
```CS
fullName = "Bro Code";
String userName = fullName.Insert(0, "@");
Console.WriteLine()
```
Output: @Bro Code

# Length of a string
Return the given amount of characters in a string. One potential use of the length property of strings is lets say that someone is creating a username and there is a maximum allowed characters is 12, well we can get the length of whatever they type in and check to see if it is more than 12 characters.
```CS
fullName = "Bro Code";
Console.WriteLine(fullName.Length);
```
Output: 8

# Substring
With the substring method we can take a section or a slice from a string and create an entirely new string from it. 

(0, 3):
0 is the start index and 3 is the amount of characters that you want to include.
```CS
fullName = "Bro Code";
String firstName = fullName.Substring(0, 3);
Console.WriteLine(firstName);
```
Output: Bro

```CS
fullName = "Bro Code";
String lastname = fullName.Substring(4,4);
Console.WriteLine(lastName);
```
Output: Code