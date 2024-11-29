/images
Binær has the base number 2.                         
Octalce has the base number 8.
Hexadecimal has the basebumer 16.
Decimal system has the basenumber 10.




# Bits
- The least significant bit (LSB) the the rightmost bit.
- The most significant bit (MSB) the the leftmost bit. Also called the sign bit.

- If the LSB is 0, the binary number is even.
- If the LSB is 1, the binary number is odd.



## Bit Patterns
### Text
ASCII
ISO
Unicode

### Numbers
We use binary notation instead of doing encoded symbols (as in text) because it uses less storage (bits).


#### Integers
Two’s compliment

#### Fractions
Floating-point notation


### Images


### Sound


# Binary Number System
- We are all familiar with the "base 10" system. This includes the numbers: 0, 1, 2, 3, 4, 5, 6, 7, 8, and 9. We are able to create any number we want using a combination of these 10 numbers.
- Computers however only understand what is called "base 2", where there is only 2 numbers: 0 and 1. We can still create any number we want using different combinations of 0 and 1.
## Binary Operations

### Binary Addition

### Binary Subtraction

## Fractions in Binary


## Two’s Compliment
- Allows us to represent negative numbers.
- It is easy to perform operations on these numbers like addition and subtraction.
- The MSB if it is 1 then it is negative if it is 0 it is positive.
- Since the MSB represents the sign , we then only have 7 bits available for representing the number which corresponds to 127 different values. 
#### Three Bit Patterns
#### Four Bit Patterns


## Excess Notation
- Offset

# Octal Number System

# Hexadecimal Number System
- Base 16
- Note that the order does not matter it can be a letter first or it could be a number first. Examples:
	- B7
	- 2EA

# Decimal Number System


# Conversion between Number Systems
## Binary to Decimal
1. Make space in between each binary number.
2. Starting from the right add $2^0$,$2^1$,$2^2$,... and so on above each binary number.
3. Evaluate the exponent for the non-zero terms.
4. Sum up the numbers to get the final answer.

Converting 1101 to 13
![[Number Systems-20240904231902766.webp|287]]

Converting 11001 to 25
![[Number Systems-20240904231941048.webp|329]]



- Every time you proceed to the next $2^n$ term, the number doubles.
- It is handy to have a table of .... available to quickly find what exponent values you need.
![[Number Systems-20240904221804079.webp|354]]
## Decimal to Binary
We have two methods for converting from decimal to binary:
1. Using subtraction
2. Using division


### Subtraction Method
1. Begin by writing base 2 terms from right to left. Write down enough terms up to 128 should be enough. So write 128, 64, 32, 16, 8, 4, 2, 1.
2. Find the largest number that is smaller than the actual number. In other words, pick the term that is one less than ............ If we call our number x, then we need to find the largest number that is smaller than x.
3. Take the decimal number and subtract it by this term. Keep track of which terms you use.



In this example we convert 63 to 111111
![[Number Systems-20240904224209130.webp|598]]

In this example we convert 18 to 10010
![[Number Systems-20240904225558363.webp|467]]

### Successive Division Method


Converting 63 to 111111
![[Number Systems-20240904231650837.webp|506]]

Converting 35 to 100011
![[Number Systems-20240904231742122.webp|413]]


## Hexadecimal to Decimal

## Decimal to Hexadecimal 

## Binary to Hexadecimal
[How To Convert Binary to Hexadecimal - Computer Science - YouTube](https://www.youtube.com/watch?v=tSLKOKGQq0Y)
- This methods works for binary numbers of length 8,10,

1. Start by separating the binary numbers into groups of 4.
	 - If there are left over binary numbers, then create a group with additional zeros in front until there are 4 numbers in total for this group.
2. Now convert these individual binary number groups into their equivalent decimal value.
3. Now convert the left most decimal value to hexadecimal value, (10-15). Replace this decimal number which should be in the range of 10-15 to this hexadecimal value.
### Example
1011101010 - 2EA

10110111 - B7




# Overflow
- With any system we can face an issue when you try to store values that don’t fit.