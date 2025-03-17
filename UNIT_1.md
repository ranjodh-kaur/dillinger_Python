_______
# Unit 1 - Lesson 1
____

#### 1.1.1. What is a computer programming language?

- Language is a tool for communication.

In this learning program, we use English to give instructions and share information with learners.
Similarly, computer programming languages communicate with computers by providing instructions.
These Programming languages help us represent data like numbers, text, and images and also provide instructions to work with that data.
You don't need to be a computer science expert or a math genius to write a computer program. If you understand basic logic, you can write computer programs easily.


- Python is an interpreted, high-level programming language for general-purpose programming.

In English, to greet someone, you say "Hello!". Similarly in Spanish, one would say "Hola!".

**For example, if we want the computer to display a greeting message, we provide instructions in a computer programming language.** 

In Python we provide instructions in the below format
```print("Hello!")```

- The above text is called source code or simply code. Since it is written in Python, it is called Python code.
- The above code represents a simple Python program which prints "Hello!".
- In the above case, we have provided some instructions in a computer programming language to the computer to display a greeting message. This sequence of instructions is called a program.

#### 1.1.2. The genesis of Python

The Python programming language was developed in the 1980s by Guido Van Rossum at Centrum Wiskunde & Informatica (CWI) in the Netherlands as a successor to the ABC language (itself inspired by SETL), capable of exception handling and interfacing with the Amoeba operating system.

###### Programming languages can be classified into the below three categories:

1. **Low-level programming languages:** It involves communication with the system in binary format , consisting of 0's and 1's, which can be directly executed. These languages provide instructions that can be used to perform low-level operations such as memory management. An example of such language is Assembly Language.

2. **High-level programming language:** In this, the communication with system occurs in the form of text (usually in English), which is easily readable and understandable by humans. Examples of such Languages include Ada, JavaScript, Python, Ruby etc.

3. **Middle-level programming languages:** These are the languages which support both low-level and high-level features. These are also written in human readable text. They typically use tools like compilers to convert the human readable instructions (high-level language constructs) into low-level executable code (usually in binary format). Eg: C, C++, Java, etc,.

**Python versions:**

- Guido Van Rossum published the first version of Python code (Python 0.9.0) at alt.sources in February 1991. This release included exception handling, functions and the core data types.

- Python 1.0 released in January 1994. It included filters, map, reduce and lambda.

- Python 2.0 released in October 2000. Features include list comprehension and garbage collection with reference cycles.

- Python 3.0 released in December 2008. This release removed duplicate constructs and modules, but it was not backward compatible with previous versions..

Do not panic. The features mentioned above will be discussed in detail in the later sections.

Python can be used for creating computer applications, computer games or even for testing microchips.

#### 1.1.3. Python Program Life Cycle

The instructions (called source code) written in Python programming language can be executed in two modes:

1. **Interactive mode:** In this mode, lines of code are directly written and executed in the Python interpreter shell, which instantaneously provides the results.
2. **Normal or script mode:** In this mode the source code is saved to a file with **.py** extension, and the file is executed by the Python interpreter.

Writing our code in files with a .py ending. This is the practice adopted for building extensive programs in Python.

For example, **calculator.py** is called a Python source file.

The Python program statements have to be entered and saved in a file through a text editor, and then the file has to be executed to produce results.

If there are any errors in Python code then the system will let you know so that you can fix them.

**There are two types of errors:**
1. Syntax errors
2. Runtime errors.

1) Syntax errors are like grammatical errors in English. They occur when the defined rules are not followed.

**For example:**
```` prin("Hello World") ````

The Python interpreter generates the following syntax error as it did not find a name prin (as the correct method name is print).
Traceback (most recent call last):
  File "", line 1, in 
NameError: name 'prin' is not defined
When we change the code to print("Hello World"), the Python interpreter would print the output as follows
```Hello World```


2) Runtime errors occur due to incorrect algorithm/logic or wrong operations like dividing by zero during the program execution.

**For example:**
```
a = 10
b = 0
print(a / b) 
```

The Python interpreter generates the following runtime error indicating that division by zero occurred during execution.

Traceback (most recent call last):
  File " ", line 1, in 
ZeroDivisionError: division by zero

#### 1.1.4. Difference between Compiler and Interpreter

