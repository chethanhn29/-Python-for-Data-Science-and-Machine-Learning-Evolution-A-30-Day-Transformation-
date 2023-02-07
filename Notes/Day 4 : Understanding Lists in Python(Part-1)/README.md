“Day 4 : Understanding Lists in Python(Part-1)”
Introduction of Lists:
In this series, we explored the basics of Python data types, including numbers, decimal values, and words and Different operators used in Python.

But Have you ever wished you could group items together in Python, like items in a shopping cart,grocery list, student roster, exam scores or names on a guest list?

Enter lists, the dynamic data type that lets you organize your data in an intuitive and flexible way.In this article, we will dive into the various aspects of lists in Python, including its definition, data structure content, and real-world examples.

What are Lists in Python?

A list is a collection of items, separated by commas, and enclosed within square brackets. Each item in the list is referred to as an element. Lists are mutable, meaning you can change the elements in a list after it has been created, which is useful for creating dynamic data structures that change over time.

Lists are useful in Python because they provide a flexible and convenient way to store and manipulate collections of data. Lists allow you to group together items of different data types, such as numbers, strings, and other lists, and they provide a number of built-in methods and operators to perform operations on these collections. Here’s an example of a simple list in Python:

fruits = [‘apple’, ‘banana’, ‘cherry’]

Properties of Lists:
Mutable: Lists are mutable, meaning you can change the elements in a list after it has been created.
Ordered: Lists are ordered, meaning the elements in a list have a specific order that can be accessed using indices.
Versatile: Lists can contain elements of different data types, including numbers, strings, and even other lists.
Accessible: The elements of a list can be easily accessed using indices, making it convenient for retrieving specific elements.
Types of Lists:
Arrays: An array is a collection of elements stored in contiguous memory locations. The elements can be of any data type, and the size of an array is fixed once it is declared.
Linked Lists: A linked list is a collection of nodes, where each node contains an element and a reference to the next node in the list. Linked lists are dynamic in size and can grow or shrink dynamically.
Stacks: A stack is a data structure that follows the Last In First Out (LIFO) principle. Elements are added and removed from the top of the stack.
Queues: A queue is a data structure that follows the First In First Out (FIFO) principle. Elements are added at the end of the queue and removed from the front.
we will disuss detailed about above types of lists in upcoming days.

Creating a List in Python: In Python, creating a list is very simple. All you have to do is assign a collection of values to a variable, separated by commas and enclosed within square brackets. Here’s an example:

#Creating a list of numbers: 
numbers = [1, 2, 3, 4, 5]

#Creating a list of strings
words = ["apple", "banana", "cherry"]

#Creating a mixed list
mixed = [1, "apple", 3.14, True]
Indexing in Lists:
Indexing is a process of accessing elements from a list based on their position or location within the list. This allows you to retrieve a specific item in the list without having to iterate through the entire list.

Indexing is important in lists because it makes it easier to manipulate and organize data within the list.

Remember in indexing always starts from 0 in Positive index ,But in Negative index Index will start from -1.


Max, Min, and Sum of Lists:These are the Built in Functions in Pythonand are available in the python standard library.

The max() function is used to retrieve the largest element in a list. The function takes the list as an argument and returns the largest element in the list. For example, consider the following list of numbers:

numbers = [1, 5, 2, 8, 10]
 maximum = max(numbers) 
print(maximum)
# Output: 10
The min() function is used to retrieve the smallest element in a list. The function takes the list as an argument and returns the smallest element in the list. For example, consider the following list of numbers:

numbers = [1, 5, 2, 8, 10]
 minimum = min(numbers) 
print(minimum)
# Output : 1
The sum() function is used to calculate the sum of all elements in a list. The function takes the list as an argument and returns the sum of all elements in the list. For example, consider the following list of numbers:

numbers = [1, 5, 2, 8, 10] 
total = sum(numbers) 
print(total)
#output : 26
List Operations:
In Python, you can perform several operations on lists, such as concatenation, repetition, and slicing.

Insertion: Adding a new element to the list.
Accessing: Retrieving an element from the list based on its position.
Updating: Changing the value of an element in the list.
Deletion: Removing an element from the list.
Slicing : To get the Portion of List
Concatenation: Combining two or more lists into a single list.
Searching: Finding an element in the list.
Sorting: Arranging the elements in a specific order.
Traversal: Visiting each element in the list.
Repetition: The repetition of an action, process, or pattern.
Reverse: The act of reversing the order of elements in a list, so that the first element becomes the last, the second element becomes the second to last, and so on.
1. Insertion or Adding Elements to a List:
Insertion involves adding a new element to the list. There are several ways to insert an element into a list, including inserting at the beginning, end, or a specific position in the list.

Most common ways to insert an element into a list are append(),Insert(),Extend() Methods.

a) append() : This method adds an element to the end of a list.

>>> a = [1, 2, 3]
>>> a.append(4)
>>> print(a)
[1, 2, 3, 4]

>>> fruits = ['apple', 'banana', 'cherry']
>>> fruits.append('orange')
>>> print(fruits)  
['grapes', 'banana', 'cherry', 'orange']
b) insert() : This method inserts an element at a specified position in a list.

>>> a = [1, 2, 3]
>>> a.insert(1, 4)
>>> print(a)
[1, 4, 2, 3]
c) extend() : This method adds all elements of a given list to the end of the original list.

>>> a = [1, 2, 3]
>>> b = [4, 5, 6]
>>> a.extend(b)
>>> print(a)
[1, 2, 3, 4, 5, 6]
2. Accessing Elements in a List:
Accessing elements in a list means retrieving or reading the values stored in a specific index of the list. There are several ways to access elements in a list in Python:

