# Python Cheat Sheet

Here's a Python cheat sheet that covers some of the most commonly used syntax and constructs in the language:

### Intro:
* Python uses whitespace indentation instead of curly braces to delimit blocks of code.
* Use # to comment out a line or block of code.

### Variables and data types:
* Use = to assign a value to a variable.
* Python is dynamically typed, so you don't need to specify the data type of a variable explicitly.
* Basic data types include integers, floats, strings, booleans, and None.
* Use type() to check the data type of a variable.

```python
age = 27
weight = 68.5
name = "Alice"
is_student = True

# Checking data types of variables
print(type(age))        # Output: <class 'int'>
print(type(weight))     # Output: <class 'float'>
print(type(name))       # Output: <class 'str'>
print(type(is_student)) # Output: <class 'bool'>
print(type(nothing))    # Output: <class 'NoneType'>
```
In the above example,

* age is an integer variable representing the age of a person.
* weight is a float variable representing the weight of a person.
* name is a string variable representing the name of a person.
* is_student is a boolean variable representing whether a person is a student or not.
We can use these variables in our Python program to perform operations or make decisions based on their values.


### How to comments in code:
```python
# This is a single-line comment in Python
age = 27 # We can also add comments after a line of code

"""
This is a multi-line comment in Python.
We can use triple quotes to start and end a multi-line comment.
It's useful for documenting functions, classes, or modules.
"""

# Here's an example of using comments to explain code:
result = 10 + 20 # Add 10 to 20 and assign the result to a variable named result


```
In the above example, we use both single-line and multi-line comments to add notes to our code. We can use single-line comments by starting a line with the # symbol. We can also add comments after a line of code by using the # symbol at the end of the line. To add multi-line comments, we use triple quotes (""") to start and end the comment. We can use comments to explain what our code does or to add reminders to ourselves or other developers. In the last line of the example, we use a comment to explain what the code does.


### Taking Input from User:
```python
# Ask the user to enter their name and age
name = input("What is your name? ")
age = int(input("What is your age? "))

# Print a message to the user
print("Hello, " + name + "! You are " + str(age) + " years old.")

# Ask the user to enter a number and perform a calculation
num = int(input("Enter a number: "))
result = num * 10
print("The result is: " + str(result))

```
In the above example, we use the input() function to prompt the user to enter their name, age, and a number. Since the input() function always returns data as a string, we convert the age and the number to integers using the int() function. We then use these variables to print a message to the user and perform a simple calculation. By using the input() function, we can make our Python programs more interactive and dynamic.

### String in Python:
In Python, a string is a sequence of characters. Strings can be defined using either single quotes ' ' or double quotes " ", and can contain any combination of letters, digits, or symbols.

Here's an example of how to define and use strings in Python:
```python
# Define a string variable
message = "Hello, World!"

# Print the string to the console
print(message)

# Get the first character of the string
first_char = message[0]
print("The first character is:", first_char)

# Use string formatting to insert variables into a string
name = "Alice"
age = 30
greeting = f"My name is {name} and I am {age} years old."
print(greeting)

# Convert the string to uppercase
uppercase_message = message.upper()
print("Uppercase message:", uppercase_message)

# Replace a character in the string
new_message = message.replace("W", "w")
print("New message:", new_message)

```


### Operators:

#### Arithmetic Operators:
```python
# + adds two numbers
# - subtracts two numbers
# * multiplies two numbers
# / divides two numbers and returns a float
# % returns the remainder of a division
# ** raises the first number to the power of the second number

x = 5
y = 2

print(x + y)    # Output: 7
print(x - y)    # Output: 3
print(x * y)    # Output: 10
print(x / y)    # Output: 2.5
print(x % y)    # Output: 1
print(x ** y)   # Output: 25
```



#### Comparison Operators:
```python
# == checks if two values are equal
# != checks if two values are not equal
# < checks if the left value is less than the right value
# <= checks if the left value is less than or equal to the right value
# > checks if the left value is greater than the right value
# >= checks if the left value is greater than or equal to the right value
x = 5
y = 2
print(x == y)   # Output: False
print(x != y)   # Output: True
print(x < y)    # Output: False
print(x <= y)   # Output: False
print(x > y)    # Output: True
print(x >= y)   # Output: True
```



#### Logical Operators:
```python
"""
and returns True if both statements are True
or returns True if one of the statements is True
not reverses the result, returns False if the result is True
"""
x = 5
y = 2
z = 0

print(x > y and y > z)   # Output: True
print(x < y or y < z)    # Output: False
print(not x == y)        # Output: True

```

### Control flow statements
* if statement: executes a block of code if a certain condition is true.
* else statement: executes a block of code if the if condition is false.
* elif statement: allows you to check multiple conditions in sequence.
* while loop: repeatedly executes a block of code while a certain condition is true.
* for loop: iterates over a sequence (such as a list or tuple) and executes a block of code for each item.
### Lists
* A list is a collection of ordered items, enclosed in square brackets: my_list = [1, 2, 3]
* Use indexing to access individual items in a list: my_list[0] returns 1
* Use slicing to access a subset of items in a list: my_list[1:3] returns [2, 3]
* Use len() to get the length of a list.
### Strings
* A string is a collection of characters, enclosed in single or double quotes: my_string = 'hello'
* Use indexing and slicing with strings in the same way as with lists.
* Use string methods such as upper(), lower(), and replace() to manipulate strings.
### Functions
* A function is a block of code that performs a specific task.
* Define a function using the def keyword: def my_function(arg1, arg2):
* Use return to return a value from a function.
* Functions can have default arguments and variable-length argument lists.
### Modules
* A module is a file containing Python code that can be imported into another file.
* Use import to import a module: import math
* Use dot notation to access functions and variables in a module: math.sqrt(2)
This is just a brief overview of some of the most commonly used syntax and constructs in Python. There's much more to the language than this, but hopefully this cheat sheet will help you get started!



## here are some of the most common built-in functions and methods
### Built-in Functions:
 Function Name | Description
 --- | ----
 print() | used to print the output to the console 
 input() | used to take input from the user
 type()| used to determine the data type of an object
 len()| used to determine the length of an object (string, list, tuple, etc.)
 range() | used to create a sequence of numbers
 int(), float(), str(), bool() | used to convert objects to their respective data types
 max(), min() | used to determine the maximum and minimum values in an iterable
 sum() | used to calculate the sum of all elements in an iterable
 abs() | used to calculate the absolute value of a number
 round() | used to round a number to a specified number of decimal places
 enumerate() | used to iterate over a sequence while keeping track of the index
 zip() | used to iterate over multiple sequences in parallel
 sorted() | used to sort an iterable in ascending order
 reversed() | used to reverse the order of an iterable

### Common Methods:
 Function Extension Name | Description
 --- | ----
 .split() | used to split a string into a list based on a delimiter
 .join() | used to join elements of a list into a string
 .append() | used to add an element to the end of a list
 .pop() | used to remove and return the last element of a list
 .sort() | used to sort a list in ascending order
 .reverse() | used to reverse the order of a list
 .strip() | used to remove whitespace from the beginning and end of a string
 .replace() | used to replace a substring with another substring in a string
 .upper(), .lower() | used to convert a string to uppercase or lowercase, respectively
 .count() | used to count the number of occurrences of a substring in a string

These are just a few of the most common functions and methods in Python, but mastering them will provide you with a solid foundation to build upon as you continue to learn and grow as a Python programmer.
