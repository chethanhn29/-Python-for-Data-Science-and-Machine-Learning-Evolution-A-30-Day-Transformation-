“Day 5: Understanding Lists in Python(Part-2)”
Introduction:We have already Covererd properties ,types of List , basic list operations of adding, updating, deleting, and accessing elements in lists in the previous article.In this article we will cover rest of the List operations.

5.Slicing :
Slicing a list in Python allows accessing a portion of the list using the syntax: list_name[start_index: end_index: step].

The start_index is inclusive and default to 0, The end_index is exclusive, representing the index of the element right before the end of the slice, and is equal to (n-1) by default, where n is the length of the list.

The step represents the increments taken when moving from the start to the end of the slice, and is 1 by default, unless specified otherwise.


Example of List Slicing
There are two types of slicing in lists in Python: positive index slicing and negative index slicing.

a) Positive Index Slicing:Positive index slicing starts from the beginning of the list and moves towards the end of the list. It is represented by a colon (:) followed by the index number. For example, list[0:3] will return the first three elements in the list.

#Slicing a portion of a list:
>>fruits = ['apple', 'banana', 'cherry', 'orange', 'grapes']
>>print(fruits[1:3]) 
Output: ['banana', 'cherry']


#Slicing from the start of a list:
>>my_list = [1, 2, 3, 4, 5]
>>print(my_list[:3])
Output: [1, 2, 3]

#Slicing until the end of a list:
>>my_list = [1, 2, 3, 4, 5]
>>print(my_list[2:])
Output: [3, 4, 5]

#Slicing with a step value:
>>my_list = [1, 2, 3, 4, 5]
>>print(my_list[::2])
Output: [1, 3, 5]
##Here, the elements from index 1 to index 3 (exclusive) are being accessed by slicing the list.
b) Negative Index Slicing:Negative index slicing starts from the end of the list and moves towards the beginning of the list. It is represented by a colon (:) followed by a negative index number. For example, list[-3:-1] will return the last two elements in the list.

#Slicing a portion of a list using negative index:
>>fruits = ['apple', 'banana', 'cherry', 'orange', 'grapes']
>>print(fruits[-3:-1]) 
# Output: ['cherry', 'orange']

#Slicing from the start of a list using negative index:
>>my_list = [1, 2, 3, 4, 5]
>>print(my_list[:-2])
Output: [1, 2, 3]

#Slicing until the end of a list using negative index:
>>my_list = [1, 2, 3, 4, 5]
>>print(my_list[-3:])
Output: [3, 4, 5]

#Slicing with a step value using negative index:
>>my_list = [1, 2, 3, 4, 5]
>>print(my_list[::-2])
Output: [5, 3, 1]
##Here, the elements from the last third position to the last but one position (exclusive) are being accessed by slicing the list using negative index.
6.Searching:
Searching is an important operation when working with lists in Python. It allows us to determine if a specific element is present in the list and to retrieve its index position. Python provides several ways to search for elements in a list, such as using the in operator, the index method, and the count method.

a) Using the “in” operator: The “in” operator can be used to check if an element exists in a list. It returns a Boolean value of True or False.

fruits = ['apple', 'banana', 'cherry', 'orange', 'grapes']
if 'apple' in fruits:
print('apple is present in the list')
Output: apple is present in the list
b) Using index() method: The index() method can be used to find the index of an element in a list. If the element does not exist in the list, it will raise a ValueError.

fruits = ['apple', 'banana', 'cherry', 'orange', 'grapes']
print(fruits.index('cherry'))
Output: 2
c) Using count() method: The count() method returns the number of times an element appears in a list.

fruits = ['apple', 'banana', 'cherry', 'orange', 'grapes','apple']
print(fruits.count('apple'))
Output: 2
7.Sorting:
Sorting elements in a list is the process of arranging the elements of a list in a specific order. There are two types of sorting in Python, ascending sorting, and descending sorting.

There are two ways to sort a list in Python:

sort() method: Sorts the list in place.
sorted() function: Returns a new sorted list without modifying the original.

numbers = [3, 1, 4, 1, 5, 9, 2, 6, 5, 3, 5]

# sort() method
numbers.sort()
print(numbers) # Output: [1, 1, 2, 3, 3, 4, 5, 5, 5, 6, 9]

# sorted() function
sorted_numbers = sorted(numbers)
print(sorted_numbers) # Output: [1, 1, 2, 3, 3, 4, 5, 5, 5, 6, 9]
a) Ascending Sorting: It is the process of arranging the elements in increasing order. The default sorting order in Python is ascending.

#Example for ascending sorting for numbers:
>>numbers = [3, 1, 4, 1, 5, 9, 2, 6, 5, 3]
>>numbers.sort()
>>print(numbers)
 # Output: [1, 1, 2, 3, 3, 4, 5, 5, 6, 9]

#Example for ascending sorting for strings:
>>fruits = ['apple', 'banana', 'cherry', 'orange', 'grapes']
>>fruits.sort()
>>print(fruits)
# Output: ['apple', 'banana', 'cherry', 'grapes', 'orange']
b) Descending Sorting: It is the process of arranging the elements in decreasing order.

