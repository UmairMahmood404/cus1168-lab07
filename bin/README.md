# Lab: Alternative Arithmetic Operations in Java

### Learning Objectives

* Implement addition operations without using the '+' operator
* Implement division operations without using the '/' operator
* Apply bitwise operators to perform arithmetic calculations
* Understand the relationship between binary representation and arithmetic operations
* Analyze algorithm efficiency for non-standard arithmetic implementations
* Debug and test alternative implementations of common operations

#### Prerequisites

* Basic understanding of Java syntax and data types
* Familiarity with operators in Java
* Knowledge of binary number representation
* Experience with conditional statements and loops

#### Task Description

In this lab, you will implement two fundamental arithmetic operations (addition and division) without using their
conventional operators. This exercise will reinforce your understanding of binary operations and alternative approaches
to solving common programming tasks.

#### Detailed Requirements

1. Implement an `addWithoutPlus` method that:
    * Takes two integers as parameters
    * Returns their sum
    * Does not use the '+' operator anywhere in the implementation

2. Implement a `divideWithoutDivideOperator` method that:
    * Takes two integers (dividend and divisor) as parameters
    * Returns the integer result of their division
    * Does not use the '/' operator anywhere in the implementation
    * Handles edge cases appropriately (e.g., division by zero)

#### Technical Requirements

* Your solution must work for both positive and negative integers
* Your solution must handle potential integer overflow cases
* You may use bitwise operators (e.g., &, |, ^, ~, <<, >>)
* You may use control flow statements (if/else, while, for)
* You may use logical operators (&&, ||, !)
* You may not use other arithmetic operators (+, -, *, /) to accomplish the main task

#### Project Setup

- Open the project in your IDE
- Locate the starter code at: `src/main/java/academy/javapro/lab7/AlternativeArithmetic.java`
- Do not modify the package structure or class name
- Implement the required functionality in the TODOs provided

#### Testing Your Implementation

Test your implementation with the following test cases:

**For addition:**

* `addWithoutPlus(5, 3)` should return `8`
* `addWithoutPlus(-2, 7)` should return `5`
* `addWithoutPlus(0, 0)` should return `0`
* `addWithoutPlus(-5, -3)` should return `-8`
* `addWithoutPlus(100, 200)` should return `300`

**For division:**

* `divideWithoutDivideOperator(10, 2)` should return `5`
* `divideWithoutDivideOperator(15, 3)` should return `5`
* `divideWithoutDivideOperator(8, 4)` should return `2`
* `divideWithoutDivideOperator(7, 2)` should return `3` (integer division)
* `divideWithoutDivideOperator(100, 10)` should return `10`

#### Expected Output

When running your program, it should produce output similar to:

```
Testing addition without '+' operator:
5 + 3 = 8 (Correct)
-2 + 7 = 5 (Correct)
0 + 0 = 0 (Correct)
-5 + -3 = -8 (Correct)
100 + 200 = 300 (Correct)
2147483647 + 1 = -2147483648 (Correct)
-100 + 100 = 0 (Correct)

Testing division without '/' operator:
10 / 2 = 5 (Correct)
15 / 3 = 5 (Correct)
8 / 4 = 2 (Correct)
7 / 2 = 3 (Correct)
100 / 10 = 10 (Correct)
-15 / 3 = -5 (Correct)
15 / -3 = -5 (Correct)
0 / 5 = 0 (Correct)
1024 / 2 = 512 (Correct)

Testing subtraction without '-' operator:
10 - 3 = 7 (Correct)
5 - 8 = -3 (Correct)
0 - 0 = 0 (Correct)
-5 - -3 = -2 (Correct)
100 - 50 = 50 (Correct)

Process finished with exit code 0
```
