- We use the increment operator in loops: `number++;//number=number+1` to increase the value of a variable by one.
- The increment operator can also be used in numerical expressions:
``` CPP
int number = 2;
int valueProduced = 2* (number++);
```
- `(number++)` first returns the value of number (2) to be multiplied by 2, then increments number to three.

# Post Increment versus Pre Increment
- `(number++)` returns the current value of number, then increments number.
	- An expression using `(number++)` will use the value of number BEFORE it is incremented.
- `(++number)` increments number first and returns the new value of number AFTER it is incremented.
- Number has the same value after either version, but the result of the expression may be different!


``` CPP file:Comparisions
#include <iostream>
using namespace std;

int main() 
{
	int n=0, x, y;
	x=(++n);
	y=(x++);
	cout << "x=" << x << " y=" << y << " n=" << n << endl;
}
```
![[Pasted image 20231106202535.png]]