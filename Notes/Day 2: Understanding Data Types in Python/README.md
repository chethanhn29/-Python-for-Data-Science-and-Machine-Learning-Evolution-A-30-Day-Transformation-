Day 2: Understanding Data Types in Python

Introduction of data types in Python:
In the previous article, we covered the basics of Python and some of the fundamental concepts involved in programming with this language.

Data types define the type of value a variable can hold, and this determines the kind of operations that can be performed on it. They are used to ensure that the data stored in a variable is of the correct type and format, which helps in avoiding errors in the code.

There are several built-in data types in Python, such as integers, floats, strings and Booleans.

In this article, we will focus on these Basic data types and discuss the rest in detail in the upcoming days.

Data Types:
Python has the following data types built-in by default, in these categories:

1.Text Type: str

2.Numeric Types: int,float,complex

3.Sequence Types: list,tuple,range

4.Mapping Type: dict

5.Set Types: set,frozenset

6.Boolean Type: bool

Examples of Data Types and Their Real-World Use:

Integer: Used to represent whole numbers, e.g. number of items in a cart.
Float: Used to represent decimal values, e.g. price of an item.
String: Used to represent characters or text, e.g. name of a product.
Boolean: Used to represent binary values, i.e., true or false, e.g. availability of a product.
1.Integers(int):

Integers are whole numbers and can be positive or negative, such as 3, -5, or 100. They are represented by the int data type in Python ,integers can be created by assigning a whole number value to a variable. For example: x = 5

They can be used for mathematical operations such as addition, subtraction, multiplication, and division. For example:

x = 10,y = 5
print(x + y) # Output: 15
print(x - y) # Output: 5
print(x * y) # Output: 50
print(x / y) # Output: 2
Integers have several methods available, such as abs(), divmod(), pow() and round().

abs(): Returns the absolute value of an integer. For example, abs(-3) would return 3.

divmod(): Returns a tuple of the quotient and remainder of a division operation. For example, divmod(5, 2) would return (2, 1).

pow(): Returns the result of raising an integer to a power. For example, pow(2, 3) would return 8.

round(): Returns the rounded value of a float, with the option to specify the number of decimal places. For example, round(3.14, 1) would return 3.1

2. Float(float):

Floats are numbers with decimal points and it can also be positive or negative, such as 3.14, -5.0, or 100.5. but they are used for more precise calculations, such as those involving decimal points, floats type Numbers can be created by assigning a decimal number value to a variable. For example:

x = 3.14

They are represented by the float data type in Python. Some common operations that can be performed on floating-point numbers include addition, subtraction, multiplication, and division. For example:

x = 10.5
y = 5.5
print(x + y) # Output: 16.0
print(x - y) # Output: 5.0
print(x * y) # Output: 57.75
print(x / y) # Output: 1.909090909090909
Floats have several methods available, such as

abs(): Returns the absolute value of a float. For example, abs(-3.14) would return 3.14.

divmod(): Returns a tuple of the quotient and remainder of a division operation. For example, divmod(5.5, 2) would return (2.0, 1.5).

pow(): Returns the result of raising a float to a power. For example, pow(2.5, 3) would return 15.625.

round(): Returns the rounded value of a float, with the option to specify the number of decimal places. For example, round(3.14, 1) would return 3.1.

3.Booleans:

Booleans are a data type that can only take on one of two values: True or False. They are represented by the bool data type in Python. Booleans can be used to make logical comparisons and it is often used in control flow statements, such as if-else statements, to determine the flow of a program. For example:

x = True
y = False
print(x and y) # Output: False
print(x or y) # Output: True
Bool data type also have several methods available some of them are listed below

bool(): Returns the Boolean value of the object. For example, bool(0) would return False, and bool(1) would return True.

int(): Returns the integer representation of a Boolean value. For example, int(True) would return 1, and int(False) would return 0.

str(): Returns the string representation of a Boolean value. For example, str(True) would return “True”, and str(False) would return “False”.

4.Strings:

A string is a sequence of characters, such as “hello”, “world” or “123 ” and Strings are used for text manipulation,it can be represented by the str data type in Python.

Strings can be created by enclosing characters in either single quotes or double quotes For example:

x = “hello”

Some common operations that can be performed on strings include concatenation, slicing, and indexing. For example:

String Concatenation:

String concatenation is the process of combining two or more strings into a single string. In Python, you can concatenate strings using the + operator.

Examples:

# Concatenating two strings
s1 = "Hello"
s2 = "World"
s3 = s1 + " " + s2
print(s3)  # Output: Hello World

# Concatenating multiple strings
s4 = " ".join(["Hello", "Beautiful", "World"])
print(s4)  # Output: Hello Beautiful World

