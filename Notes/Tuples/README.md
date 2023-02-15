# `Tuples`
A tuple is an ordered, immutable, and heterogeneous collection of elements. It is defined using round brackets ( ) and each element is separated by a comma. For example, you can create a tuple containing integers, strings, and lists like this:

t = (1, 'Hello', [1, 2, 3])
![Screenshot%20%28194%29.png](attachment:Screenshot%20%28194%29.png)


## `Tuples Properties`

#### 1.Indexing:
Elements in a tuple can be accessed using indexing, starting from 0. Negative indexing is also possible, where -1 refers to the last element in the tuple.

my_tuple = (1, 2, 3, 4, 5)

print(my_tuple[2]) # Output: 3


#### 2.Immutable:
Tuples are immutable, which means that their elements cannot be changed once they are created.

#### 3.Heterogeneous: 
Tuples can contain elements of different data types, such as integers, strings, lists, etc.

#### 4.Packing and Unpacking: 
Tuples can be packed and unpacked. Packing is the process of creating a tuple from individual elements, while unpacking is the process of extracting elements from a tuple.

#### 5.Methods:
Some of the common methods for tuples are len(), count(), and index().

#### 6.Iteration: 
Tuples can be iterated over, just like lists.

#### 7.Comparison: 
Tuples can be compared to each other element-wise. If all elements in a tuple are equal to the corresponding elements in another tuple, then the two tuples are equal.

#### 8.Usage: 
Tuples are commonly used for returning multiple values from a function, for grouping data together, and for representing points in geometry, among other things.
#### 9.Optimized for Access: 
Accessing elements in a tuple is faster than accessing elements in a list.

#### 10.Nested: 
Tuples can contain other tuples as elements.


## `Built-In Functions`

all()	Returns true if all element are true or if tuple is empty

any()	return true if any element of the tuple is true. if tuple is empty, return false

len()	Returns length of the tuple or size of the tuple

enumerate()	Returns enumerate object of tuple

max()	return maximum element of given tuple

min()	return minimum element of given tuple

sum()	Sums up the numbers in the tuple

sorted()	input elements in the tuple and return a new sorted list

tuple()	Convert an iterable to a tuple.

## `Creating Tuples`
Tuples can be created in several ways in Python. Here are some of the most common methods for creating tuples:

#### Creating a tuple using parentheses
 You can create a tuple by enclosing a comma-separated list of elements in parentheses.

####  Creating a tuple using the tuple function
You can create a tuple from any iterable (such as a list) using the tuple() function.

####  Creating a tuple with a single element
If you want to create a tuple with a single element, you need to include a comma after the element.


```python
#Creating a tuple using parentheses
my_tuple = (1, 2, 3, 4, 5)
print("\nTuple created by using parentheses: ")
print(my_tuple) #  Output: (1, 2, 3, 4, 5)

#Creating a tuple using the tuple function
my_list = [1, 2, 3, 4, 5]
my_tuple = tuple(my_list)
print("\nTuple created by using the tuple function: ")
print(my_tuple) # Output: (1, 2, 3, 4, 5)

#Creating a tuple with a single element
single_tuple = (1,)
print("\nTuple with single element: ")
print(single_tuple) # Output: (1,)

# Creating a Tuple
# with nested tuples
Tuple1 = (0, 1, 2, 3)
Tuple2 = ('python', 'geek')
Tuple3 = (Tuple1, Tuple2)
print("\nTuple with nested tuples: ")
print(Tuple3)
 
# Creating a Tuple
# with repetition
Tuple1 = ('Geeks',) * 3
print("\nTuple with repetition: ")
print(Tuple1)
 
# Creating a Tuple
# with the use of loop
Tuple1 = ('Geeks')
n = 5
print("\nTuple with a loop")
for i in range(int(n)):
    Tuple1 = (Tuple1,)
    print(Tuple1)
```

    
    Tuple created by using parentheses: 
    (1, 2, 3, 4, 5)
    
    Tuple created by using the tuple function: 
    (1, 2, 3, 4, 5)
    
    Tuple with single element: 
    (1,)
    
    Tuple with nested tuples: 
    ((0, 1, 2, 3), ('python', 'geek'))
    
    Tuple with repetition: 
    ('Geeks', 'Geeks', 'Geeks')
    
    Tuple with a loop
    ('Geeks',)
    (('Geeks',),)
    ((('Geeks',),),)
    (((('Geeks',),),),)
    ((((('Geeks',),),),),)
    

## `Accessing Tuple Elements`

To access elements in a tuple, you use indexing. The index of the first element in a tuple is 0, the second element has an index of 1, and so on. You can use negative indexing to access elements from the end of the tuple. For example, the last element in a tuple can be accessed using an index of -1. Here is an example that demonstrates accessing elements in a tuple:

t = (1, 'Hello', [1, 2, 3])

