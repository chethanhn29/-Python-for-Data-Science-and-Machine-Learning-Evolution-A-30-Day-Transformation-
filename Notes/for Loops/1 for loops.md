# `for loop`
for loop in Python is a control structure used for iterating over a sequence (such as a list, tuple, dictionary, set, or string) and executing a block of code for each item in the sequence.

#### Break and Continue: 
The break and continue statements can be used to control the flow of a loop. The break statement will exit the loop while the continue statement will skip the current iteration and move on to the next one.

#### Loop Control Variables:
A loop control variable is used to control the number of iterations in a loop. This variable is typically incremented or decremented after each iteration.


##### The general syntax of a for loop in Python is as follows:

`for element in sequence:`
    
    # code to be executed for each element in the sequence
    
Here, element is a variable that takes on the value of each item in the sequence, one at a time, and the sequence can be any iterable object in Python, such as a list, tuple, dictionary, set, or string. The # code to be executed block is executed once for each item in the sequence.
Example:


```python
print("List Iteration")
l = ["geeks", "for", "geeks"]
for i in l:
    print(i)
 
# Iterating over a tuple (immutable)
print("\nTuple Iteration")
t = ("geeks", "for", "geeks")
for i in t:
    print(i)
 
# Iterating over a String
print("\nString Iteration")
s = "Geeks"
for i in s:
    print(i)
 
# Iterating over dictionary
print("\nDictionary Iteration")
d = dict()
d['xyz'] = 123
d['abc'] = 345
for i in d:
    print("%s  %d" % (i, d[i]))
 
# Iterating over a set
print("\nSet Iteration")
set1 = {1, 2, 3, 4, 5, 6}
for i in set1:
    print(i),
```

    List Iteration
    geeks
    for
    geeks
    
    Tuple Iteration
    geeks
    for
    geeks
    
    String Iteration
    G
    e
    e
    k
    s
    
    Dictionary Iteration
    xyz  123
    abc  345
    
    Set Iteration
    1
    2
    3
    4
    5
    6
    


```python
# Using `reversed()` function in for loops
#The `reversed()` function in Python can be used to iterate over elements in a sequence in reverse order.
numbers = [1, 2, 3, 4, 5]
for number in reversed(numbers):
    print(number)


```

    5
    4
    3
    2
    1
    

### `range(start, stop, step)`
where start is the first number in the range (inclusive), stop is the last number in the range (exclusive), and step is the difference between each number in the range.

We can use the range() function to generate a sequence of numbers, and then use a for loop to iterate over that sequence. 

The range() function takes in one, two, or three arguments: start, stop, and step. start is the first number in the sequence (default is 0), stop is the last number in the sequence (this number is not included in the sequence or (n-1)), and step is the difference between each number in the sequence (default is 1).



```python
#Example 1 :
for i in range(5):
    print(i)
    
#Example 2 :    
print("\t") ## To print the output in New line 
for number in range(2, 5):
    print(number)

#Example 3 :
print("\t") ## To print the output in New line 
for number in range(0, 10, 2):
    print(number)
```

    0
    1
    2
    3
    4
    	
    2
    3
    4
    	
    0
    2
    4
    6
    8
    

### `enumerate()`
We can also use the enumerate() function in a for loop to iterate over the items in a sequence and keep track of the index of each item.
The enumerate() function is a built-in function in Python that takes an iterable object as an argument and returns an iterator that produces pairs of index and value.




```python
  #Example1:
fruits = ['apple', 'banana', 'cherry']
for i, fruit in enumerate(fruits):
    print(i, fruit)
    
#Example2:
print("\t")

numbers = [1, 2, 3, 4, 5]
for i, number in enumerate(numbers):
    print(i, number)

#Example3: 
print("\t") ## To print the output in New line 

numbers = [1, 2, 3, 4, 5]
for i, number in enumerate(numbers, start=10):
    print(i, number)
```

    0 apple
    1 banana
    2 cherry
    	
    0 1
    1 2
    2 3
    3 4
    4 5
    	
    10 1
    11 2
    12 3
    13 4
    14 5
    

###   `zip()`
The zip() function is a built-in function in Python that takes multiple iterables as arguments and returns a single iterator that aggregates elements from each of the iterables.
or We can use the zip() function in a for loop to iterate over two or more sequences in parallel and pair the corresponding items from each sequence.


```python
#Example:
fruits = ['apple', 'banana', 'cherry']
colors = ['red', 'yellow', 'red']
for fruit, color in zip(fruits, colors):
    print(fruit, color)
```

    apple red
    banana yellow
    cherry red
    

