- Constants declared on the top of a program allows us to use them in the whole program.
``` CPP
#define PI 3.1415
```
- The latest versions of C/C++ allow us to declare a constant using keyword `const`.
``` CPP
const float a;
```
These two ways of definining a constant in C/C++ will do the same thing. However, the obvious difference between the two ways is the syntax. The less obvious difference is that `const` will consume memory while `#define` does not.