Example for descending sorting for numbers:
>>numbers = [3, 1, 4, 1, 5, 9, 2, 6, 5, 3]
>>numbers.sort(reverse=True)
>>print(numbers)
# Output: [9, 6, 5, 5, 4, 3, 3, 2, 1, 1]

Example for descending sorting for strings:
>>fruits = ['apple', 'banana', 'cherry', 'orange', 'grapes']
>>fruits.sort(reverse=True)
>>print(fruits)
# Output: ['orange', 'grapes', 'cherry', 'banana', 'apple']
8.Traversal:
Traversing a list means visiting each element in the list exactly once. This can be done using a loop, such as a for loop, to iterate over the list and access each element one by one. For example:

>>fruits = ['apple', 'banana', 'cherry', 'orange', 'grapes'] 
>>for fruit in fruits:
>> print(fruit)
##Output
apple
banana
cherry
orange
grapes
Traversing a list is useful for various operations like counting the number of elements in a list, printing all elements, summing up elements, etc.

9.Concatenation:
Concatenation refers to the process of combining two or more lists into a single list.

There are two types of concatenation in Python:

a) Concatenating two lists using the “+” operator: This method involves combining two lists by using the “+” operator to add the elements of one list to the end of the other list.

list1 = [1, 2, 3]
list2 = [4, 5, 6]
list3 = list1 + list2
print(list3) # Output: [1, 2, 3, 4, 5, 6]
b) Concatenating two lists using the extend() method: This method involves using the extend() method to add the elements of one list to the end of the other list. The extend() method is called on the list to which we want to add the elements and takes the list to be added as an argument.

list1 = [1, 2, 3]
list2 = [4, 5, 6]
list1.extend(list2)
print(list1) # Output: [1, 2, 3, 4, 5, 6]
10.Repetetion :
Repetition is a property in which the elements in a list are repeated a specified number of times to create a new list. This can be achieved by using the * operator. For example:

list1 = [1, 2, 3]
print(list1 * 3) 
# Output: [1, 2, 3, 1, 2, 3, 1, 2, 3]
##In this example, the list list1 is repeated 3 times to create a new list with 9 elements.

fruits = ['apple', 'banana', 'cherry']
print(fruits * 3)
# Output: ['apple', 'banana', 'cherry', 'apple', 'banana', 'cherry', 'apple', 'banana', 'cherry']
##Here, the fruits list is repeated 3 times resulting in a new list that contains the same elements 3 times.
11.Reverse:
Reversing: Reversing the elements of a list. The reverse() method can be used to reverse the elements of a list. Another method to reverse a list is slicing the list with a step value of -1, which returns the list in reverse order.

a) Reversing a List Using Slicing :

>>my_list = [1, 2, 3, 4, 5] 
>>print(my_list[::-1]) 
Output: [5, 4, 3, 2, 1]
Reversing a List Using the reverse() Method :

>>my_list = [1, 2, 3, 4, 5] 
>>my_list.reverse() print(my_list) 
Output: [5, 4, 3, 2, 1]
List Methods:
Lists in Python have a number of built-in methods that can be used to perform various operations on them. Some of the most commonly used list methods are:

append(): This method is used to add an element to the end of a list.Example: list.append(item)
insert(): This method is used to insert an element at a specific index in the list.Example: list.insert(index, item)
extend(): This method is used to extend a list by appending the elements from another list.Example: list.extend(another_list)
remove(): This method is used to remove an element from the list.Example: list.remove(item)
pop(): This method is used to remove an element from a specific index in the list.Example: list.pop(index)
count(): This method is used to count the number of times an element appears in the list.Example: list.count(item)
sort(): This method is used to sort the elements of the list in ascending order.Example: list.sort()
reverse(): This method is used to reverse the order of the elements in the list.Example: list.reverse()
index(): Returns the index of the first occurrence of a specified item. Example: list.index(item)
Difference between del keyword and remove() method:
The del keyword is used to delete an item from a list based on its index. For example: del list[2] will delete the third item in the list. On the other hand, the remove() method is used to delete an item from a list based on its value. For example: list.remove(2) will remove the first occurrence of the value 2 in the list.

Let’s take a look at some examples to understand these methods better.

Example 1: append() method
>>my_list = [1, 2, 3, 4, 5] 
>>my_list.append(6) 
>>print(my_list) 
# Output: [1, 2, 3, 4, 5, 6]

Example 2: insert() method
>>my_list = [1, 2, 3, 4, 5] 
>>my_list.insert(3, 6)
>> print(my_list) 
# Output: [1, 2, 3, 6, 4, 5]

Example 3: extend() method
my_list = [1, 2, 3, 4, 5]
 another_list = [6, 7, 8, 9] 
my_list.extend(another_list) 
print(my_list) 
# Output: [1, 2, 3, 4, 5, 6, 7, 8, 9]

Example 4: insert() method

This method allows you to insert an item at a specific index in a list. The syntax for the insert() method is:

list.insert(index, item)
where index is the position where you want to insert the item, and item is the value you want to insert. The index of the first item in a list is 0, and the index of the last item is len(list) — 1. Here’s an example:

