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
