COURSE LEARNINGS:

- Basic programming concepts in python
- Writing effective Python code
- Working with strings and lists
- Putting Python into practice

**My code notes:** [https://www.online-python.com/j15qrEvlYx](https://www.online-python.com/j15qrEvlYx)

**Update daily.**

**Programming**: Used to create a spesific set of instructions for a computer to excecute tasks

**Automation**: The use of technology to reduce human and manual effort to preform common and repetitive tasks

Advantages of Python

- Resembles human language
- Less code
- Easy to read
- Standard guidelines
- Online support
- Built-in code

**Comment**: A note programmers make about the intentation behind their code

**`print()`**: Outputs a specified object to the screen

Syntax: The rules that determine what is correctly structured in a computing language

**Data type**: Category for a particular type of data item

**Float data**: Data consisting of a number with decimal point

**Integer data**: Data consisting of a number that does not include a decimal point

**Boolean data**: Data that can only be one of two values; either true or false

**List data**: Data structure that consists of a collection of data in sequential form

**Variable**: A container that stores data

Ex: `device_id = “h32rb17”`

`type()`: Returns the data type of its input

**Type error**: An error that results from using the wrong data type

Conditional statement: A statement that evaluates soda to determine if it meets a specified set of conditions

`if`: starts conditional statement

Operators

- `>`:
- `<`:
- `>=`:
- `<=`:
- `==`: Evaluates whether two objects match (equal)
- `!=`: Evaluates whether two objects are different (not equal)

`else`: Precedes a code section that only evaluate when all condition that precede it within the conditional ststement evaluate to `False`

**Iterative statement**: Code that repeatedly executes a set of instructions (also refered to as loops)

Ex: `for i in [1, 2, 3, 4]:`

`print (i)`

`for`: signals the beginning of a `for` loop

**Loop variable**: A variable that is used to control the iterations of a loops

`range()`: Generates a sequence of numbers

Ex: `range(0,10)` will generate “0, 1, 2, 3, 4, 5, 6, 7, 8, 9”

**Note: when a start isnt given (0,), it will automatically be set to 0**

**Iterative statement**: Code that repeatedly executes a set of instructions 

**Note:** `while` **loops still repeatedly execute, but this repitition is based on a condition**

`while`: Signals the beggining of a `while` loop

**Function**: A section of code that can be reused in a program

**Built-in functions**: Functions that exist within Python and can be called directly

**User-defined functions**: Function that programmers design for their specific needs

`def`: placed before a function name to define a function

**Parameter (Python)**: An object that is in a function definition for use in that function

**Argument (Python)**: The data brought into a function when it is called

**Return statement**: A Python statement that executes inside a function and sends information back to the function call

`return`: Used to return information from a function

**NOTE: You can also combine functions.** 

**Ex: `print(type(”Hello World!”))`**

`max()`: Returns the largest numeric input passed into it

`sorted()`: Sorts the components of a list

**Library**: A collection of modules that provide code users can access in their programs

Python Standard Library Modules

- re
- csv
- glob
- os
- time
- dateline

**Style guide**: A manual that informs the writing, formatting, and design of documents

**PEP (Python Enhancement Proposals) 8 style guide**: A resource that provides stylistic guidelines for programmers working in python

**Comment**: A not programmers make about the intentions behind their code

**Indentation**: Space added to the beginning of a line of code

`len()`: Returns the number of elements in an object

**String concatenation**: The process of joining two strings together

**Method**: A function that belongs to a specific data type

`.upper()`: Returns a copy of the string in all uppercase letters

`.lower()`: Returns a copy of the string in all lowercase letters

The upper and lower are used like this: `print("Hello".upper())`, you just replace upper with lower

**Index**: A number assigned to every element in a sequence that indicates its position

An index starts from the first character being one and the second being two and so on

`print("HELLO"[1])` would bring the result “E”
`print("HELLO"[1:4])` would extract and show the result “ELL”

`.index()`: Finds the FIRST occurrence of an input in a string and returns its location

**Immutable**: Cannot be changed after it is created and assigned a value

**List concatenation**: Combining two lists into one by placing the elements of the second list directly after the elements of the first list

`.insert()`: Adds an element in a specific position inside a list

`.remove`: Removes the first occurrence of a specific element in a list

Algorithm: A set of rules that solve a problem

**Regular expression (regex)**: A sequence of characters that forms a pattern

`+`: Represents one or more occurrences of a specific character

EX: a+ would have the result “a”, “aaa”, or any number of as in a row. 

If you were given a list saying “a37rz87”, “io2aap4”, “32rb5a2”, “9aaa9595y” you would be given the result [”a”, ”aa”, ”a”, ”aaa”]

`\w`: Matches with any alphanumerical character, but it doesn't match symbols

EX: these are some examples of what some results would be “1”, “k”, “i”

**\w+ is a combination that would give you an alphanumerical string of any length**

So, to find an email like username@email1com it would be \w+ @ \w+\. \w+

`re.findall()`: Returns a list of matches to a regular expression

`with`: Handles errors and manages external resources

EX: This code would take a file of names and separate them and make them usable for code

`with open("login_attempts.txt", "r") as file:
file_text = file_read()
print(file_text.split())
usernames = file_text.split()`

`open()`: Opens a file win python

`.read()`: Converts files into strings

**Parsing**: The process of converting data into a more readable format

`.split()`: Converts a string into a list

![Screenshot 2024-05-28 132627.png](Screenshot_2024-05-28_132627.png)