>>> fruits = ['apple', 'banana', 'cherry']
>>> fruits.insert(1, 'grape')
>>> print(fruits)
['apple', 'grape', 'banana', 'cherry']
Example 5: remove() method.

This method is used to remove an item from a list based on its value. If the value is present in the list more than once, only the first occurrence is removed. The syntax for the remove() method is:

list.remove(item)
where “item” is the value you want to remove. Here’s an example:

>>> fruits = ['apple', 'banana', 'cherry', 'grape']
>>> fruits.remove('grape')
>>> print(fruits)
['apple', 'banana', 'cherry']
Example 6:pop() method.

This method is used to remove an item from a list based on its index. After using the pop() method it returns the Removed Value .The syntax for the pop() method is:

list.pop(index)
where index is the position of the item you want to remove. The index of the first item in a list is 0, and the index of the last item is len(list) — 1. Here’s an example:

>>> fruits = ['apple', 'banana', 'cherry']
>>> fruits.pop(1)
## Output : 'banana' 
>>> print(fruits)
['apple', 'cherry']
In this example, we first created a list of fruits, then we removed the item at index 1, which is ‘banana’. The list after the removal is now [‘apple’, ‘cherry’]. Note that the pop() method also returns the value of the removed item, which in this case is ‘banana’.

Now, let’s take a real-world example of a grocery list and perform various operations on it:

In this example, we have created a grocery list, performed various operations on it such as accessing an element, appending, removing, inserting, sorting, reversing, and finding the length.

# Grocery List
grocery_list = ["apples", "bananas", "cherries", "dates", "eggs"]

# Accessing an element in the list
print(grocery_list[2]) # Output: "cherries"

# Appending an element to the list
grocery_list.append("figs")
print(grocery_list) # Output: ["apples", "bananas", "cherries", "dates", "eggs", "figs"]

# Appending an element to the list
grocery_list.append("figs")
print(grocery_list) # Output: ["apples", "bananas", "cherries", "dates", "eggs", "figs"]

# Removing an element from the list
grocery_list.remove("dates")
print(grocery_list) # Output: ["apples", "bananas", "cherries", "eggs", "figs"]

# Inserting an element at a specific index
grocery_list.insert(1, "blueberries")
print(grocery_list) # Output: ["apples", "blueberries", "bananas", "cherries", "eggs", "figs"]

# Sorting the list
grocery_list.sort()
print(grocery_list) # Output: ["apples", "bananas", "blueberries", "cherries", "eggs", "figs"]

# Reversing the list
grocery_list.reverse()
print(grocery_list) # Output: ["figs", "eggs", "cherries", "blueberries", "bananas", "apples"]

# Finding the length of the list
print(len(grocery_list)) # Output: 6
let’s take another list of numbers and perform some common methods on it:

numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]

# append method
numbers.append(11)
print(numbers) # Output: [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11]

# insert method
numbers.insert(3, 15)
print(numbers) # Output: [1, 2, 3, 15, 4, 5, 6, 7, 8, 9, 10, 11]

# remove method
numbers.remove(15)
print(numbers) # Output: [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11]

# count method
count = numbers.count(4)
print(count) # Output: 1

# index method
index = numbers.index(7)
print(index) # Output: 6

# sort method
numbers.sort()
print(numbers) # Output: [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11]

# reverse method
numbers.reverse()
print(numbers) # Output: [11, 10, 9, 8, 7, 6, 5, 4, 3, 2, 1]

# clear method
numbers.clear()
print(numbers) # Output: []
Practice Questions:
Create a list containing the numbers from 1 to 5, another list of numbers 7 to 10, add both lists, insert 11 at index 3, delete 11, insert 6 at index 5, reverse and sort the final list.
Create a list containing the following elements: ‘apple’, ‘banana’, ‘cherry’,and then access the second element of the list ,Add ‘orange’ to the end of the list [‘apple’, ‘banana’, ‘cherry’], and Remove the first occurrence of ‘cherry’ from the list [‘apple’, ‘banana’, ‘cherry’].
Create a list of strings [‘apple’, ‘banana’, ‘cherry’, ‘date’, ‘elderberry’]. Find the length of the list, add the string ‘fig’ at the end of the list, remove the string ‘banana’, insert the string ‘blackberry’ at index 2, find the index of the string ‘date’, reverse the list and sort it in ascending order.
Create a list of numbers from 11 to 20, then find the maximum number, the minimum number and the sum of all numbers. Then, extend the list by adding a list of numbers from 21 to 25, reverse the list and remove the number 21. After that, insert the number 30 at index 4, count the number of occurrences of 15, sort the list in descending order and finally, slice the list to print only the numbers from index 2 to index 7.
You can find the more Practice Questions and answers to each of the questions Here.

Conclusion:
In conclusion, this article has covered the Remaining List operations in python, and use of built-in methods and operations.The article has provided a foundation for further exploration of more advanced topics such as List Comprehension, Removing duplicates from a list ,Using loops to iterate through lists ,Nested lists ,List filtering and Using lists with other data structures such as tuples and dictionaries which we will discuss in the upcoming sessions.
