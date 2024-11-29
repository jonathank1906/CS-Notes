# Generate random whole number
This will generate so called “pseudorandom” numbers so they are not truly random, but pretty close.

```CS
Random random = new Random();

int num = random.Next(1,7);

Console.WriteLine(num);
```

Line 3: `Next` will generate a random number within the specified range. 1 is the lower range (inclusive) and 7 is the upper range (exclusive). We could get any number between 1 and 6, similar to a dice.

# Generate random decimal number
This code snippet will generate a random decimal (double) between 0 and 1.
```CS
Random random = new Random();

int num = random.NextDouble();

Console.WriteLine(num);
```