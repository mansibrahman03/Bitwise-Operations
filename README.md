CS Data Lab

Overview: This repository contains solutions to the Data Lab, a programming assignment from the CS (Computer Systems: A Programmer's Perspective) course. The Data Lab focuses on bit manipulation and understanding of the binary representation of data in C programming.

Purpose
The Data Lab is designed to develop a deep understanding of bit-level operations and data representations by implementing various functions using only a limited set of C operators. This helps students gain insights into how computers represent and manipulate data at the most fundamental level.

Structure
The main file is bits.c, which contains implementations for the following functions:
1. bitXor: Compute x^y using only ~ and &
2. isNotEqual: Check if two integers are not equal
3. getByte: Extract a specific byte from a word
4. copyLSB: Set all bits of result to the least significant bit of x
5. logicalShift: Perform a logical right shift
6. bitCount: Count the number of 1's in a word
7. bang: Compute logical negation without using !
8. leastBitPos: Return a mask marking the position of the least significant 1 bit
9. tmax: Return the maximum two's complement integer
10. isNonNegative: Check if an integer is non-negative
11. isGreater: Check if x is greater than y
12. divpwr2: Compute x/(2^n) with rounding toward zero
13. absVal: Compute the absolute value of an integer
14. addOK: Determine if addition can be performed without overflow

Coding Rules
1. Only the following operators are allowed:
- Bitwise operators: ~, &, ^, |
- Integer constants (0-255)
- Arithmetic operators: +, <<, >>
- Logical operators: ! (in most functions)
2. The following are expressly forbidden:
- Control constructs (if, while, for, etc.)
- Macros and additional functions
- Function calls
- Logical operators && and ||
- The subtraction operator -
- The conditional operator ?:
- Casting
- Data types other than int
3. Each function has a maximum number of operators that can be used.

Assumptions
- The machine uses 2's complement, 32-bit representations of integers
- Right shifts are performed arithmetically
- Shifting an integer by more than the word size has unpredictable behavior

Testing
The lab provides two main tools for testing:
- dlc (data lab checker): Verifies that solutions conform to the coding rules
- btest: Tests the correctness of the implemented functions

Author
Mansib Rahman

License
This code includes elements from the GNU C Library, which is covered by the GNU Lesser General Public License.