## `Nested for loops`
Nested loops are when you have one or more loops inside another loop. This allows you to iterate over multiple lists at the same time.


```python
fruits = ['apple', 'banana', 'cherry']
colors = ['red', 'yellow', 'red']
for fruit in fruits:
    for color in colors:
        print(fruit, color)

# Nested loop that prints multiplication table
print("\t") ## To print the output in New line
for i in range(1, 6):
    for j in range(1, 6):
        print(i * j, end='\t')
    print()
    
    
print("\t") ## To print the output in New line    
fruits = ['apple', 'banana', 'cherry']
colors = ['red', 'yellow', 'red']
for i, fruit in enumerate(fruits):
    color = colors[i]
    print(fruit, 'is', color)
```

    apple red
    apple yellow
    apple red
    banana red
    banana yellow
    banana red
    cherry red
    cherry yellow
    cherry red
    	
    1	2	3	4	5	
    2	4	6	8	10	
    3	6	9	12	15	
    4	8	12	16	20	
    5	10	15	20	25	
    	
    apple is red
    banana is yellow
    cherry is red
    

##### `In this example, the outer for loop iterates over the fruits list using the enumerate function, as in the previous example. The inner for loop then iterates over the colors list, using the index of the current item in the fruits list to access the corresponding color. The indented block of code then prints both the fruit and its color.`



```python
#Example 1:
fruits = ['apple', 'banana', 'cherry']
numbers = [1, 2, 3]
for fruit in fruits:
    for number in numbers:
        print(fruit, number)
        
#Example 2:
print("\t") ## To print the output in New line
words = ['hello', 'world']
characters = ['a', 'b', 'c']
for word in words:
    for character in characters:
        print(word, character)
        
#Example 3:
print("\t") ## To print the output in New line
fruits = ['apple', 'banana', 'cherry']
numbers = [1, 2, 3]
for i, fruit in enumerate(fruits):
    for j, number in enumerate(numbers):
        print(i, fruit, j, number)
```

    apple 1
    apple 2
    apple 3
    banana 1
    banana 2
    banana 3
    cherry 1
    cherry 2
    cherry 3
    	
    hello a
    hello b
    hello c
    world a
    world b
    world c
    	
    0 apple 0 1
    0 apple 1 2
    0 apple 2 3
    1 banana 0 1
    1 banana 1 2
    1 banana 2 3
    2 cherry 0 1
    2 cherry 1 2
    2 cherry 2 3
    


```python
#Example 4:
print("\t") ## To print the output in New line
words = ['hello', 'world']
characters = ['a', 'b', 'c']
for i, word in enumerate(words):
    for j, character in enumerate(characters):
        print(i, word, j, character)

#Example 5:
print("\t") ## To print the output in New line
fruits = ['apple', 'banana', 'cherry']
numbers = [1, 2, 3, 4, 5]
for fruit in fruits:
    for number in numbers:
        if number % 2 == 0:
            print(fruit, number)
```

    	
    0 hello 0 a
    0 hello 1 b
    0 hello 2 c
    1 world 0 a
    1 world 1 b
    1 world 2 c
    	
    apple 2
    apple 4
    banana 2
    banana 4
    cherry 2
    cherry 4
    


```python
#Example 6:
print("\t") ## To print the output in New line
words = ['hello', 'world']
characters = ['a', 'b', 'c', 'd']
for word in words:
    for character in characters:
        if character in ['a', 'c']:
            print(word, character)
#Example 7:
print("\t") ## To print the output in New line
fruits = ['apple', 'banana', 'cherry']
numbers = [1, 2, 3, 4, 5]
for i, fruit in enumerate(fruits):
    for j, number in enumerate(numbers):
        if number % 2 == 0:
            print(i, fruit, j, number)
            
#Example 8:
print("\t") ## To print the output in New line
words = ['hello', 'world']
characters = ['a', 'b', 'c', 'd']
for i, word in enumerate(words):
    for j, character in enumerate(characters):
        if character in ['a', 'c']:
            print(i, word, j, character)
```

    	
    hello a
    hello c
    world a
    world c
    	
    0 apple 1 2
    0 apple 3 4
    1 banana 1 2
    1 banana 3 4
    2 cherry 1 2
    2 cherry 3 4
    	
    0 hello 0 a
    0 hello 2 c
    1 world 0 a
    1 world 2 c
    


