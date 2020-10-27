# hello-world
Journal my progress of Python Learning.
I will register my daily learnings, my questions
Review my own knowledge and make small notes to 
Myself. 

**Remember set() will chose the unique Items in a
List [] and iterate over the list returning unique
Values 

Example

mylist = [1,2,2,2,2,4,4,5,5]
set(mylist)
Print [1,2,4,5]

To find out what attributes a type has:

dir(str)
dir(list)
dir(dict)
To find out what Python builtin functions there are:

dir(__builtins__)
Documentation for a Python command can be found with:

help(str)
help(str.replace)
help(dict.values)

Tip: Converting Between Datatypes
Sometimes you might need to convert between different data types in Python for one reason or another. That is very easy to do:

From tuple to list:

>>> data = (1, 2, 3)
>>> list(data)
[1, 2, 3]
From list to tuple:

>>> data = [1, 2, 3]
>>> tuple(data)
(1, 2, 3)
From list to dictionary:

>>> data = [["name", "John"], ["surname", "smith"]]
>>> dict(data)
{'name': 'John', 'surname': 'smith'}
Note that the original data type needs to have the data structured in a way that can be understood by the new data type. For example, the following would not work:

>>> data = [1, 2, 3]
>>> dict(data)
TypeError: cannot convert dictionary update sequence element #0 to a sequence
That's because a dictionary is made of key and value pairs, but the list was not constructed that way, so the above would generate an error.



===================#####FUNCTION

Udemy logo
The Python Mega Course: Build 10 Real World Applications
Your progress
Summary: Functions and Conditionals
In this section, you learned to:

Define a function:

def cube_volume(a):
    return a * a * a
Write a conditional block:

message = "hello there"
 
if "hello" in message:
    print("hi")
else:
    print("I don't understand")
Write a conditional block of multiple conditions:

message = "hello there"
 
if "hello" in message:
    print("hi")
elif "hi" in message:
    print("hi")
elif "hey" in message:
    print("hi")
else:
    print("I don't understand")
Use the and operator to check if both conditions are True at the same time:

x = 1
y = 1
 
if x == 1 and y==1:
    print("Yes")
else:
    print("No")
Output is Yes since both x and y are 1.

Use the or operator to check if at least one condition is True:

x = 1
y = 2
 
if x == 1 or y==2:
    print("Yes")
else:
    print("No")
Output is Yes since x is 1.

Check if a value is of a particular type with:

isinstance("abc", str)
isinstance([1, 2, 3], list)
or

type("abc") == str
type([1, 2, 3]) == lst



======== Inputs =======
Summary: Processing User Input
In this section, you learned that:

A Python program can get user input via the input function:

The input function halts the execution of the program and gets text input from the user:

name = input("Enter your name: ")
The input function converts any input to a string, but you can convert it back to int or float:

experience_months = input("Enter your experience in months: ")
experience_years = int(experience_months) / 12
You can format strings with (works both on Python 2 and 3):

name = "Sim"
experience_years = 1.5
print("Hi %s, you have %s years of experience." % (name, experience_years))
Output: Hi Sim, you have 1.5 years of experience.

You can also format strings with:

name = "Sim"
experience_years = 1.5
print("Hi {}, you have {} years of experience".format(name, experience_years))
Output: Hi Sim, you have 1.5 years of experience.


===========LIST COMP

Summary: List Comprehensions
In this section, you learned that:

A list comprehension is an expression that creates a list by iterating over another container.

A basic list comprehension:

[i*2 for i in [1, 5, 10]]
Output: [2, 10, 20]

List comprehension with if condition:

[i*2 for i in [1, -2, 10] if i>0]
Output: [2, 20]

List comprehension with an if and else condition:

[i*2 if i>0 else 0 for i in [1, -2, 10]]
Output: [2, 0, 20]