print(t[0]) # 1

print(t[1]) # 'Hello'

print(t[2]) # [1, 2, 3]

print(t[-1]) # [1, 2, 3]


## `Tuple Methods`

Tuples have several built-in methods that can be used to perform various operations. Some of the most commonly used methods are:

#### len(): 
This method returns the number of elements in a tuple.

#### count(): 
This method returns the number of times an element appears in a tuple.

#### index(): 
This method returns the index of the first occurrence of an element in a tuple.


#### tuple(iterable): 
 Converts an iterable (such as a list) into a tuple.


Here is an example that demonstrates using these methods:

t = (1, 2, 3, 4, 5, 1, 2)

print(len(t)) # 7

print(t.count(1)) # 2

print(t.index(3)) # 2

l = [1, 2, 3]
t = tuple(l)
print(t) # (1, 2, 3)



### `Iterating Over Tuples`

Tuples can be iterated over just like lists. You can use a for loop to iterate over the elements in a tuple and perform some operation on each element. Here is an example that demonstrates iterating over a tuple:



```python
t = (1, 2, 3, 4, 5)
for x in t:
    print(x)
```

    1
    2
    3
    4
    5
    

###  `Tuple Comprehensions`

Just like list comprehensions, you can also create tuples using tuple comprehensions. This is a concise way to create new tuples from existing tuples. Here is an example that demonstrates creating a tuple using a tuple comprehension:


```python
t = (1, 2, 3, 4, 5)
squared = tuple(x**2 for x in t)
print(squared)
```

    (1, 4, 9, 16, 25)
    

### `Tuple Unpacking`

Tuple unpacking is a useful feature that allows you to unpack the elements of a tuple into separate variables. This is useful when you have a tuple that contains multiple values and you want to assign each value to a separate variable. Here is an example that demonstrates tuple unpacking:



```python
t = (1, 2, 3)
a, b, c = t
print(a) # 1
print(b) # 2
print(c) # 3
```

    1
    2
    3
    

### `Nested Tuples`

A nested tuple is a tuple that contains another tuple as its element. You can nest tuples as many times as you want, resulting in a hierarchical structure of tuples.

To access elements in a nested tuple, you can use multiple indexing operations. Here is an example that demonstrates creating and accessing elements in a nested tuple:


```python
t = (1, (2, 3), 4)
print(t[1]) # (2, 3)
print(t[1][0]) # 2

```

    (2, 3)
    2
    

### Converting Tuples to Lists and Vice Versa

It is possible to convert tuples to lists and vice versa using the `list()` and `tuple()` functions. This can be useful when you need to perform operations that are only available for lists on tuples, or when you need to convert a list to a tuple for use in a particular context. Here is an example that demonstrates converting a tuple to a list and back to a tuple:



```python
t = (1, 2, 3)
l = list(t)
print(l) # [1, 2, 3]
t = tuple(l)
print(t) # (1, 2, 3)
```

    [1, 2, 3]
    (1, 2, 3)
    

### zip() function in tuples
The zip function in Python is a built-in function that allows you to combine multiple iterables into one iterable. When used with tuples, the zip function takes multiple tuples as arguments and returns a tuple of tuples, where each inner tuple contains elements from each of the input tuples.

Here's an example of how the zip function can be used with tuples:


```python
a = (1, 2, 3)
b = (4, 5, 6)
c = (7, 8, 9)

zipped = zip(a, b, c)
print(list(zipped))
```

    [(1, 4, 7), (2, 5, 8), (3, 6, 9)]
    

In this example, zip takes three tuples a, b, and c as arguments and returns a tuple of tuples, where each inner tuple contains elements from each of the input tuples.

Note that the length of the returned zip object is determined by the length of the shortest input iterable. If one of the input tuples is shorter than the others, then the resulting zip object will also be shorter.

Additionally, you can use the zip function to unzip a list of tuples into separate lists, like this:



```python


zipped = [(1, 4, 7), (2, 5, 8), (3, 6, 9)]
a, b, c = zip(*zipped)
print(a)
print(b)
print(c)
#In this example, zip is used with the * operator to unzip the list of tuples zipped into three separate lists.
```

    (1, 2, 3)
    (4, 5, 6)
    (7, 8, 9)
    

### `Tuples VS Lists:`

![word-image-344.png](attachment:word-image-344.png)

#### Similarities	

Functions that can be used for both lists and tuples:
len(), max(), min(), sum(), any(), all(), sorted()

Methods that can be used for both lists and tuples:  count(), Index()
    
Tuples can be stored in lists.

Lists can be stored in tuples

Both ‘tuples’ and ‘lists’ can be nested.


#### Differences

Methods that cannot be used for tuples:
append(), insert(), remove(), pop(), clear(), sort(), reverse()

we generally use ‘tuples’ for heterogeneous (different) data types and ‘lists’ for homogeneous (similar) data types.