```python
#Example 9:
print("\t") ## To print the output in New line
fruits = ['apple', 'banana', 'cherry']
numbers = [1, 2, 3, 4, 5]
for fruit in fruits:
    for number in numbers:
        if number % 2 == 0:
            print(fruit, number)
            break
#Example 10:
print("\t") ## To print the output in New line
words = ['hello', 'world']
characters = ['a', 'b', 'c', 'd']
for word in words:
    for character in characters:
        if character in ['a', 'c']:
            print(word, character)
            break
```

    	
    apple 2
    banana 2
    cherry 2
    	
    hello a
    world a
    

##### if we can observe Clearly the inner loop will iterate all the elements  for every outer loop iteration of each element.

## `else clause in for loop`
 The else clause in a for loop is executed when the loop has completed its iteration and there was no break statement encountered.


```python
#Example 1:
fruits = ['apple', 'banana', 'cherry']
for fruit in fruits:
    if fruit == 'banana':
        break
    print(fruit)
else:
    print('No bananas found!')
    
#Example 2:
numbers = [1, 2, 3, 4, 5]
for number in numbers:
    if number == 4:
        print("Found 4!")
        break
else:
    print("Did not find 4.")
    
#Example 3:
numbers = [1, 2, 3, 4, 5]
for number in numbers:
    if number == 6:
        print("Found 6!")
        break
else:
    print("Did not find 6.")
#Example 4:
numbers = [1, 2, 3, 4, 5]
for number in numbers:
    if number == 6:
        break
else:
    print('Loop completed successfully')
    
#Example 5:    
numbers = [1, 2, 3, 4, 5]
for number in numbers:
    if number == 3:
        print("Found 3")
        break
else:
    print('Loop completed successfully')
    

```

    apple
    Found 4!
    Did not find 6.
    Loop completed successfully
    Found 3
    


```python

```

    Found 4!
    Did not find 6.
    

## `map() and filter() functions`
    
The map() and filter() functions are built-in functions in Python that can be used to apply a function to each item in a sequence and return a new sequence.


```python
fruits = ['apple', 'banana', 'cherry']
fruits_length = list(map(len, fruits))
print(fruits_length)

fruits = ['apple', 'banana', 'cherry']
fruits_longer_than_5 = list(filter(lambda x: len(x) > 5, fruits))
print(fruits_longer_than_5)
```

    [5, 6, 6]
    ['banana', 'cherry']
    

## `List comprehensions`
List comprehensions are a concise way to create lists in Python. They are equivalent to a for loop with a single line of code that defines the expression for each item in the list.




```python
#Example 1: 
fruits = ['apple', 'banana', 'cherry']
fruits_length = [len(fruit) for fruit in fruits]
print(fruits_length)

#Example 2: 
# List comprehension that squares all numbers in a list
numbers = [1, 2, 3, 4, 5]
squared_numbers = [i**2 for i in numbers]
print(squared_numbers)

```

    [5, 6, 6]
    [1, 4, 9, 16, 25]
    

## `Generators`
Generators are a type of iterable in Python that allow you to produce a sequence of values one at a time. They are defined using a yield statement instead of a return statement.
python


```python
def count_up_to(n):
    i = 1
    while i <= n:
        yield i
        i += 1

for num in count_up_to(5):
    print(num)
```

    1
    2
    3
    4
    5
    

### Using `break` and `continue` statements in for loops

We can use the `break` and `continue` statements in for loops to control the flow of the loop. 
The `break` statement is used to exit a loop prematurely, while the `continue` statement is used to skip the current iteration and continue with the next iteration.


```python
#Example 1 :
numbers = [1, 2, 3, 4, 5]
for number in numbers:
    if number == 3:
        break
    print(number)
    
#Example 2 :
print("\t") ## To print the output in New line
numbers = [1, 2, 3, 4, 5]
for number in numbers:
    if number == 3:
        continue
    print(number)
    
#Example 3 :
print("\t") ## To print the output in New line    
# For loop that prints numbers from 1 to 10 with a break statement
for i in range(1, 11):
    if i == 5:
        break
    print(i)
    
#Example 4 :
print("\t") ## To print the output in New line
# For loop that prints only even numbers from 1 to 10 with a continue statement
for i in range(1, 11):
    if i % 2 != 0:
        continue
    print(i)

```

    1
    2
    	
    1
    2
    4
    5
    	
    1
    2
    3
    4
    	
    2
    4
    6
    8
    10
    


```python

```
