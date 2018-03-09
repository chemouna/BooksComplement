
# Hacker's Delight 

## Learned
- An unsigned integer is a power of two if and only if it has exactly one 1 bit. 
- 2^n = 1 << n
- 2^n is the number of ways the bits in a binary word of length n can be arranged 
- binary representation of integers makes it possible to apply a very fast test to determine whether a given positive integer x is a power of two:
  positive x is a power of two <=> (x & (x − 1)) is equal to zero. 
- the binary representation of integers makes it possible to calculate the modulos of a non-negative integer (x) with a power of two (y) very quickly:
   x mod y = (x & (y − 1)). 
- division by two can be performed by a bit shift operation that shifts the number one place to the right. 
  For example, 1101001 in binary (the decimal number 105), shifted one place to the right, is 110100 (the decimal number 52): the lowest order bit, a 1, 
  is removed. Similarly, division by any power of two 2k may be performed by right-shifting k positions. 
- checking whether a binary integer is odd is the same as checking if its least significant bit is 1.
- x is power of 2 if ((x != 0) && ((x & (~x + 1)) == x)), (x & (~x + 1)) == x, is true only when x is a power of two. 
  It compares x with its two’s complement. The two’s complement of x is computed with ~x + 1, which inverts the bits of x and adds 1 
 
 
## Links 
- [Power of two](https://en.wikipedia.org/wiki/Power_of_two)
- [Division by two](https://en.wikipedia.org/wiki/Division_by_two)
- [Ten Ways to Check if an Integer Is a Power Of Two in C](http://www.exploringbinary.com/ten-ways-to-check-if-an-integer-is-a-power-of-two-in-c/)
