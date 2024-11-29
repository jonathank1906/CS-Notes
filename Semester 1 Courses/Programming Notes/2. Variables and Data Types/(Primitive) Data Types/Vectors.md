# What is a vector?
- A vector is a data structure that allows you to store multiple values of a data type. A vector is similar to an array except that a vector can grow in size at anytime during the program execution.


```CPP file:Vectors
#include <iostream>
#include <vector>
using namespace std;

int main()
{
	vector <int> myVector;
	myVector.push_back(10); // Push in the number 10 into myVector. It stores this value in the next avaliable slot in the vector.
	// The value is pushed to the last or back slot.
	cout << myVector[0] << endl;
	myVector.push_back(5);
	cout << myVector[1] << endl;


	//Initilize #2
	vector <int> anotherVector(5); // Reserve 5 slots
	cout << anotherVector[0] << endl;

	//Initilize #3
	vector <int> aThirdvector(5, 3); // 3 is default and 5 slots is saved
	for (int i = 0; i < aThirdvector.size(); i++)
	{
		cout << aThirdvector[i] << endl;
	}
	cout << aThirdvector[0] << endl;
	int number;
	for (int i = 0; i < 5; i++)
	{
		cout << "Enter a number: ";
		cin >> number;
		myVector.push_back(number);
	}

	cout << endl;
	for (int i = 0; i < myVector.size(); i++) // sizeof(myArray) / 4 (for arrays). 4 bites per integer
	// Do not use sizeof funtion on vectors.
	{
		cout << "Index: " << i << ": " << myVector[i] << endl;
	}

	// Remove elements from vector(pop back)
	myVector.pop_back();
	myVector.pop_back();
	myVector[0] = 35;
	cout << endl;
	for (int i = 0; i < myVector.size(); i++) 										 
	{
		cout << "Index: " << i << ": " << myVector[i] << endl;
	}
	//-----------------------------------------------------------------------------
	int temp = 0;
	temp = myVector.size();
	cout << temp << " Elements" << endl;
	system("pause");
	return 0;

}
```