|Compiler|	Interpreter|
|----|-----|
|Compiler takes entire program as input|	Interpreter takes single instruction as input|
|Intermediate object code is generated|	No Intermediate object code is generated|
|Conditional control statements execute faster|	Conditional control statements are slower in execution|
|Memory Requirement is More(Since Object code is generated)|	Memory Requirement is Less|
|Program need not be compiled every time|	Every time higher level program is converted into lower level program|
|Errors are displayed after entire program is checked|	Errors are displayed for every instruction interpreted (if any)|
|Example : C compiler|	Example : Python|

#### 1.1.5. High level language categories

The Programming Languages are divided into following categories:

1. **Interpreted languages:** These languages are executed line by line by an interpreter without prior compilation.
Examples include Python, Ruby, and JavaScript.
2. **Functional languages:** These languages treat functions as important parts and promote a way of programming where functions are used a lot. These are designed on the concept of mathematical functions that use conditional expressions and recursion to perform computation.
Examples include Haskell, Lisp, and Erlang.
3. **Compiled languages:** These languages require compilation before execution. The source code is transformed into machine code or intermediate code.
Examples include C, C++, and Rust.
4. **Procedural languages:** These languages follow a procedural programming paradigm, emphasizing the use of procedures or functions to organize code.
Examples include C, Pascal, and Fortran.
5. **Scripting languages:** These languages are interpreted and used for automating tasks and scripting applications.
Examples include Python, Perl, Ruby, and Bash.
6. **Markup languages:** These languages are used to define and present structured data. They are not traditional programming languages but play a crucial role in data representation.
Examples include HTML, XML, and JSON.
7. **Concurrency-Oriented languages:** These languages are designed to handle multiple tasks at the same time, working together.
Examples include Go (Golang) and Erlang.
8. **Object-Oriented languages:** These languages support object-oriented programming (OOP) concepts like classes, objects, inheritance, and polymorphism.
Examples include Java, C++, C#, and Python.

#### 1.1.6. Identify the Error

The code in the editor has a syntax error.

Find and fix the error and click on Submit.

Note: If you are unable to find the error, click on Submit to see the error message.
````prnt("Python is Easy")````
**Source code:**
````print("Python is Easy")````

#### 1.1.7. Identify the Error

The below code in the editor has a syntax error.

Fix the error and Submit.

Note: If you are unable to find the error, click on Submit to see the error message.
````     Print("Python is not Typhoon")                  ````
**Source code:**
````print("Python is not Typhoon")````

#### 1.1.8. Other usages of print function

Here are a few interesting ways in which the print() function works.

 1. **With comma (,) as a separator:** When two or more strings are given as parameters to a print(...) function with a comma (,) as a separator, the strings are appended with a space and printed.
 **For example:**
````print("I", "Love", "Python")````
````will generate the output as````
````I Love Python````

2. **With space as a separator:** When two or more strings are given as parameters to a print(...) function with space as a separator, the strings are appended without a space between them.
**For example:**
```print("I"   "Love"   "Python")```
```will generate the output as```
```ILovePython```
 
3. **With repeat character ( * ) :** We can print a string n times by using the repeat character (*) as shown below:
````print("ABC" * 3);````
will generate the output as
````ABCABCABC````

**Write code to print the magic word Abracadabra, n times, using the repeat character ( * ).**
In the given code, we are taking input from the user. We will learn more about input statements in the upcoming lessons.
```python
n = int(input())
print("Abracadabra"*n)
# write your code here to print the given word n times
```

#### 1.1.9. Fill in the missing code

The print statement in the below code is supposed to generate the following output:
````where there is a will, there is a way````
add or remove commas (,) accordingly to achieve the desired output.
````print("wh", "ere" "the", "re" "is" "a" "will," "th","ere", "is" "a", "way")````
**Source Code:**
````python
print("wh" "ere" ,"the" "re", "is" ,"a", "will,", "th""ere", "is", "a", "way")
````

#### 1.1.10. Features of Python

Features of Python Programming Language

1. **Simple:** Python is a simple and minimalistic language. Reading a good Python program feels almost like reading English, although very strict English! This pseudocode nature of Python is one of its greatest strengths. It allows one to concentrate on the solution to the problem rather than the language itself.

2. **Easy to Learn:** Python has a very simple syntax, which means it is very easy to learn and code.

