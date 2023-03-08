# Python Cheat Sheet

Here's a Python cheat sheet that covers some of the most commonly used syntax and constructs in the language:

### Intro:
* Python uses whitespace indentation instead of curly braces to delimit blocks of code.
* Use # to comment out a line or block of code.

### Variables and data types:
* Use = to assign a value to a variable.
* Python is dynamically typed, so you don't need to specify the data type of a variable explicitly.
* Basic data types include integers, floats, strings, booleans, and None.


```python
# This is an integer variable
x = 5

# This is a float variable
y = 3.14

# This is a boolean variable
z = True

# This is a string variable
name = "John"

# This is a list variable
fruits = ["apple", "banana", "orange"]

# This is a tuple variable
coordinates = (2.5, 3.0)

# This is a dictionary variable
person = {"name": "John", "age": 30, "city": "New York"}

# Print the values of the variables
print(x)  # Output: 5
print(y)  # Output: 3.14
print(z)  # Output: True
print(name)  # Output: John
print(fruits)  # Output: ['apple', 'banana', 'orange']
print(coordinates)  # Output: (2.5, 3.0)
print(person)  # Output: {'name': 'John', 'age': 30, 'city': 'New York'}

```

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

#### Here's an example of an if statement in Python:
```python
x = 10

if x > 0:
    print("x is positive")

```
In this example, we have a variable x with a value of 10. The if statement checks if x is greater than 0, and if so, it executes the code inside the block (in this case, it prints "x is positive").

####  here's an example of an else statement:

```python
x = -5

if x > 0:
    print("x is positive")
else:
    print("x is not positive")

```
In this example, we have the same variable x, but this time it has a value of -5. The if statement checks if x is greater than 0, and if so, it executes the code inside the first block (prints "x is positive"). If x is not greater than 0, it executes the code inside the else block instead (prints "x is not positive").

#### Finally, here's an example of an elif (short for "else if") statement:

```python
x = 0

if x > 0:
    print("x is positive")
elif x < 0:
    print("x is negative")
else:
    print("x is zero")

```
In this example, we have the same variable x, but this time it has a value of 0. The if statement checks if x is greater than 0, and if so, it executes the code inside the first block (prints "x is positive"). If x is not greater than 0, it moves on to the elif statement and checks if x is less than 0. If x is less than 0, it executes the code inside the elif block (prints "x is negative"). If neither the if nor elif conditions are true, it executes the code inside the else block instead (prints "x is zero").

#### Here's an example of a for loop in Python with the result printed in the output:
```python
fruits = ["apple", "banana", "cherry"]

for fruit in fruits:
    print(fruit)

# Output:
# apple
# banana
# cherry

```
In this example, we have a list of fruits containing three elements: "apple", "banana", and "cherry". The for loop iterates over each element in the list and assigns it to the variable fruit. Then, the print() function is called inside the loop with fruit as the argument, so each fruit in the list is printed to the console.


#### here's an example of a while loop in Python with the output:
```python
i = 0
while i < 5:
    print(i)
    i += 1

# Output:
# 0
# 1
# 2
# 3
# 4
```
In this example, we initialize a variable i with a value of 0. Then, we use a while loop to print the value of i and increment it by 1 until i is no longer less than 5. This is because the while loop executes the code inside the block as long as the condition i < 5 is true. On each iteration of the loop, the current value of i is printed to the console using the print() function. Then, the value of i is incremented by 1 using the += operator. This process continues until i is equal to 5, at which point the condition i < 5 is false and the loop terminates.


### Lists
In Python, a list is a collection of ordered items enclosed in square brackets. Lists are a fundamental data structure in Python and are used to store and manipulate a collection of related data.

Lists can contain any type of data, including integers, floats, strings, and even other lists. The items in a list are indexed starting from 0, so the first item in the list has an index of 0, the second item has an index of 1, and so on.

Here's an example of how to create a list in Python:

```python
my_list = [1, 2, 3, 4, 5]

print(my_list[0])      # Output: 1
print(my_list[1:3])    # Output: [2, 3]
print(len(my_list))    # Output: 5

my_list.append(6)
print(my_list)         # Output: [1, 2, 3, 4, 5, 6]

my_list.remove(3)
print(my_list)         # Output: [1, 2, 4, 5, 6]

my_list.reverse()
print(my_list)         # Output: [6, 5, 4, 2, 1]
```

In this example, we define a list my_list containing five integers. We then use indexing to access the first element of the list (my_list[0] returns 1) and slicing to access a subset of the list (my_list[1:3] returns [2, 3]).

We also use the len() function to get the length of the list (len(my_list) returns 5).

Next, we use the append() method to add a new element to the end of the list (my_list.append(6)). We then use the remove() method to remove an element from the list (my_list.remove(3) removes the element with the value 3 from the list).

Finally, we use the reverse() method to reverse the order of the elements in the list (my_list.reverse() returns [6, 5, 4, 2, 1]).


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

### Functions
In Python, a function is a block of code that performs a specific task. To define a function, we use the def keyword, followed by the name of the function, and a set of parentheses containing any arguments that the function takes. For example, def my_function(arg1, arg2): defines a function called my_function that takes two arguments.

Functions can return a value using the return statement. The value that is returned by the function can be used by the calling code. If the return statement is omitted, the function will return None.

Functions can also have default arguments and variable-length argument lists. Default arguments are values that are used if no argument is provided for that parameter. Variable-length argument lists allow a function to accept any number of arguments, which can be useful in certain situations.

Here's an example of how to define a simple function in Python:

```python
# Define the square function
def square(x):
    return x ** 2

# Call the square function with an argument of 5 and store the result in a variable
result = square(5)

# Print the result to the console
print(result)

```
In this example, we define the square() function, which takes a single argument x and returns the square of x. The function definition is followed by a call to the square() function with an argument of 5, which returns the value 25. We then store the result in a variable called result and print it to the console.

The square() function has an argument x, which represents the input value that the function will operate on. In this case, x is an integer.

The square() function has a return type of integer, since the return statement in the function body returns an integer value (the square of x). In Python, functions can have any valid data type as their return type, or they can return None if they do not explicitly return a value.


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


### Modules
In Python, a module is a file containing Python code that can be imported into another file. Modules are a fundamental building block of Python programming, allowing us to organize our code into separate files and reuse code across multiple projects.

To import a module into our code, we use the import statement, followed by the name of the module. For example, import math imports the built-in math module, which contains various mathematical functions and constants.

Once a module is imported, we can access its functions and variables using dot notation. For example, math.sqrt(2) calls the sqrt() function from the math module, which computes the square root of 2.

Here's an example of how to use the math module in Python:

```python
import math

# Calculate the square root of 2 using the math module
result = math.sqrt(2)

# Print the result to the console
print(result)

# OUTPUT
# 1.4142135623730951


```
In this example, we import the math module using the import statement. We then call the sqrt() function from the math module with an argument of 2, which computes the square root of 2 and returns the result. Finally, we store the result in a variable called result and print it to the console. 
