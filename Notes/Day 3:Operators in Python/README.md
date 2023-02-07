Day 3:Operators in Python

Introduction:

Operators are symbols in Python that carry out arithmetic or logical computations. They help perform mathematical operations, compare values, test conditions, and assign values to variables. The value that the operator operates on is called the operand. For instance, in the expression 2 + 3 = 5, + is the operator that performs addition and the operands are 2 and 3, with the result being 5.

In this blog, we’ll explore the different types of operators in Python and their usage, including:

Arithmetic Operators
Comparison Operators
Logical Operators
Bitwise Operators
Assignment Operators
Membership Operators
Identity Operators
Let’s dive in and understand each of these operators in detail.

Arithmetic Operators
Arithmetic operators perform mathematical operations such as addition, subtraction, multiplication, and division. Some of the commonly used arithmetic operators in Python are +, -, *, /, %, and **.

For example:

a = 10
b = 20
#Addition
print(a + b) # Output: 30
#Subtraction
print(b - a) # Output: 10
#Multiplication
print(a * b) # Output: 200
#Division
print(b / a) # Output: 2.0
#Modulo
print(b % a) # Output: 0
#Floor Division
print(b // a) # Output: 2
2.Comparison Operators

Comparison operators are used to compare two values and return a Boolean value (True or False) based on the comparison. Some of the commonly used comparison operators in Python are ==, !=, >, <, >=, and <=.

For example:

a = 10
b = 20
#Greater than
print(b > a) # Output: True

#Less than
print(a < b) # Output: True

#Greater than or equal to
print(b >= a) # Output: True

#Less than or equal to
print(a <= b) # Output: True

#Equal to
print(a == b) # Output: False

#Not equal to
print(a != b) # Output: True
3. Logical Operators

Logical operators are used to combine multiple conditions and return a Boolean value based on the evaluation of the conditions. Some of the commonly used logical operators in Python are and, or, and not.

Use: Logical operators are used to make decisions based on multiple conditions. For example, you can use the AND operator to check if two conditions are both True, or the OR operator to check if either of two conditions is True.

For example:

a = True
b = False

# AND
print(a and b) # Output: False

# OR
print(a or b) # Output: True

# NOT
print(not a) # Output: False
In this example, a and b are the operands, and the and operator performs the logical operation, which returns True if both conditions are true in when we are using and operator, and if one of the conditions is false then returns False

In or operator it returns True if either any one or both of the conditions is True, if the both of the conditions is False then it Returns False.

4. Assignment Operators

Assignment operators are used to assign values to variables. Some of the commonly used assignment operators in Python are =, +=, -=, *=, /=, and %=.

a = 10
b = 20

#Basic Assignment
c = a
print(c) # Output: 10

#Addition Assignment
c += a
print(c) # Output: 20

#Subtraction Assignment
c -= a
print(c) # Output: 10

#Multiplication Assignment
c *= a
print(c) # Output: 100

#Division Assignment
c /= a
print(c) # Output: 10.0

#Modulo Assignment
c %= a
print(c) # Output: 0.0
5. Bitwise Operators

Bitwise operators perform bit by bit operations on integers. Some of the commonly used bitwise operators in Python are &, |, ^, ~, and <<.

Use: Bitwise operators are used for low-level operations, such as working with computer hardware, data compression, and cryptography. They are also used in some optimization techniques, such as caching and indexing.

For example:

a = 10 (in binary: 0000 1010)
b = 20 (in binary: 0001 0100)

Bitwise AND
print(a & b) # Output: 0

Bitwise OR
print(a | b) # Output: 30

Bitwise XOR
print(a ^ b) # Output: 30

Bitwise NOT
print(~a) # Output: -11

Bitwise Left Shift
print(a << 2) # Output: 40

Bitwise Right Shift
print(a >> 2) # Output: 2
In this example, a and b are the operands, and the & operator performs the bitwise operation, which returns the binary AND of the two values.

6. Membership Operators: Membership operators are used to test whether a value is found in a sequence (such as a list, tuple, or string).

Use: Membership operators are used to test if a value is a member of a sequence. They are commonly used in control flow statements, such as if statements, to make decisions based on the presence of a value in a sequence.

a) in operator: The in operator is used to test if a value is a member of a sequence. If the value is found, it returns True, otherwise it returns False. Examples:

list = [1, 2, 3, 4, 5]
print(3 in list) # Output: True

string = "Hello World" 
print("Hello" in string) # Output: True

a = [1, 2, 3, 4, 5]
b = 10