Iterating through a ‘tuple’ is faster than in a ‘list’.

‘Lists’ are mutable whereas ‘tuples’ are immutable.

Tuples that contain immutable elements can be used as a key for a dictionary.


Tuples and lists are similar in many ways, but there are some key differences between them. One of the main differences is that tuples are immutable, while lists are mutable. This means that you cannot change the elements in a tuple once it is created, but you can change the elements in a list.

Another difference between tuples and lists is that tuples are generally used to represent a collection of heterogeneous values, while lists are used to represent a collection of homogeneous values. This means that tuples can contain elements of different data types, while lists are typically used to store elements of the same data type.

In general, tuples are more efficient than lists for representing and processing collections of data, since they are immutable and can be used as keys in dictionaries. On the other hand, lists are more flexible than tuples, since they are mutable and can be used for a wider range of tasks.



### `Tuple as Keys in Dictionaries:`

In Python, you can use tuples as keys in dictionaries as long as the elements in the tuple are hashable. Hashable objects have a hash value that never changes during their lifetime, making them suitable for use as dictionary keys. Examples of hashable objects include numbers, strings, and tuples that contain only hashable objects. Here's an example of using a tuple as a key in a dictionary:



```python
d = {(1, 2): 'tuple key'}
print(d[(1, 2)]) # 'tuple key'
```

    tuple key
    

### Concatenation: 
Tuples can be concatenated using the + operator to create a new tuple.The new tuple will contain all the elements from both tuples. Here's an example:


```python
t1 = (1, 2, 3)
t2 = (4, 5, 6)
t3 = t1 + t2
 # Printing Final Tuple
print("\nTuples after Concatenation: ")
print(t3)
```

    
    Tuples after Concatenation: 
    (1, 2, 3, 4, 5, 6)
    

### Slicing:
Tuples support slicing, which allows you to extract a sub-tuple from a larger tuple. Slicing uses the square brackets [] with a start and stop index separated by a colon :. Here's an example:




```python
# Slicing of a Tuple
t = (1, 2, 3, 4, 5, 6)
print(t[2:5]) # (3, 4, 5)
```

    (3, 4, 5)
    


```python
# Slicing of a Tuple
# with Numbers
Tuple1 = tuple('GEEKSFORGEEKS')
print("Before Slicing tuple ",Tuple1)
# Removing First element
print("slicing after first elemnent: ")
print(Tuple1[1:])
 
# Reversing the Tuple
print("\nTuple after sequence of Element is reversed: ")
print(Tuple1[::-1])
 
# Printing elements of a Range
print("\nPrinting elements between Range 4-9: ")
print(Tuple1[4:9])
```

    Before Slicing tuple  ('G', 'E', 'E', 'K', 'S', 'F', 'O', 'R', 'G', 'E', 'E', 'K', 'S')
    slicing after first elemnent: 
    ('E', 'E', 'K', 'S', 'F', 'O', 'R', 'G', 'E', 'E', 'K', 'S')
    
    Tuple after sequence of Element is reversed: 
    ('S', 'K', 'E', 'E', 'G', 'R', 'O', 'F', 'S', 'K', 'E', 'E', 'G')
    
    Printing elements between Range 4-9: 
    ('S', 'F', 'O', 'R', 'G')
    

### Tuple as Function Arguments:

Tuples can be used as function arguments, allowing multiple arguments to be passed to a function as a single tuple. This can be useful when you need to pass a variable number of arguments to a function. Here's an example of a function that takes a tuple as an argument:



```python
def add_tuple(t):
    return sum(t)

print(add_tuple((1, 2, 3))) # 6
```

    6
    

## Deleting a Tuple
Tuples are immutable and hence they do not allow deletion of a part of it. The entire tuple gets deleted by the use of del() method. 

Note- Printing of Tuple after deletion results in an Error. 


```python
# Deleting a Tuple
Tuple1 = (0, 1, 2, 3, 4)
del Tuple1
 
print(Tuple1)
```


    ---------------------------------------------------------------------------

    NameError                                 Traceback (most recent call last)

    ~\AppData\Local\Temp\ipykernel_15756\2722297116.py in <module>
          3 del Tuple1
          4 
    ----> 5 print(Tuple1)
    

    NameError: name 'Tuple1' is not defined


### Returning Multiple Values from a Function
In Python, you can return multiple values from a function using a tuple. For example, consider a function that returns the sum and product of two numbers:




```python
def sum_product(a, b):
    return a + b, a * b

result = sum_product(3, 4)
print(result)
#You can then access the individual elements of the returned tuple:
sum = result[0]
product = result[1]
print("Sum:", sum)
print("Product:", product)
```

    (7, 12)
    Sum: 7
    Product: 12
    