# Concatenating string and integer
num = 123
s5 = s1 + " " + str(num)
print(s5)  # Output: Hello 123
String Indexing:


Example of String Indexing
String indexing is the process of accessing individual characters in a string by specifying their position or index. In Python, you can access a specific character in a string using square brackets ( [ ]). The index of the first character is 0, and the index of the last character is ( -1 ).

Examples:

makefileCopy code# Accessing the first character
s = "Hello World"
c1 = s[0]
print(c1)  # Output: H

# Accessing the last character
c2 = s[-1]
print(c2)  # Output: d

# Accessing a specific character
c3 = s[5]
print(c3)  # Output: W
String Slicing:

String slicing is the process of extracting a part of a string by specifying the start and end index. In Python, you can slice a string using square brackets ( [ ]) and the colon ( : ) operator.


Examples:

# Slicing the first 3 characters
s = "Hello World"
s1 = s[:3]
print(s1)  # Output: Hel

# Slicing the last 5 characters
s2 = s[-5:]
print(s2)  # Output: World

# Slicing a specific range of characters
s3 = s[2:5]
print(s3)  # Output: llo
Strings have several methods available some of them are listed belowStrings have several methods available, such as capitalize(), upper(), replace() and find().

upper(): Returns the string in all upper case. For example, “hello”.upper() would return “HELLO”.

lower(): Returns the string in all lower case. For example, “HELLO”.lower() would return “hello”.

capitalize(): Returns the string with the first character capitalized and the rest of the characters in lower case. For example, “hello world”.capitalize() would return “Hello world”.

split(): Returns a list of substrings in the string, split by a specified delimiter. For example, “hello world”.split(“ “) would return [“hello”, “world”]

len() : Returns the length of a string

count(): returns the number of occurrences of a substring in the string

endswith(): returns True if the string ends with the specified suffix.

Type Checking:

In some cases, it may be necessary to check the data type of a value or variable. This can be done using the built-in function type().In Python, you can use the built-in function type() to check the data type of a variable.

In this example, we assigned the value 42 to the variable x, and then used the type() function to check its data type. The output shows that x is of type int.

# Assign a value to a variable
x = 42

# Check the data type of the variable
print(type(x))

# Output:
# <class 'int'>
In this example, we assigned the values 3.14 and “Hello, world!” to the variables y and z, respectively, and then used the type() function to check their data types. The outputs show that y is of type float and z is of type str.

y = 3.14
print(type(y))
# Output: <class 'float'>

z = "Hello, world!"
print(type(z))
# Output: <class 'str'>
Operators :

Depending on the data type, different operators can be used to perform operations on values or variables. For example, the + operator can be used to concatenate strings, while the * operator can be used to repeat strings. For int and float data types, mathematical operators like +, -, *, / and % are used.

The * operator is used to multiply two numbers:
a = 3
b = 4
c = a * b
print(c)
Output: 12
For example, the + operator is used to add two numbers:
a = 3
b = 4
c = a + b
print(c)
Output: 7
# For strings, * operator is used to repeat a string:
a = "Hello"
c = a * 3
print(c)
Output: HelloHelloHello
# For strings, the + operator is used to concatenate two strings:
a = "Hello"
b = "World"
c = a + b
print(c)
Output: HelloWorld
It’s important to note that the operators used for different data types can have different results, so it’s important to understand the behavior of each operator for different data types.

Practice Questions on Data types of Python :
Try to Solve on your own , and if you can’t sovle ,then you can find solution for the below questions Here

x = 25 ,y = 15 ,z = “Hello”

a = “World” , b = -15.8 , c = 20.5 , d = True , e = False

Perform integer mathematical operations:
Add x and y and print the result.
Subtract y from x and print the result.
Multiply x and y and print the result.
Divide x by y and print the result.
2.String methods:

Find the length of the string z.
Concatenate z and a and print the result.
Slice the first three characters of z and print the result.
Find the index of the character ‘l’ in z.
3.Boolean operations:

Print the result of x > y.
Print the result of x < y.
Print the result of d and e.
Print the result of d or e.
4.Float operations:

Add b and c and print the result.
Subtract c from b and print the result.
Multiply b and c and print the result.
Divide b by c and print the result.
Check the type of b and c.
Conclusion:
In this post, we have covered the different data types available in Python, including integers, floats, strings, and booleans. We also discussed string indexing,Slicing,Concatenation and how to check the type of variable.

By mastering these concepts, you can write efficient and accurate code. Practice and experimentation are key to becoming proficient in these areas. Keep learning and keep coding!”

Python
Datatypes In Python
Python For Data Science
Towards Data Science
Python For Beginners
1





1



More from Chethan H N
Data Science Enthusiast
