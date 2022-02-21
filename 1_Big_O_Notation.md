# Big O Notation

Motiviation
* It's important to have a precise vocabulary to talk about how our code performs
* Useful for discussing trade-offs between different approaches
* Identifying parts of the code that are inefficient can help find pain points

Rather than counting seconds, which are so variable. Let's count the number of simple operations the computer has to perform.

## Definition
Big O is:
* A way to formalize fuzzy counting
* It allows us to talk formally about how the runtime of an algorithm grows as the inputs grow
* We won't care about the details, only the trends

### Time complexity
An algorithm is O(f(n)) if the number of simple operations the computer has to do is eventually less than a constant times f(n), as in increases.

## Simplifying Big O Expressions
**Constants don't matter**
* O(2n) -> O(n)
* O(500) -> O(1)
* O(13n^2) -> O(n^2)

**Smaller terms don't matter**
* O(n+10) -> O(n)
* O(1000n + 50) -> O(n)
* O(n^2 + 5n + 8) -> O(n^2)

**Shorthands**
1. Arithmetic operations are constant
1. Variable assignment is constant
1. Accessing element in an array by index or object by key is constant
1. In a loop, the complexity is the length of the loop times the complexity of whatever happens inside the loop

### Space complexity
* Most primitives (booleans, numbers, undefined, null) are constant space
* Strings require O(n) space (where n is the string length)
* Reference types are generally O(n), where n is the length for array or the number of keys for objects

### Notes on logarithms
What's a log? - The inverse of a exponentiation (how many times a numbe can be divided by 2 until it reaches 1)
Logarithmic time complexity is great!