3. **Free and Open Source:** Most Linux operating systems have Python by default. The standard modules and the Python interpreter are free.
4. **High-level Language:** When one writes programs in Python, one need not bother about the low-level details such as managing the memory (allocation & deallocation) as the language has a built-in garbage collector.
5. **Interpreted:** Meaning, a Python program need not be compiled like programs in C and Java languages, Python programs can be directly executed from their source code using a Python interpreter.
6. **Portable:** Python interpreter exists for almost all platforms/operating systems. Python programs can execute on any platform like Windows, Linux, etc., without requiring any change, as long as there is a Python interpreter. Internally, Python interpreter converts the source code into an intermediate form called byte code, translates this into the native language of the computer, and then runs it. This is what makes a Python program portable. A Python program copied to another operating system works because of the Python interpreter present on that operating system.
7. **Object Oriented:** Python supports procedure-oriented programming as well as object-oriented programming.
8. **Extensible:** If one needs a critical piece of code or an algorithm to run very fast, one can code that part of the program in C or C++ and then use or execute it from inside a Python program.
9. **Embeddable :** Similarly, one can embed Python within a C or C++ program.
10. **Extensive Libraries:** The Python Standard Library is a very exhaustive library for regular expressions, documentation generation, unit testing, threading, databases, web browsers, CGI, FTP, Email, XML(Extensible Markup Language), XML-RPC, HTML, WAV files, cryptography, GUI (graphical user interfaces), and other OS-related operations.
________

# Unit 1 - Lesson 2
_________
#### Types of Errors

#### 2.1.1. Syntax Error

An error in programming is generally a bug in the code introduced by the developer. There are generally three types of errors Syntax, Logical, and Runtime. To correct these known errors, exception-handling mechanisms are used.

Let's understand about Syntax Errors: These errors are mistakes that happen when there is an incorrect format in the code. These programs are not executed as the compiler of the program raises the errors that need to be corrected. Compiler identifies the line of error and provides an error message.

**Common Python syntax errors are:**
1. Missing a required keyword.
2. Missing symbol, such as a colon or comma.
3. Misspelling a keyword.
4. Wrong indentation.

#### 2.1.2. Logical Errors

**Logical Errors:** These are also known as semantic errors and are tough to identify. These errors occur when a program compiles and runs but doesn’t produce the expected output. They are often due to incorrect logic or misuse of a language’s syntax.

**Common Python logical errors are:**
1. Usage of the wrong variable name.
2. Indentation of a block to the wrong level.
3. A boolean logic gone wrong.
4. Integer division instead of floating-point division.
5. Working on operator precedence in a wrong way.

#### 2.1.3. RunTime Errors
**Runtime errors:**

These errors occur during the execution of a program after it has been successfully compiled or interpreted. These errors are not detected during the compilation or interpretation phase because they depend on specific conditions that occur during the program’s execution.
When a runtime error occurs, the program “crashes,” or stops running. This is because the program has encountered a condition it was not equipped to handle (like division by zero or an operation on incompatible types).


**Some common Python runtime errors include:**

1. ZeroDivisionError: Occurs when you try to divide by zero.
2. TypeError: Occurs when an operation is applied to an object of an inappropriate type.
3. IndexError, KeyError, AttributeError: Occurs when you try to access a list element, dictionary value, or object attribute that doesn’t exist.
4. FileNotFoundError: Occurs when trying to open a file that doesn’t exist.

_______
# Unit 1 - Lesson 3
________
#### 3.1.1. Understanding Python Comments

A computer program is a collection of instructions or statements.

A Python program is usually composed of multiple statements. Each statement is composed of one or a combination of the following:
- Comments
- Whitespace characters
- Tokens

**Comments :** In a computer program, a comment is used to mark a section of code as non-executable.
- Comments can be used to explain Python code, so one can understand the code better.
- Comments can be used to prevent execution when testing code.