### Swapping Values
Tuples can be used to swap the values of two variables without using a temporary variable.For example, you can write a, b = b, a to swap the values of two variables a and b.


```python
a = 1
b = 2
a, b = b, a
print("a:", a)
print("b:", b)
```

    a: 2
    b: 1
    

### if a element in nested tuple is a list, can we change the values of list
Yes, you can change the values of a list that is an element within a nested tuple. Lists are mutable, so you can modify their elements directly. Here's an example to demonstrate this:


```python
original_tuple = ((1, 2, 3), [4, 5, 6], (7, 8, 9))
original_tuple[1][1] = 10

print(original_tuple) # ((1, 2, 3), [4, 10, 6], (7, 8, 9))
```

    ((1, 2, 3), [4, 10, 6], (7, 8, 9))
    

In the example above, we modify the second element in the list (which is at index 1) to be 10. Note that this change only affects the list within the tuple and not the tuple itself.



### can we change the element tuples values inside the nested list
Yes, you can change the values of elements within nested tuples that are inside a list. However, since tuples are immutable, you will need to create a new tuple with the updated values and then replace the original tuple in the list with the new one. Here's an example to demonstrate this:





```python
original_list = [(1, 2, 3), (4, 5, 6), (7, 8, 9)]
new_tuple = (10, 11, 12)
original_list[1] = new_tuple

print(original_list) # [(1, 2, 3), (10, 11, 12), (7, 8, 9)]
```

    [(1, 2, 3), (10, 11, 12), (7, 8, 9)]
    

In the example above, we create a new tuple new_tuple with the updated values and then replace the second tuple in the list (which is at index 1) with the new tuple.

## `Advanced Topics on Tuples`


### Performance: 
Tuples are generally faster than lists in terms of indexing, iteration, and memory usage, as they are immutable. 

This means that once a tuple is created, you cannot change its contents, making it more efficient for certain operations. For example, when indexing a tuple, Python can access the desired element directly without having to search through the entire collection. Additionally, since tuples have a fixed size, they use less memory than lists, which can grow dynamically.


### Named Tuples:
Named tuples are a subclass of tuples and allow you to access elements using named attributes instead of indexes. Named tuples are created using the namedtuple function from the collections module.


### Tuple as a Return Value: 
Tuples can be used as a return value from a function to return multiple values. This can be useful when you want to return multiple values from a function, but don't want to use a dictionary or class.


### Tuple in Comparison Operations: 
Tuples can be compared using the usual comparison operators such as <, >, <=, >=, ==, and !=. When comparing tuples, the comparison is done element-wise and stops as soon as a non-equal element is found.

### Tuple in Sorting: 
Tuples can be sorted based on their elements. The sorting is done based on the first element of the tuple, and if the first elements are equal, then the second elements are compared, and so on. You can use the sorted() function to sort a list of tuples.



## Practice Questions

1. Create a tuple with the following elements: 1, 2, 3, 4, 5.

2. Access the second element of the tuple.

3. Slice the tuple to get the elements 2 to 4.

4. Count the number of occurrences of the number 3 in the tuple.

5. Get the index of the first occurrence of the number 2 in the tuple.

6. Create a tuple with two elements: the name and age of a person.

7. Write a function that takes two numbers as arguments and returns their sum and product as a tuple.

8. Swap the values of two variables using a tuple.

9. Unpack the elements of a tuple into separate variables.


## Answers




```python
# 1.Create a tuple with five elements, and print its length.
t = (1, 2, 3, 4, 5)
print(len(t))  # Output: 5

# 2.Access the third element of a tuple and print it.
t = (1, 2, 3, 4, 5)
print(t[2])  # Output: 3

# 3.Concatenate two tuples and print the result.
t1 = (1, 2, 3)
t2 = (4, 5, 6)
t3 = t1 + t2
print(t3)  # Output: (1, 2, 3, 4, 5, 6)

# 4.Unpack the elements of a tuple into separate variables and print them.
t = (1, 2, 3)
a, b, c = t
print(a, b, c)  # Output: 1 2 3

# 5.Slice a tuple and print the result.
t = (1, 2, 3, 4, 5)
print(t[1:3])  # Output: (2, 3)

# 6.Count the number of occurrences of an element in a tuple and print the result.
t = (1, 2, 3, 2, 1, 4, 2)
print(t.count(2))  # Output: 3

# 7.Sort a list of tuples based on the first element of each tuple, and print the result.
t = [(3, 4), (1, 2), (5, 6), (2, 3), (4, 5)]
print(sorted(t, key=lambda x: x[0]))  # Output: [(1, 2), (2, 3), (3, 4), (4, 5), (5, 6)]

```

    5
    3
    (1, 2, 3, 4, 5, 6)
    1 2 3
    (2, 3)
    3
    [(1, 2), (2, 3), (3, 4), (4, 5), (5, 6)]
    


```python

```