# In
print(b in a) # Output: False
b) not in operator: The not in operator is used to test if a value is not a member of a sequence. If the value is not found, it returns True, otherwise it returns False. Examples:

list = [1, 2, 3, 4, 5] 
print(6 not in list) # Output: True

string = "Hello World" 
print("Goodbye" not in string) # Output: True

a = [1, 2, 3, 4, 5]
b = 10
print(b not in a) # Output: True
7.Identity Operators: Identity Operators are used to compare the memory location of two objects in Python. The identity operators are “is” and “is not”.

The identity operator (is) operator returns True if two variables refer to the same object and False otherwise. The negation of the identity operator (is not) operator returns True if two variables do not refer to the same object and False otherwise.

a = [1, 2, 3, 4, 5]
b = [1, 2, 3, 4, 5]

# Is
print(a is b) # Output: False

# Is not
print(a is not b) # Output: True

x = 20
y = 20

Identity operator
print(x is y) # Output: True

Negation of identity operator
print(x is not y) # Output: False

x = 5 y = 3 
print(x is y) # False

x = [1, 2, 3] 
y = [1, 2, 3] 
print(x is y) # False

x = [1, 2, 3] 
y = x 
print(x is y) # True
In the first example, x and y are two different integer objects, so “is” returns False. In the second example, x and y are two different lists, so “is” returns False. In the third example, x and y refer to the same list object, so “is” returns True.

Operator precedence:
Operator precedence is the order in which operations are performed when multiple operations are used in an expression. Python follows the standard mathematical precedence for performing operations, and some operators have higher precedence than others. The following table lists the operator precedence in Python, from highest to lowest:

** (Exponentiation)
~ + — (Complement, Unary plus, and Unary minus)
/ % // (Multiplication, Division, Modulo, and Floor Division)
(Addition and Subtraction)
<< (Right and Left Bitwise Shift)
& (Bitwise AND)
^ | (Bitwise XOR and Bitwise OR)
<= < > >= (Comparison Operators)
== != (Equality Operators)
= %= /= //= -= += *= **= (Assignment Operators)
is, is not (Identity Operators)
in, not in (Membership Operators)
not,or ,and (Logical Operators)
If two or more operators have the same precedence, they are evaluated from left to right.Example:

a = 10
b = 20
c = 30

result = a + b * c
print(result) # Output: 610

result = (a + b) * c
print(result) # Output: 900

result = a + b / c * 2
print(result) # Output: 16.0

result = a + b / (c * 2)
print(result) # Output: 11.0
In the above example, the expression a + b * c is evaluated first, as * has higher precedence than +. In the expression (a + b) * c, the addition is performed within the parentheses first, as parentheses have the highest precedence.

In the expression a + b / c * 2, the division is performed first, as / has higher precedence over +, and then the multiplication is performed. In the expression a + b / (c * 2), the multiplication is performed within the parentheses first, and then the division is performed, followed by the addition.

Practice Questions :

1.Create two variables, a and b, with the following values:
a = 10
b = 20
Calculate the sum of a and b and store the result in a new variable c.
Subtract b from a and store the result in a new variable d.
Multiply a and b and store the result in a new variable e.
Divide b by a and store the result in a new variable f.
Find the remainder of dividing b by a and store the result in a new variable g.
Floor divide b by a and store the result in a new variable h.

2.Create two variables, x and y, with the following values:
x = 10
y = 20
Check if x is less than y.
Check if y is greater than x.
Check if x is equal to y.
Check if y is not equal to x.
Check if x is less than or equal to y.
Check if y is greater than or equal to x.

3.Create two variables, p and q, with the following values:
p = True
q = False
Check if both p and q are True.
Check if either p or q is True.
Check if p is not True.

4.Create two variables, m and n, with the following values:
m = 10
n = 20
Assign the value of m to a new variable o.
Add the value of m to n and store the result in n.
Subtract the value of m from n and store the result in n.
Multiply the value of m and n and store the result in n.
Divide the value of n by m and store the result in n.
Find the remainder of dividing n by m and store the result in n.

Conclusion:
In conclusion, operators play a vital role in Python programming, and understanding the different types of operators and how they work is crucial for writing efficient and effective code. Each operator has a specific purpose and can be used in different scenarios. We can use arithmetic operators for mathematical operations, comparison operators for comparing values, logical operators for combining conditions, bitwise operators for bit by bit operations on integers, assignment operators for assigning values to variables, membership operators for testing the presence of values in sequences, and identity operators for comparing memory locations of objects.