**In Python, there are two types of comments:**
- Single-line comments: These start with a # symbol, and everything after it on the same line is treated as a comment.
- Docstring comment: These are enclosed in triple quotes ((''') or (""")). We'll learn more about these later.

Below code example demonstrates the usage of comments.
````python
riverName1 = "Ganga" # A comment can follow after a line of code.
					 # Above one is called an inline-comment.

riverName3 = "Nile#Long" #"#" is part of the text and does not start a comment
````
Below are a few important points regarding comments:
1. The # character must be specified at the beginning of a comment line.
2. Python style guide suggests that each line of a block comment starts with a # and a single space.
3. Comments do not nest. Meaning # has no special meaning inside a comment line that starts with #.
4. One cannot write comments inside string literals which are enclosed between single-quotes or double-quotes. The # character inside a string literal is treated as part of the string's content.
5. In a comment anything written after # in a particular line is ignored by the interpreter. Meaning it does not form part of the executable code in the program.

**Make the following changes in the code given:**
- Remove the comment on the line which prints "I am a Python Guru"
- Add a comment on the line which prints "Python is not cool"
````python
# This is my first program
# print("I am a Python Guru")
print("Python is not cool")
# print() is used to print the message on console
````

**Source code:**
````python
# This is my first program
print("I am a Python Guru")
# print("Python is not cool")
# print() is used to print the message on console
````

#### 3.1.2. Problem Solving in Comments

Comment and uncomment appropriate lines of code so that the given program prints only odd numbers.
````python
# print("1")
# print("2")
# print("3")
# print("4")
print("5")
print("6")
print("7")
print("8")
print("9")
# print("10")
# print("11")
# print("12")
# print("13")
````

**Source code:**
````python
print("1")
# print("2")
print("3")
# print("4")
print("5")
#print("6")
print("7")
#print("8")
print("9")
# print("10")
print("11")
# print("12")
print("13")
````

#### 3.1.3. Understanding Docstring in Python

**Docstrings:**
- Python has a way to specify documentation comments known as docstrings.
- A docstring is a simple text, usually in English, placed in your code to explain what a specific part of the code does.
- A docstring is a text enclosed in triple quotes, and it's usually the first non-comment statement in a module, function, class, or method definition.
- This docstring becomes a special attribute called __doc__ for that object.
- Python allows the use of both """triple-double-quotes""" or '''triple-single-quotes''' to create docstrings. However, the Python coding conventions specification recommends us to use """triple-double-quotes""" for consistency.
- The main purpose of docstrings in Python is to provide information on what a particular Python object does and not how it does.
- According to the Python coding conventions, the docstring should always begin with a capital letter and end with a period (.)

**There are two types of docstrings:**
1. **One-line docstring:** Provides information what an object does in a single line.
2. **Multi-line docstring:** Provides information what an object does in multiple lines.

An example of a one-line docstring is as follows :
````python
def add(a, b): 
	"""Return the sum of given arguments."""
	return a + b
````

An example of a multi-line docstring is as follows :

````python
def gcd(a, b):
	"""Return gcd of the given arguments.

	a -- blah blah blah
	b -- blah blah blah blah
	"""
````

Syntax for extracting the docstring in script mode is :
````print(object_name.__doc__)````

- The docstring of any object can be extracted using __doc__ attribute on that object
- If an object does not have a docstring, then the object.__doc__ results in None.
- None is a reserved word (keyword) in Python used to define a null value or no value at all.

Examples:
````python
def add(a, b): 
	"""Return the sum of given arguments."""
	return a + b
print(add.__doc__)

output:
Return the sum of given arguments.
````
````python
def add(a, b): 
	return a + b 

print(add.__doc__)

output:
None
````

**Write the print statements in the code editor to print the one-line docstring for add() method and the multi-line docstring of power() method.**

````python
def add(a, b):
	"""Return sum of given arguments."""
	return a + b

def power(b, e):
	"""Return the power value.
	
	b -- is the base
	e -- is the exponent
	"""
	return b ** e

print(add.__doc__)# print docstring of add method

print(power.__doc__)# print docstring of power method
````

#### 3.2.1. Understanding Identifiers in Python

**Identifiers:**

- An identifier is a name used to identify a variable, function, class, module, or object.
- Identifier helps in differentiating one entity from the other.
- Python is a case-sensitive programming language. Meaning, Age and age are two different identifiers in Python.

**Let us consider an example:**
````python
Name = "codeTantra1"
name = "CodeTantra2"
````
Here the identifiers Name and name are different, because of the difference in their case.

**Rules for writing identifiers:**

- Identifiers can be a combination of lowercase letters (a to z) or uppercase letters (A to Z) or digits (0 to 9) or an underscore ( _ ).
- Examples: myClass, var_1, print_this_to_screen, _number etc..
- An identifier can start with an alphabet or an underscore (_), but not with a digit.
- 1_variable is invalid, but variable_1 is perfectly fine.
- Keywords cannot be used as identifiers. (Keywords are reserved words in Python which have a special meaning, Keywords in Python will be explained later.)
**Examples: def, and, not, for, while, if, else and so on.**
- Special symbols like !, @, #, $, % etc. are not allowed in identifiers. Only one special symbol underscore (_) is allowed.
**company#name, $name, email@id are invalid Python identifiers.**
- Identifiers can be of any length.

**Naming conventions for Python identifiers :**
- Class names start with an uppercase letter. All other identifiers start with a lowercase letter.
- Starting an identifier with a single leading underscore (_) indicates that the identifier is private.
- Starting an identifier with two leading underscores (__) indicates that the identifier is strongly private.
- If an identifier begins with two leading underscores (__) and also ends with two trailing underscores (__), then it indicates that the identifier is a language-defined special name. For example, Docstrings become __doc__ - a special attribute of an object.

##### 3.2.2. Understanding Python Keywords

Every programming language usually has a set of words known as keywords.

These are reserved words with special meaning and purpose. They are used only for the intended purpose.

**Note:** We cannot use a keyword as a variable name, function name, or as any other identifier name.
Python also has its own set of reserved words called keywords.

The interpreter uses the keywords to recognize the structure of the program.

Python 2 has 32 keywords while Python 3.5 has 33 keywords. An extra keyword called nonlocal was added in Python 3.5.

**Note:** Python 3.5 introduced async and await as context-dependent keywords, and their usage as identifiers was deprecated. In Python 3.7 async and await were added as keywords, resulting in a total of 35 keywords in Python 3.7.

**The 33 keywords are as follows:**
|   |   |    |   |   |
|---|---|---|---|--|
|False	|	class	|	finally	|	is	|		return|
|None	|	continue|	for		|	lambda	|	try|
|True	|	def		|	from	|	nonlocal|	while|
|and		|	del		|	global	|	not		|	with|
|as		|	elif	|	if		|	or		|	yield|
|assert 	|	else	|	import	 |	pass|
|break	|	except	|	in	|		raise	|	


Python provides a way to print the list of keywords in its current version.
````python
import keyword	 		# This statement is used to import the keyword module.
print(keyword.kwlist)	# kwlist contains all the keywords of Python
````
The output of the above program is:
````python
['False', 'None', 'True', 'and', 'as', 'assert', 'break', 'class', 'continue', 'def', 'del', 'elif', 'else', 'except', 'finally', 'for', 'from', 'global', 'if', 'import', 'in', 'is', 'lambda', 'nonlocal', 'not', 'or', 'pass', 'raise', 'return', 'try', 'while', 'with', 'yield']
````

To check whether a given word is a Python keyword or not, we use a built-in function iskeyword(). This function returns a boolean value, if the given word is a keyword then it returns True as output otherwise returns False.

#### 3.2.3. Fill in the missing code

Fill in the missing code in the below program to print whether the given words - exec, nonlocal and False are keywords or not in Python .

Hint: See how the word and is verified to be a keyword or not.

````python
import keyword
print('and is a keyword :', keyword.iskeyword('and'))

#Fill in the missing code in the below lines
print('exec is a keyword :',keyword.iskeyword('exec') )
print('nonlocal is a keyword :',keyword.iskeyword('nonlocal') )
print('False is a keyword :',keyword.iskeyword('False') )
````

_________
# Unit 1 - Lesson 4
_______
##### 4.1.1. Understanding Variables

**Variables in Python:**
- In Python, a variable is a reserved memory location used to store values.
- Python being a dynamically typed language, there is no need to declare variables or declare their types before using them.
- Python has no command for declaring a variable. A variable is created the moment a value is assigned to it.
- The equal-to (=) operator is used to assign value to a variable.

**Note:** Operators are special symbols used in programming languages that represent particular actions. = is called the assignment operator.

**For example :**
````python
marks = 100 # Here marks is the variable and 100 is the value assigned to it.
````

**Note:** As a good programming practice, we should use meaningful names for variables.

- Python interpreter automatically determines the type of the data, based on the data assigned to it.
- In Python, we can even change the type of the variable after it has been set once (or initialized with some other type). This can be done by assigning a value of a different type to the variable.
- A variable in Python can hold any type of value like 12 (integer), 560.09 (float), "CodeTantra" (string) etc.


The code given below shows how values of multiple types can be assigned to a single variable.
````python
# In the below line, current time is represented as the number of milliseconds since 1 January 1970 00:00:00
currentTime = 1548594278157	

# In the below line, the same variable currentTime is being re-assigned the time in the form of a String (text)
currentTime = "Sun Jan 27 2019 18:35:36 GMT+0530 (India Standard Time)"
````

**Note:** At any given point of time, a variable can hold only one value.

**Fill in the missing code as per the instructions given in the comments.**
````python
# In the below line, assign value 18 to the length variable
length = 18
# In the below line, assign value "King Cobra" to the snake variable
snake = "King Cobra"
print(snake, "can grow up to a length of", length, "feet")
````
##### 4.1.2. Assigning Different Values to Variables

Associating a value with a variable using the assignment operator (=) is called as binding.

In Python, when you assign a value to a variable, you're actually creating a reference to that value, not making a copy.

Python uses reference semantics, which means that variables essentially point to objects rather than containing the objects themselves.

We cannot use Python variables without assigning any value.

If we try to use a variable without assigning any value then, the Python interpreter shows an error saying "name is not defined".

**Fill the missing code in the given program as per the below instructions:**
1. Assign the variable value1 with value 99
2. Assign the variable value2 with string value "Hello Python"
3. Assign the variable value3 with string value "Hello World"
then print the variables in the same order.

**Expected Output:**
````
Hello
Hello
Hello
99
Hello Python
Hello World
````
**Source code:**
````python
value1 = value2 = value3 = "Hello"
print(value1)
print(value2)
print(value3)
# Assign values to variables and print again
value1 = 99
value2 = "Hello Python"
value3 = "Hello World"
print(value1)
print(value2)
print(value3)
````

##### 4.1.3. Assignment of Variables

Python variables do not need explicit declaration to reserve memory space.

The declaration happens automatically when you assign a value to a variable.

The equals to sign (=) is used to assign values to variables.

The operand to the left of the = operator is the name of the variable and the operand (or expression) to the right of the = operator is the value stored in the variable.

**Let us consider the below example:**
````python
counter = 100 # An integer assignment 
print(counter) # Prints 100
miles = 1000.50 # A floating point assignment
print(miles) # Prints 1000.5
name = "John" # A string assignment
print(name) # Prints John
````

In the above example 100, 1000.50, and "John" are the values assigned to the variables counter, miles, and name respectively.

The above example program produces the result as:
````
100
1000.5
John
````

**Complete the given code in which :**

- A variable kilometers is created and you need to assign an integer value to it.
- A variable convertfactor is created and 0.621371 is assigned to it.
- Calculate the product of kilometers and convertfactor and assign it to miles variable which is already created.
- Print the value of miles as Miles: miles where miles is the calculated value.
````
Sample Input: Enter·a·value:·6
Expected Output:
Miles:·3.7282260000000003
````
**Source code:**
````python
kilometers = int(input("Enter a value: ")) # assign the correct value
convertfactor = 0.621371 # assign the correct value

miles =  (kilometers) * (convertfactor)# multiply kilometers and convertfactor

print("Miles:",  miles )

````

##### 4.1.4. Understanding Multiple Assignment

Python allows you to assign a single value to several variables simultaneously.

Let us consider an example:
````number1 = number2 = number3 = 100````
Here an integer object is created with the value 100, and all the three variables are references to the same memory location. This is called chained assignment.

We can also assign multiple objects to multiple variables, this is called multiple assignment.

Let us consider the below example:
````value1, value2, value3 = 1, 2.5, "Ram"````
Here the integer object with value 1 is assigned to variable value1, the float object with value 2.5 is assigned to variable value2 and the string object with the value "Ram" is assigned to the variable value3.

**Fill in the missing code in the given program to assign the integer value 25 to the variable named age, float value 24.789 to the variable named length and the string value "Python" to the variable named language using multiple assignment syntax so that their individual values are printed by the existing code.**

````
Expected Output:
999
24.789
Python
````

**Source code:**
````python
age,length,language =25,24.789,"Python"  # Assign the values to the variables
print(age)
print(length)
print(language)
````

##### 4.1.5. Chained Assignment

In Python, assignment statements do not return a value. Chained assignment is recognised and supported as a special case of the assignment statement.

````a = b = c = x```` is called a chained assignment in which the value of x is assigned to multiple variables a, b, and c.

Let us consider a simple example:
````python
a = b = c = d = 10
print(a) # will print result as 10
print(b) # will print result as 10
print(c) # will print result as 10
print(d) # will print result as 10
````
Here, we are initializing the variables a, b, c, d with value 10.

**Write a program to assign a user given value to a, b, c variables.**

**Note:** Let us assume that input() is used to read values given by the user. We will learn about input() in later sections.
Here,
````a = b = c = str1````
Sample Input and Output:
````
Enter a value: Hello Python
Value of a: Hello Python
Value of b: Hello Python
Value of c: Hello Python
````
**Source Code:**
````python
str1 = input("Enter a value: ")
a=b=c=str1
# Assign str1 to three objects a, b and c

print("Value of a:", a) # Print a
print("Value of b:",  b ) # Print b
print("Value of c:",  c ) # Print c
````

_________
# Unit 1 - Lesson 5
_______
#### 5.1.1. Understanding Expressions

An expression is a combination of values(Constants), variables and operators.

An expression may also include call to functions and objects. We will learn about functions and objects in the later sections.

Operators are symbols that represent particular actions. Operands participate in the action performed by the operator.

Some of the arithmetic operators present in Python are :
Operator 	Meaning 					Expression 		Value
+			Arithmetic addition			10+20			30	(addition of 10 and 20)
-			Arithmetic subtraction		40-20			20	(subtraction of 20 from 40)
*			Arithmetic Multiplication	5*4				20	(multiplication of 5 and 4)
/			Arithmetic Division			8/4				2	(quotient when 8 is divided by 4)
%			Modulus (Remainder)			5%3				2	(remainder when 5 is divided by 3) 
More operators will be discussed in the later sections.
Any expression evaluates to a single value, which becomes the value of the expression.

Instructions that a Python interpreter can execute are called statements. For example, a = 1 is an assignment statement.

In the example given below a + b is an expression and the print() function prints the resultant value which is 20.

Example1
a = 10 # This is an assignment statement
b = 10 # This is an assignment statement
print(a + b) # a + b is an expression and print(a + b) is a statement

Example2:
b = 10 # This is an assignment statement
c = 10 # This is an assignment statement
a = b * 5 + c # b * 5 + c is an expression, we are assigning this expression to the variable a then a = b * 5 + c is an assignment statement 
print(a)

Note : In the above example we have used simple arithmetic operators like + and * which performs arithmetic addition and multiplication respectively. The operator + works as a concatenation operator if the operands are strings(text).
Understand and fill the missing code given, to know about expressions and statements.

````python
number1 = 20.50
number2 = 38.25
# Print the multiplication of number1 and number2 using * operator.
print(number1*number2)
string1 = "Amazon"
string2 = "River"
# Print the concatenated value of string1 and string2 using + operator.
print(string1+string2)
````

#### 5.1.2. Understanding Statements - Print statements
02:27
A statement in Python is a logical instruction which can be read and executed by Python interpreter.

In Python, we have different kinds of statements :
Print statements
Assignment statements
Selective statements
Iterative statements
Control Flow statements
Function declaration statements
The purpose of Python's assignment statement is to associate variables with values in your program.

It is the only statement that does not start with a keyword.

An assignment statement contains atleast one equal sign (=), to the left hand side of = we have a variable and to the right hand side we have an expression.

The general form of an assignment statement is as follows :
target0 = target1 = ... = expression

Here target0, target1, target2 ... are variables and Python will evaluate the expression to a single value and that single value is assigned to the variables. 
This association of a value to a variable is called as binding. 
For example, Let us consider the following code:
a = 15
print(a)
Here, a = 15 is a simple assignment statement and print(a) is a print statement used to display the value of a.

5.1.3. Types of Assignment Statements
01:26
There are two types of assignment statements in Python. They are:

1. Basic assignment statements
2. Augmented assignment statements

The simple syntax for a basic assignment statement is:
variable_name = expression

In the example given below we are assigning a string value "CodeTantra" to a variable called name.
name  =  "CodeTantra"

Fill the missing code in the given editor follow the instructions given below.
Create a variable message and assign "Welcome to Python" to it.
Print the variable message.
Create a variable number which is taking input from the user
Add 5 to the variable number by using number = number + 5.
Print the variable number.

````python
message = "Welcome to Python" 
print(message) # print message
number = int(input())
number=number+5 # add 5 to the number
print(number) # print number
````

5.1.4. Augmented Assignment Statement
01:17
Augmented assignment is a combination of an arithmetic or a binary operation and an assignment operation in a single statement.

We can combine arithmetic operators in assignments to form an augmented assignment statement.

The combined operations of the augmented assignments are represented using the following operators : +=, -=, *=, /=, %=

Let us consider a simple example:
a += b
The above statement is a shorthand for the below simple statement.

a = a + b
In augmented assignment statements, the left-hand side is evaluated before the right-hand side

Let us discuss with a simple example:
a += b
Here the left-hand side i.e. a is evaluated first, then value of b is evaluated and then addition is performed, and finally the addition result is written back to a.

An augmented assignment expression like
x += 1
can be rewritten as
x = x + 1
Both the above statements give out similar result, but the effect is slightly different.

In the augmented version, the value of x is evaluated only once. Furthermore, whenever feasible, the actual operation takes place in the existing memory location of x, without creating a new memory space and then assigning it to the target variable.


5.2.1. What is an Indentation
01:28
Python utilizes white spaces to define control flow blocks. This concept is inherited from its predecessor, ABC. Instead of relying on punctuation or keywords, Python uses indentation to signify the scope of a block of code.

The first line of the function definition is called the header, the rest is called the body.

The header has to end with a colon (:) and the body has to be indented.

By convention, the indentation is always four spaces or one Tab space.

The body can contain any number of statements.

Interpreter returns Indentation Error when we are not providing correct Indentation.

Let us see the Indentation with Example:

Indentation in Python:

if(i == 10):  # Indentation started with :
	print("i is 10") # this print statement is in if block(providing tab space at front of print statement)
else: # else is in out of if block
	print("i is not 10") #print statement is in else block
Follow the instructions given in comment lines in the program and complete the code to understand the Indentation in python.

Expected Output:
Small Value: 10.0

````python
# add the proper indentation to the print statements
if 100.0 > 10.0:
	print("Small Value:", 10.0)
else:
	print("Large Value:", 100.0)
````

5.2.2. A simple program in Python
01:04
We can run a Python program in two ways. They are:

Interactive mode
Scripting mode
1. Interactive mode

Interactive mode in Python offers a command-line environment that provides instant feedback for every statement. It also retains the memory of previously entered statements, allowing them to remain active.
With each new line of code entered, the interpreter evaluates both the partial code and the entire fed program.
Interactive mode is particularly useful for swiftly and conveniently executing individual lines or chunks of code. It's a handy platform for experimentation, trying out different syntax variations, and quickly testing ideas.
Furthermore, debugging becomes straightforward within the interactive mode environment.

To start interactive mode on Ubuntu/Linux/macOS, open the terminal and type the following :
python
To start interactive mode on Windows, open the command prompt and type the following :
c:\python33>python
To start interactive mode of a particular version of python in windows, open the command prompt and type the following :
c:\python33>py -N   N can be 1 or 2 or 3.
Invoking the python interpreter in the interactive mode brings up the prompt like as follows:

some information about the python version 
>>>
The >>> is Python's way of telling you that you are in interactive mode and is ready to execute Python statements.
>>> print("Python is fun")
Python is fun
2. Scripting mode

To execute a Python program in the scripting mode, the following steps are to be followed:
Write group of Python statements in any one of the editor like: Notepad, Notepad++, editplus, nano, gedit, IDLE.
Create and save the file with extension of “.py” or “.pyw”
If script.py is the file that contains the Python statements, then to start scripting mode in Ubuntu/Linux/macOS, open the terminal and type the following :

$python script.py  
If script.py is the file that contains the Python statements, then to start scripting mode in windows, open the command prompt and type the following :

c:\python33>python script.py 
or 
c:\python33>py script.py 
Invoking the interpreter with a script parameter begins execution of the script and continues until the script is finished. When the script is finished, the interpreter is no longer active.

Click on the  button to know different modes of execution in Python.

Change the text in the code given to make the program print "Hello Python" instead of "Hello Basic".

Expected Output:
Hello Python

````python
print("Hello Python")
````

______
# Unit 1 - Lesson 6
_______


