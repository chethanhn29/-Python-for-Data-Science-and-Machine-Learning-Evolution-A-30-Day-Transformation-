# Day 2: Variables and Built-in Functions

In this second day, we will dive deeper into the world of variables and built-in functions. We will learn about different types of variables, including integers, floats, and strings, and how to use them in Python. We will also learn about some of the most commonly used built-in functions in Python, such as print() and input().
Introduction to Variables:
A variable is a container that stores a value. Variables are used to store values that can be changed later in the program. In Python, you can use any name as a variable name, but it must start with a letter or an underscore and cannot start with a number. To assign a value to a variable, use the assignment operator (=).

Types of Variables in Python:

#### Integer: A whole number, either positive or negative, without a decimal point. For example, 10, -20, 50, etc.

#### Float: A floating-point number, which has a decimal point. For example, 10.5, 3.14, -2.7, etc.

#### String: A string is a sequence of characters surrounded by quotes. It can be either single quotes (') or double quotes ("). For example, "Hello World!", 'Python is fun!', etc.

Using Variables in Python:
To use a variable in Python, you first need to assign a value to it. For example:


x = 10
y = 20
z = x + y
print(z)
In this example, we have assigned the value 10 to the variable x, the value 20 to the variable y, and then added both values to get the sum and stored it in the variable z. Finally, we used the print() function to display the value of z.

Introduction to Built-in Functions:
A built-in function is a pre-defined function in Python that performs a specific task. Some of the most commonly used built-in functions in Python are:

print(): This function is used to display output on the screen. For example:

print("Hello World!")

input(): This function is used to take input from the user. For example:

name = input("Enter your name: ")
print("Hello, " + name + "!")

In this example, we used the input() function to take input from the user and stored it in the variable name. Then, we used the print() function to display a message along with the value of the name variable.

In conclusion, understanding variables and built-in functions is a crucial step in learning Python programming. These concepts will lay the foundation for more complex programming constructs in the future.




## String Formatting in print() function

There are several methods to format strings in the print function in Python:

#### Concatenation: You can use the + operator to concatenate multiple strings together and print them. For example:

name = "John"

print("Hello, " + name)

####  String Interpolation: You can use the % operator to insert values into a string, also known as string interpolation. For example:
perl

name = "John"

age = 30

print("My name is %s and I am %d years old." % (name, age))

#### f-strings: This is a new way to format strings that was introduced in Python 3.6. f-strings allow you to embed expressions inside string literals, using the {expression} syntax. For example:


name = "John"

age = 30

print(f"My name is {name} and I am {age} years old.")

#### format() method: The format() method is another way to format strings. It allows you to substitute values into a string, using placeholders represented by curly braces {}. For example:

name = "John"

age = 30

print("My name is {} and I am {} years old.".format(name, age))

Each of these methods has its own advantages and disadvantages, and the best method to use depends on your specific needs. However, f-strings are generally considered the most readable and easiest to use, so they are a good starting point.