Indexing: Accessing elements using their index number in square brackets.
Negative indexing: Accessing elements using negative index numbers.
Slicing: Accessing elements in a range by slicing the list.
Iteration: Looping through the list and accessing its elements one by one.
a) Indexing :

You can access an element of a list by using square brackets [] and the index of the element you want to access. Indexing starts from 0, so the first element has an index of 0, the second element has an index of 1, and so on. For example, list[2] would return the third element of the list.

numbers = [1, 2, 3, 4, 5]
words = ["apple", "banana", "cherry"]
mixed = [1, "apple", 3.14, True]

#Accessing Elements in the above Lists by indesing method:
print(numbers[0]) # Output: 1
print(words[1]) # Output: "banana"
print(mixed[2]) #
 Output: 3.14
b) Negative Indexing:
You can access elements from the end of the list by using negative indices. For example, list[-1] would return the last element of the list.

fruits = ['apple', 'banana', 'cherry']
print(fruits[-1]) # Output: 'cherry'
Here, the last element of the list is being accessed using negative index number -1.

c) Slicing:

You can access a portion of a list by using slicing. Slicing is done by using two indices separated by a colon( : ) . The first index is the starting position and the second index is the ending position. For example, list[1:3] would return a new list containing the second and third elements of the original list.

The syntax for slicing a list is as follows: list_name[start_index : end_index : step].

The start_index is inclusive and if the start_index didn’t mentioned in the syntax List will consider starting_index as (0), while the end_index is exclusive and step is steps(Increments) to take from start to end.

Slicing a portion of a list:
fruits = ['apple', 'banana', 'cherry', 'orange', 'grapes']
print(fruits[1:3]) # Output: ['banana', 'cherry']

Slicing a portion of a list:
my_list = [1, 2, 3, 4, 5]
print(my_list[1:3])
Output: [2, 3]

Slicing from the start of a list:
my_list = [1, 2, 3, 4, 5]
print(my_list[:3])
Output: [1, 2, 3]

Slicing until the end of a list:
my_list = [1, 2, 3, 4, 5]
print(my_list[2:])
Output: [3, 4, 5]

Slicing with a step value:
my_list = [1, 2, 3, 4, 5]
print(my_list[::2])
Output: [1, 3, 5]
Here, the elements from index 1 to index 3 (exclusive) are being accessed by slicing the list.

d) Iteration or Looping:

You can loop through a list and access its elements one by one. This can be done using a for loop. For example, the following code would print out each element of the list:

fruits = ['apple', 'banana', 'cherry']
for fruit in fruits:
 print(fruit)
# Output:
# apple
# banana
# cherry
Here, the elements of the list are being accessed one by one using a for loop.

3. Updating Elements or Modifying elements in a List:
we can modify the elements of List by assigning a values for particular index of the index or by assigning values to the portion of list(Slicing),and by Looping.

a) Indexing: You can access an element of a list using its index and assign a new value to it.

fruits = ['apple', 'banana', 'cherry']
fruits[0] = 'grapes'
print(fruits)  # Output: ['grapes', 'banana', 'cherry']

numbers = [1, 2, 3, 4, 5]
numbers[0] = 10
print(numbers) # Output: [10, 2, 3, 4, 5]
b) Using a loop: You can use a loop to iterate through the elements of a list and modify them as desired.

numbers = [1, 2, 3, 4, 5]
for i in range(len(numbers)):
 numbers[i] = numbers[i] * 2
print(numbers) # Output: [2, 4, 6, 8, 10]
c) Using a slice: You can update a range of elements in a list by slicing it and assigning a new list to the sliced portion.

numbers = [1, 2, 3, 4, 5]
numbers[1:3] = [10, 20]
print(numbers) # Output: [1, 10, 20, 4, 5]
4.Deleting Elements from a List:
You can delete elements from a list in Python using the del keyword or the remove() method and pop() method. The del keyword deletes the element at a specific index, while the remove() method deletes the first occurrence of a specific value.

a) Using the del statement: del is used to delete elements from a list based on their index. This method is useful when you want to remove an item from a specific position in the list.

Example 1:
>>> my_list = [1, 2, 3, 4, 5]
>>> del my_list[2]
>>> print(my_list)
[1, 2, 4, 5]

Example 2:
>>> my_list = [1, 2, 3, 4, 5]
>>> del my_list[1:3]
>>> print(my_list)
[1, 4, 5]
b) Using the remove method: remove is used to remove the first occurrence of a specific value in the list. This method is useful when you want to remove an item based on its value.

Example 1:
>>> my_list = [1, 2, 3, 4, 5]
>>> my_list.remove(3)
>>> print(my_list)
[1, 2, 4, 5]

Example 2:
>>> my_list = [1, 2, 3, 4, 5, 4]
>>> my_list.remove(4)
>>> print(my_list)
[1, 2, 3, 5, 4]
c) Using the pop method: pop is used to remove an item from the list based on its index. Unlike del, pop also returns the value that is removed. This method is useful when you want to remove an item and also use its value.

Example 1:
>>> my_list = [1, 2, 3, 4, 5]
>>> item = my_list.pop(2)
>>> print(my_list)
[1, 2, 4, 5]
>>> print(item)
3


Example 2:
>>> my_list = [1, 2, 3, 4, 5]
>>> item = my_list.pop()
>>> print(my_list)
[1, 2, 3, 4]
>>> print(item)
5
Conclusion :
In conclusion, this article has covered the basics of lists in Python, including their creation, modification and basic list operations of adding, updating, deleting, and accessing elements in lists. Other important list operations such as sorting, merging, slicing, and iterating through lists will be covered in the “Lists in Python(Part-2)” of the series, offering a more comprehensive understanding of lists and their use in programming.
