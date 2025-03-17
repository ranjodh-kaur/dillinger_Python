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

#### 6.1.1. Understanding Types of Data Types

Computer programming is all about processing data. In computer programming, the data is always represented in the binary form (0's and 1's), i.e. groups of Bits called as Bytes.

In the real world, we come across different types of data like age of a person(integer), number of rooms in a house (integer), price(floating-point number), height (floating-point number), Names of people, places and things (strings), inventory list (list) etc.

Data types categorize data for efficient processing in Python and all programming languages. They assign specific characteristics to data, enhancing accuracy and control in operations.

The data type of the data determines :
 possible values it can be assigned.
 possible operations that can be performed. (Arithmetic operations can be applied on numeric data and not strings)
 the format in which it is stored in the memory.
 the amount of memory allocated to store the data.

Some of the built-in data types supported in Python are:
Number
String
List
Tuple
Set
Dictionary

In Python, each value possesses a data type. A variable in Python is capable of holding a value of any data type.

The same variable in Python can refer to data of different data types at different times. Thus, variables in Python are not strongly typed, implying that you don't have to explicitly declare the data type of a variable when creating it.

Let us consider an example:

a = 5 # variable a now refers to Integer data type
a = 90.45 # variable a now refers to Float data type
a = "India"  # variable a now refers to String data type
a = [5, 90.45, "India"]  # variable a now refers to List data type

We use the built-in function type() to determine the type of data that a variable is referring to at any given point in time.

The syntax of the type() function is as follows :
type(variable_name)
returns the data type of variable_name
Variable Assignment		 	Output of print(type(a))
a = 345					<class, 'int'>
a = 34.56				<class, 'float'>
a = "India"				<class, 'str'>
a = [5, 90.45, "India"]			<class, 'list'>


6.2.1. Numbers
01:59
Numbers

We have three different categories of numbers in Python. They are :
int
float
complex

1.int:
It stands for integer. This Python data type stores signed integers.
In Python an integer can be of any length, with the only limitation being the available memory.

Example 1:
# type() function finds the class the variable belongs.
a = -7
print(type(a)) # will print output as follows
<class 'int'>
Example 2:
a = 12536984596965565656236534754587821564
print(type(a)) # will print output as follows
<class 'int'>

2.float:
It stands for floating-point numbers. This Python data type stores floating-point real values.
For example : An int can only store the number 20, but float can also store numbers with decimal fractions like 20.25.

Example:
a = 3.0 
print(type(a)) # will print output as follows
<class 'float'>

3.complex:
It stands for complex numbers. A complex number is a combination of a real number and an imaginary number.
It takes the form of a + bj Here, a is the real part and b*j is the imaginary part.

Example
a = 2 + 3j # It is important to note that there should not be any space between 3 and j
print(type(a)) # will print output as follows
<class 'complex'>
Write the missing code in the given program to know which class the given variable a belongs to.

````python
a = 365
print(type(a))#Print type of a

a = 345.65
print(type(a))#Print type of a


a = 45 + 5j
print(type(a))#Print type of a
````

6.3.1. String data type
01:01
In Python, a string is a sequence of characters enclosed inside a pair of single quotes(‘) or double quotes(“). Even triple quotes (''') are used to represent multi-line strings.

The computer doesn’t see letters at all. Every letter you use is represented by a number in memory.

For example, the letter A is actually the number 65. This is called encoding. There are two types of encoding for characters – ASCII and Unicode.

ASCII uses 8 bits for encoding whereas Unicode uses 32 bits. Python uses Unicode for character representation.

An individual character within a string is accessed using an index.

Index starts from 0 to n-1, where n is the number of characters in the string.

Python allows negative indexing in strings. The index of -1 refers to the last item in the string, -2 refers to the second last item and so on.



In Python, a string of length 1 is treated as a character.

Ways of creating strings in Python are:

1. Using single quotes (' ')

str = 'Welcome To Python World'
print(str)# will print output as follows  

Output :
Welcome To Python World
If single quote (') is part of the string, then the characters of the string are enclosed between double quotes(").

sentence =  "Welcome to Python's world"
print (sentence) # will print output as follows

Output :
Welcome to Python's world
If single quote (') is part of the string, and the characters are enclosed between single quotes, then a backslash (\) should be added before (') of the string.

The other way of having a single quote in the string content and enclosing the string within single quotes is using a backslash(\)
sentence =  'Welcome to Python\'s world' # observe a backslash (\) before (')
print (sentence) # will print output as follows

Output :
Welcome to Python's world
2. Using double quotes (" ")

str = "Welcome to the world of Python"
print(str) # will print output as follows

Output:
Welcome to the world of Python
3. Using triple double quotes(""" """)

We use triple double quotes(""" """) to create multi-line strings in Python.

str = """Welcome to the world of Python
I love Python and Python is very easy to learn
Practice makes man perfect"""
print(str) # will print output as follows

Output : 
Welcome to the world of Python
I love Python and Python is very easy to learn
Practice makes man perfect
We can also use triple single quotes(''' ''') to create multi-line strings in Python.

str = '''Welcome to the world of Python
I love Python and Python is very easy to learn
Practice makes man perfect'''
print(str) # will print output as follows

Output : 
Welcome to the world of Python
I love Python and Python is very easy to learn
Practice makes man perfect
Note: Using triple single quotes or triple double quotes

______
# Unit 1 - Lesson 7
______
7.1.1. Understanding List Creation
15:15
List is a data type of Python used to store multiple values of different types of data at a time. List are represented with [].

A list can be created by putting comma separated values between square brackets [].

The following program shows creation of two lists namely list1 and list2 :
list1 = [1, 2, "one", "hi"]
list2 = [4, 5, "hello"]
Values stored in the list are accessed using an index.

Index range between 0 to n-1, where n is the number of values in the list

Python allows negative indexing for lists. The index of -1 refers to the last value of the list, -2 refers to the second last value of the list and so on.

Printing lists: The lists can be printed using the built-in function print() as shown below.

list1 = [1, 2, "one", "hi"]
print(list1) # will print output as follows

Output :
[1, 2, 'one', 'hi']
list2 = [4, 5, "hello"]
print(list2) # will print output as follows

Output :
[4, 5, 'hello']

Accessing Values in Lists: A value at a particular index in a list is accessed using listname[index]

list2 = [4, 5, "hello"]
print(list2[1]) # prints the value present at 1st index in list2

Output :
5
Slicing lists: Slicing is used to access a subset of of a list. For a list l = [1, 4, 5, 7, 4, 15], a subset of list from 2nd index to 3rd index is obtained by l[2:4] which is equal to [5,7]. Slicing can be understood using the following examples:

Let us assume that we have a list l = [1, 4, 6, 22, 44, 12, 55, 66]

Slicing expression

  Value

Explanation

l[1:4]

[4, 6, 22]

The starting index is 1 and the ending index is 4. (Observe that the value at the index 4 is not included in the result)

l[3:-3]

[22, 44]

The starting index is 3 and the ending index is -3 which represents the third last element i.e 12

l[3:]

[22, 44, 12, 55, 66]

The stopping index is not specified so slicing is done till the end of the list.

l[:4]

[1, 4, 6, 22]

The starting index is not given so 0 is considered as starting index.


Slicing operation can be performed on strings as well.

In Python, the plus (+) operator is a list concatenation operator and the asterisk (*) operator is the repetition operator.

Concatenating lists: We can concatenate two lists using (+) operator.

list1 = [1, 2, 'one', 'hi']
list2 = [4, 5, 'hello']
print(list1 + list2) # will print output as follows

Output: 
[1, 2, 'one', 'hi', 4, 5, 'hello']
Repeating lists: We can print a list multiple times using (*) operator as shown below.

list2 = [4, 5, 'hello']
print(2 * list2) # will print output as follows

Output :
[4, 5, 'hello', 4, 5, 'hello']
Working with nested lists: The items of the list can be lists themselves, which means that the lists can be nested.

Let us consider example:
list1 = [23, 5.65, ["A", 34.23], "India"]
In the above example, the third element (i.e index = 2) of list1 is a list.

We access the 3rd item by list1[2], which is a list and the second item of this list can be accessed using index 1. So, list1[2] [1] will be 34.23.

Write the missing code given to understand List Concatenation. Follow the instructions given as comment lines in the program.

````python
value1 = input("Enter the first value: ")
value2 = input("Enter the second value: ")
value3 = input("Enter the third value: ")
list1 = [value1,value2,value3] # create llist one with above three variables
print("List1:",list1) 
#print the list1

value4 = input("Enter the first value: ")
value5 = input("Enter the second value: ")
value6 = input("Enter the third value: ")
list2 = [value4,value5,value6] 
# create llist one with above three variables


# print the list2
print("List2:",   list2   )
# Concatenate list1 and list2 and print the result

print("List after Concatenation:", list1 + list2     )
````
7.1.2. Accessing items in a List
19:04
We can access the elements of a list by using index similar to accessing the individual characters of a string.

Unlike strings, lists are mutable i.e. we can modify the list (change the items, add items and reassign an item).

The following operations can be performed on the list :
 Modify or reassign an item present at a particular index.
 Add an item to the list at a particular index.
 Remove an item from the list.
Consider a list chars equal to ['a', 'b', 'c', 'd' ], the code to change the item at 3rd index from 'd' to 'xyz' is as follows :

chars = ['a', 'b', 'c', 'd']
chars[3] = 'xyz'
print(chars) # will print output as follows

Output :
['a', 'b', 'c', 'xyz']
Trying to access an index that does not exist in a list results in an error called "IndexError".

chars = ['a', 'b', 'c', 'd']
chars[4] = 'abcd' # Valid indices are only 0, 1, 2, and 3.

Output : 
Traceback (most recent call last):  
	File "1.py", line 2, in 
		chars[4] = 'abcd'
IndexError: list assignment index out of range
Add an item to the list

The append() method is used to add items to the list.

chars = ['a', 'b', 'c', 'd']
chars.append("abcd")
print(chars) # will print output as follows

Output :
['a', 'b', 'c', 'd', 'abcd']
Consider the following example :

chars = ['a', 'b', 'c', 'd']
chars.append( ['e', 'f'])  # This will append the list ['e', 'f'] as the last item to the chars list.  
print(chars) # will print output as follows 

Output :
['a', 'b', 'c', 'd', ['e', 'f']]
The above program shows that if a list is passed to append() method, it would append the entire list as a single item to the list.

Adding items of a list as individual items of another list

The extend() method is used to add items of one list to be added as individual items of another list.

chars = ['a', 'b', 'c', 'd']
list2 = [1, 2, 3]
chars.extend(list2)
print(chars) # will print output as follows

Output : 
['a', 'b', 'c', 'd', 1, 2, 3]

Note : Closely observe that the items of list2 are added as individual items to the chars list.
Fill in the missing code in the program. Follow the instructions given in comment lines.

````python

value1 = input("Enter the first value: ")
value2 = input("Enter the second value: ")
value3 = input("Enter the third value: ")

list1 = [value1,value2,value3] # create list1
print(list1[0])
print(list1[1])
print(list1[2])

# print every element in list1 using index
list1[2] = "Python"
print(list1) # print list1

list1.append("Code is Life") # add "Code is Life" to list1
print(list1) # print list1

value4 = input("Enter the first value: ")
value5 = input("Enter the second value: ")
value6 = input("Enter the third value: ")

list2 = [value4,value5,value6]# create list2
list1.extend(list2)
# Extend list1 with the elements from list2
print(list1)
# print list1

````

7.2.1. Introduction to Set
04:46
A set is a mutable data type that contains an unordered collection of items. A set is represented with { }.

Every element in the set should be unique (no duplicates) and must be immutable (which cannot be changed). But the set itself is mutable. We can add or remove items / elements from it.
Note: Mutable data types like list, set and dictionary cannot become elements of a set.

The set itself is mutable i.e. we can add or remove elements from the set.

The main uses of sets are:
 Membership testing
Removing duplicates from a sequence
Performing mathematical operations such as intersection, union, difference, and symmetric difference

Creation of sets
1. One way to create a set is by using built-in function set()

Empty set
An empty set can be created using built-in set() function.

myset = set()
print(myset)       # Result: set()
print(type(myset)) # <class 'set'>
2. Another way to create a set is to put all elements inside curly braces separated by commas.
myset1 = {1, 2, 3} 
print(myset1)       # Result: {1, 2, 3}
print(type(myset1)) # Result: <class 'set'>
Note : Empty curly braces { } does not make an empty set in Python, it makes an empty dictionary instead. Dictionary data type is introduced in the upcoming lessons.
test = { } 
print(type(test)) Result: <class 'dict'>

7.3.1. Introduction to Tuple
16:44
A tuple in Python is similar to a list, but with important distinctions:

Lists are enclosed in square brackets [], and their elements and size can change (mutable). Tuples are enclosed in parentheses () and are unchangeable (immutable).
Tuples are similar as read-only lists, providing a performance advantage during iteration due to their immutability.
Once defined, you can't add or remove elements from a tuple.
You can convert a tuple to a list to modify its elements and revert it to a tuple later.


Creating a tuple:

Use the built-in tuple() function.
An empty tuple can be created with tuple1 = tuple().
tuple1 = tuple()
print(tuple1) # Result: ()
Tuples can be defined by placing items within parentheses, separated by commas.
The parentheses are optional but it is a good practice to write them.
A one-element tuple must require a trailing comma, like (1,).
mytuple = (1, 2, 3, "Data types")
print(mytuple)        # Result: (1, 2, 3, "Data types")
print(type(mytuple))  # Result: <class 'tuple'>
Be cautious with single-element tuples:

(1) is interpreted as an integer, not a tuple. Use (1,) for a one-element tuple.
Consider the following program:

mytuple = (1)
print(mytuple)       # Result: 1
print(type(mytuple)) # Result: <class 'int'>


One-element tuples can be created as follows :

mytuple = (1,)
print(mytuple)       # Result: (1,)
print(type(mytuple)) # Result: <class 'tuple'>/span>


Multiple-element tuples:

Trailing commas in multiple-element tuples are optional.

Multiple-element tuple looks like this:

(1, 2, 3) or 1, 2, 3

(or)

(1, 2, 3,) or 1, 2,



Note:

The trailing comma is mandatory for the one-element tuples.
The trailing comma is completely optional for the multiple-element tuples.


7.3.2. Accessing elements in tuples
09:48
Individual elements of the tuple can be accessed using index similar to lists.

tuple1 = ("hi", "hello", 55, 66)
print(tuple1[0]) # Printing the element at the  0th index of the tuple, tuple1

Output:
hi
Negative index values can also be used to access the individual elements. -1 represents the last element, -2 represents the second last element and so on.

tuple1 = ("hi", "hello", 55, 66)
print(tuple1[-2]) # Printing the second last element of the tuple.  

Output:
55
Trying to access an element using an index outside the range results in an IndexError.

tuple1 = ("hi", "hello", 55, 66)
print(tuple1[4]) # Printing the element at the 4th index of the tuple, tuple1 results in an IndexError.

Output:
Traceback (most recent call last):  
	File "1.py", line 2, in     
		print(tuple1[4])
IndexError: tuple index out of range
Reassigning any value to tuple element results in an TypeError as tuples are immutable.

 
tuple1 = ('hi', 'hello', 55, 66) 
tuple1[1]= 'world' # Reassigning a value to an element of tuple results in a TypeError. 

Output : 
Traceback (most recent call last):
	File "1.py", line 2, in 
		tuple1[1]= 'world'
TypeError: 'tuple' object does not support item assignment
Write the missing code in the program and understand the result. Follow the instructions given in the editor

````python
value1 = input("first value: ")
value2 = input("second value: ")
value3 = input("third value: ")
value4 = input("fourth value: ")
value5 = input("fifth value: ")
mytuple =(value1,value2,value3,value4,value5) # create tuple with the above 5 inputs
print(mytuple)
# Print value at index 0
print(mytuple[0])
# Print value at index 1
print(mytuple[1])
# Print value at index -1
print(mytuple[-1])
# Print all the values from index 0
print(mytuple[0::])
# Print all the values except the last value
print(mytuple[0:-1])
print(mytuple[::-1])
````
7.3.3. Converting a tuple into a list and a list into a tuple
09:37
It is possible to convert tuples into lists and vice versa using built-in functions like tuple() and list()

Converting a tuple into a list

A tuple can be converted into a list using the built-in list() function.

tuple1 = ('hi', 'hello', 55, 66) # Creating a tuple, tuple1
print(tuple1) # Printing tuple1 , output contains values enclosed in parentheses indicating a tuple
print(type(tuple1)) # Printing the type of tuple1

list1 = list(tuple1) # Converting the tuple1 into a list using list() function.
print(list1) # Printing list1 , output contains values enclosed in square brackets indicating a tuple
print(type(list1))

Output :
('hi', 'hello', 55, 66)
<class 'tuple'>
['hi', 'hello', 55, 66]
<class 'list'>
Converting a list into a tuple

A list can be converted into a tuple using the built-in tuple() function.

tuple1 = ('hi', 'hello', 55, 66) # Creating a tuple, tuple1
print("Given tuple :",tuple1) 
list1 = list(tuple1) # Converting the tuple to a list using built-in list() function.
print("After conversion of tuple to list :",list1) 
list1[2] = "fifty five"  # Updating the value of element at 2nd index. This does not result in an error as the lists are mutable.
print("List after changing the element :",list1) 
tuple1 = tuple(list1)  # Converting the list back to tuple using the built-in tuple() method.
print("After converting list into tuple :",tuple1) # Printing the final tuple with the updated element at 2nd index.

Output :
Given tuple : ('hi', 'hello', 55, 66)
After conversion of tuple to list : ['hi', 'hello', 55, 66]
List after changing the element : ['hi', 'hello', 'fifty five', 66]
After converting list into tuple : ('hi', 'hello', 'fifty five', 66)
To modify an individual element in a tuple, follow these steps:
Convert the tuple into a list.
Update the desired element within the list.
Convert the modified list back into a tuple.

Write a program to convert the tuple into list. Follow the instructions given below:
 In the below program tuple values are initialized
 Print the element using the print statement "Given Tuple:"
 Convert the tuple into list using list function
 After converting print the list elements using the print statement "After Converting Tuple into List:"
 Change the value at index 1 to practice in the list
 Print the list using the print statement "List after changing element:"
 Convert the list into tuple and print the final tuple elements using the statement "After Converting List into Tuple:"
The result should be as follows:
Given Tuple: ('i', 'love', 'python')
After Converting Tuple into List: ['i', 'love', 'python']
List after changing element: ['i', 'practice', 'python']
After Converting List into Tuple: ('i', 'practice', 'python')

````python
mytuple = ("i", "love", "python")

# Write the missing code here
print("Given Tuple:",mytuple)
list1=list(mytuple)

print("After Converting Tuple into List:",   list1  )

list1[1]="practice"
print("List after changing element:",list1)

tuple=tuple(list1)
print("After Converting List into Tuple:",   tuple  )
````

______
# Unit 1 - Lesson 8
________

8.1.1. Introduction to Dictionary
06:41
Dictionaries:
Dictionary is an unordered collection of key and value pairs.
General usage of dictionaries is to store key-value pairs like Employees and their wages, Countries and their capitals, Commodities and their prices etc.
In a dictionary, the keys should be unique, but the values can be similar.
Immutable data types like number, string, tuple etc. are used for the key and any data type is used for the value.
Dictionaries are optimized to retrieve values when the keys are known.
Dictionaries are represented using key-value pairs separated by commas inside curly braces {}.
The key-value pairs are represented as key : value.
   For example:, daily temperatures in major cities are mapped into a dictionary as { "Hyderabad" : 27 , "Chennai" : 32 , "Mumbai" : 40 }.
Note: While other compound data types (like lists, tuples and sets) have only value as an element, a dictionary has a key : value pair


Creating a dictionary:
A dictionary can be created in two ways.

1. Using built-in dict() function.

An empty dictionary can be created as follows :
mydict = dict()      # Creating an empty dictionary called mydict
print(type(mydict))  # Result: <class 'dict'>
print(mydict)        # Result: {} 
A dictionary with elements can be created as follows :
mydict = dict("Hyderabad" : 20, "Delhi" : 30)  # A dictionary with two key pairs is created.
print(mydict)                                  # Result: {'Hyderabad': 20, 'Delhi': 30} 
Note : The two key pairs are specified in the dict() function as comma separated key : value.


2. Assigning elements directly:

A dictionary is created using direct assignment as follows :
mydict = {1:"one", 2 :"two", 3:"three"}   # Create a dictionary with three key-value pairs.
print(mydict)                             # Result: {1:"one", 2 :"two", 3:"three"}
print(type(mydict))                       # Result: <class 'dict'>

8.1.2. Understanding Dictionary
08:14
Let us create a dictionary called dict1 with three keys named as name, number and age, values of dictionary are Jay , 514, and 12 and then try to get values using respective keys.

1. Creating a dictionary:
dict1 = {"name":"Jay", "number":514, "age":12}
print(dict1)            #Result : {'name': 'Jay', 'number': 514, 'age': 12}

2. Let us retrieve the values using their keys as index:
print(dict1['age'])     # using key called 'age', we can get value 12
print(dict1['number'])  # using key called 'number', we can get value 514

3. Let us find what happens when we try to retrieve an element (key) which is not present in the dictionary:
print(dict1['place'])   #Results in KeyError as there is no key 'place' in the dictionary
If the key is not there in the dictionary, we get a KeyError .

4. We can change (update) the values in a dictionary.
dict1['name'] = "Krithika"
print(dict1)           #{'name':'Krithika' ,'number':514, 'age':12}

Identify the errors in given program and correct the program.
````python

mydict = {"game":"chess","dish":"chicken","place":"home"}
print(mydict.get('game'))
print(mydict['dish'])
print(mydict.get('place'))
mydict["game"] = "cricket" # change game chess to cricket using respective key
print(mydict['game'])
````

8.1.3. Accessing Elements of Dictionary
06:13
We cannot use a numerical index (as in lists, tuples and strings) to access the items/elements of the dictionaries as dictionaries are unordered(Imagine all the items of a dictionary are put in a bag and jumbled, so there is no order and we cannot retrieve the items using a sequential index.)

The elements of the dictionary can be retrieved/accessed in 2 ways.

1. Using the keys of the dictionary.
capitals = {"U.S.A": "Washington D.C", "India": "New Delhi", "Nepal": "Kathmandu"}
print(capitals["India"])        # Printing the value with the key "India" i.e. "New Delhi".

Trying to access an element in the dictionary using a key that is not present in the dictionary, results in a Key Error.
capitals = {"U.S.A": "Washington D.C", "India": "New Delhi", "Nepal": "Kathmandu"}
print(capitals["Australia"])    # Since the key "Australia" is not present, it results in a Key Error

2. Using the get() method.
capitals = {"U.S.A": "Washington D.C", "India": "New Delhi", "Nepal": "Kathmandu"}
print(capitals.get("India"))   # Printing the value with the key "India" i.e. "New Delhi".

Trying to access a key that is not present in the dictionary using the get() method results in None
capitals = {"U.S.A": "Washington D.C", "India": "New Delhi", "Nepal": "Kathmandu"}
print(capitals.get("Australia")) # Since the key "Australia" is not present, it results in a "None"

Write the missing code in the program to retrieve the elements of the dictionary using keys.
````python
# Taking input from the user for keys and values
key1 = input("key1: ")
value1 = input("value1: ")

key2 = input("key2: ")
value2 = input("value2: ")

key3 = input("key3: ")
value3 = input("value3: ")

# Construct the dictionary with the given key and value
dict1={key1:value1,key2:value2,key3:value3}
print(dict1)# print the dictionary

# Print the values of dictionary using keys
print(dict1[key1])
print(dict1[key2])
print(dict1[key3])
````

8.2.1. Data Type Conversion - int,float
00:45
Converting data of one type to data of another type is called Type Conversion. Python defines various type conversion functions.

1. int(x, base): This function converts x to an integer of the specified base, the default x value is 0. If the base is not specified, it defaults to 10.

The syntax of int() function is:
int(x=0, base=10)
Consider the following program to understand the working of int() function.
s = "0011"       # A binary string.
print(int(s, 2)) # Result: 3
print(int(s))    # Result: 11
If "0011" is considered with base 2, then its integer value will be 3, whereas if "0011" is considered with base 10, then its integer value will be 11.

2. float(x): This function is used to convert any data type to a floating point number. The float() function returns a floating point number from a number or a string.

The syntax of float() function is:
float(x)
where x is a number or string that needs to be converted to a floating point number. If it's a string, the string should contain decimal points

The below table gives information about the Usage of the float() functions and their respective outputs with the explanation.

print(float(23.4))

23.4

The parameter is already a float number. So no conversion happens

print(float(9))

9.0   

The integer 9 is converted to float 9.0 

print(float("32"))

32.0   

The string "32" is converted to float 32.0     

print(float("-42.48"))

-42.48

The string "-42.48" is converted into float -42.48

print(float(" -24.45 "))

-24.45

Leading and trailing spaces are trimmed and converted to float value.

print(float("InF"))

inf   

inf represents the upper bound value of float.

print(float("InFiNiTy"))

inf      

The case of text does not matter. Words used : inf or infinity

print(float("nan"))

nan      

nan represents not a number.

print(float("NaN"))

nan   

The case of text does not matter.

print(float("CodeTantra"))

ValueError

Cannot convert string "CodeTantra" to float.




Write a simple program to convert given input values to floating point values.
````python
a = int(input("Enter a value: "))
b = input("Enter b value: ")

# Convert "a" to floating point value and print it
print(float(a))
# Convert "b" to floating point value and print it
print(float(b))
````
8.2.2. Data Type Conversion - ord(), hex(), oct and complex()
04:10
3. ord( ): The ord() method returns an integer representing a Unicode code point for the given Unicode character.

The syntax of ord() function is:
ord(c)
Examples:
print(ord('A'))   # Result: 65
print(ord('a'))   # Result: 97
print(ord('AB'))  # Results TypeError
If the length of the string is greater than 1, then ord() function results in a TypeError.

4. hex(x): The hex() function converts an integer to its corresponding hexadecimal string.

The syntax of hex() function is:
hex(x)
Examples:
print(hex(45))  # Result: '0x2d'.
print(hex(9.9))  # Results TypeError
A non-integer results in a TypeError: 'float' object cannot be interpreted as an integer
Note: The returned hexadecimal string starts with prefix "0x" indicating that it is in hexadecimal form.

5. oct(x): The oct() method takes an integer and returns its octal representation.

The syntax of oct() function is:
oct(x)
print(oct(45))  # Result: '0o55'
print(ord(9.9))  # Results TypeError
A non-integer results in a TypeError: 'float' object cannot be interpreted as an integer
Note: The returned octal string starts with prefix "0o" indicating that it is in octal form.

6. complex(real, imag): The complex() method returns a complex number when the real and imaginary parts are provided, or it converts a string to a complex number.

The syntax of complex() function is:
complex(real, imag)
print(complex(10, 3)) # Result: (10 + 3j)
print(complex("10+4j")) # Result: (10 + 3j)
If the first parameter passed to this method is a string, it will be interpreted as a complex number.
Note: The string passed to the complex() should be in the form real + imag

Follow the comment lines in the given editor and complete the code.
````python

a = input("Enter character: ")
b = int(input("Enter an integer: "))

# Calculate and print the Unicode code point of 'a'
print(ord(a))  
# Calculate and print the hexadecimal representation of 'b'
print(hex(b))
# Calculate and print the octal representation of 'b'
print(oct(b)) 
# Calculate and print the complex number representation of 'b' and '0'
print(complex(b, 0))


````
8.2.3. Data Type Conversion - str(),eval() and chr()
03:09
7. str(x): The str() function is used to convert x to a string representation.

The syntax of str() function is:
str(object='')
str(object=b'', encoding='utf-8', errors='strict')
If no object is given, it returns an empty string. The behaviour of str() depends on whether encoding or errors are specified.

object - object whose informal representation is to be returned
encoding - Defaults of UTF-8. Encoding of the given object
errors - response when decoding fails.

Example:
      
print(str(100)) # Result: 100

8. eval(str): The eval() method parses the expression passed to this method and runs python expression (code) within the program.

The syntax of eval() function is:
eval(expression, globals=None, locals=None)

expression: this string is parsed and evaluated as a Python expression.
globals (optional): a dictionary to specify the available global methods and variables.
locals (optional): another dictionary to specify the available local methods and variables.

Example:
a = 100
b = 3
print(eval("a + b")) # Result: 103

9. chr(): The chr() method returns a character (a string) from an integer (that represents unicode code point of the character). This is the inverse of ord() function.

The syntax of chr() function is :
chr(i)
i - integer value, The valid range of i is from 0 through 1,114,111(0x110000).

Example:
print(chr(97))      # Result: a
print(chr(65))      # Result: A
print(chr(1200))    # Result: Ұ
If the value is outside the range of (0 , 1114111), it results in a ValueError: chr() arg not in range(0x110000).
print(chr(-1))       # Results ValueError
print(chr(1114112))  # Results ValueError

Follow the comment lines in the given editor and complete the code.
````python

a = int(input("Enter an integer: "))

# Calculate and print the character representation of 'a'
print(chr(a))
# Calculate and print the string representation of 'a'
print(str(a))
````
8.2.4. Data Type Conversions
36:14
10. tuple( ) : This function is used to convert any data type to a tuple.
str = "python"
print(tuple(str)) # Result: ('p', 'y', 't', 'h', 'o', 'n')
11.set( ) : This function is used to convert any data type to set.
str = "python"
print(set(str)) # Result: {'n', 't', 'p', 'h', 'y', 'o'}
12. list( ) : This function is used to convert any data type to a list type.
str = "python"
print(list(str)) # Result: ['p', 'y', 't', 'h', 'o', 'n']
13.dict(d) : This function is used to create a dictionary, but d must be tuple of order (key, value).
mytuple = ((1, 'a'), (2, 'b')) 
print(dict((y, x) for x, y in mytuple)) # {'a': 1, 'b': 2}
Here we used for loop to iterate every element of tuple object and we use dict( ) function to convert tuple elements into key-value pairs.

Note:zip() function in Python is used to map a similar index of multiple containers. We learn more details on zip( ) in the upcoming sections.


Follow the comment lines in the given editor and complete the code.
Hint: Since a set does not maintain the order of insertion, use sorted(set) to print the result in the sorted order.

````python
tup1 = tuple(input().split(","))
tup2 = tuple(input().split(","))

print(tup1)# print tup1

print(tup2)# print tup2

list1 = list(tup1)# convert tup1 to list data type
list2 = list(tup2)# convert tup2 to list data type

print(list1)
print(list2)

dict1 =  zip(list1,list2) 
# create a dictionary with the elements of list1 as keys and list2 as values using dict().
print(dict(zip(list1,list2)))
set1 = set(list1)# convert dict1 to set data type

print(sorted(set1))
````
______
# Unit 1 - Lesson 9
_____
9.1.1. Reading input in Python - strings
03:49
In Python, to read input from the user, we have an in-built function called input().

The syntax for input() function is :
input([prompt])
Here, the optional prompt string will be printed to the console for the user to input a value. The prompt string is used to indicate the type of value to be entered by the user.

Reading string inputs

Let us consider the below example:

name = input("Enter your Name: ")
print("User Name:", name)
If the input is given as CodeTantra, the result will be

User Name: CodeTantra
If the input is given as Jacob, the result will be

User Name: Jacob
If you want to take only specified data type input from the user, you need to mention the data type before the input.

 For example : a= int(input("Enter an integer :")

So that, if the user gives an input other than the mentioned data type, it results in the valueError.

Write a program to print your favourite place.
````python
place = input("favourite place: ") #take your favourite place using input statement

print("My favourite place is:", place)# Print your favourite place

````
9.1.2. Understanding Output in Python.
01:26
We already discussed this function to print output on Screen.

It is print() function, which is a built-in function in Python.

We can pass zero or more number of expressions separated by commas(,) to print() function.

The print() function converts those expressions into strings and writes the result to standard output which then displays the result on screen.

Let us consider an example of print() with multiple values with comma(,) as separator.

print("Hi", "Hello", "Python") # will print output as follows
Hi Hello Python
Let us discuss another example:

a = 10
b = 50
print("A value is", a, "and", "B value is", b) # will print output as follows
A value is 10 and B value is 50
Here we have assigned values 10 and 50 to a and b respectively.

The above print() statement consists of both strings and integer values.

Write a program to print your favourite programming language.

At the time of execution, the program should print the message on the console as:

Enter Language: 
For example, if the user gives the input as:

Enter Language: Python
then the program should print the result as:

My Favourite Language is Python
Identify the error and correct the given code.

````python
lang = input("Enter Language: ")
print("My Favourite Language is",lang)
````

9.1.3. % - formatting and str.format() function
06:36
The print() function is used to print the values to the standard output.

The general syntax of print() function is:
print(value1, value2..., sep = ' ', end = '\n', file = sys.stdout, flush = False)

where,

value1,value2...,valuen These are the actual data values to be printed.

sep: It is the separator used between each value. If there is no separator, then by default 'whitespace' is taken.

end: It is the character which gets printed after all values have been printed. The newline character '\n' is the default. 

file: This argument specifies where the output needs to be printed. The screen is the standard output by default


Output Formatting in Python

1. Python uses C-style string formatting to create new, formatted strings. The % operator also called as 'string modulo operator' is used to format a set of variables enclosed in a "tuple" (a fixed size list), together with a format string, which contains normal text together with "argument specifiers", special symbols like %s and %d.

The general syntax for a format placeholder is:
%[flags][width][.precision]type
The following are some basic argument specifiers:
%s - String (or any object with a string representation, like numbers)
%d - Integers
%f - Floating point numbers
%.<number of digits>f  - Floating point numbers with a fixed amount of digits for the decimal part.
%x or %X - Integers in hexadecimal representation (uppercase/lowercase)
%o - Octal representation
Example 1: If we consider a single variable called 'name' with a username in it, and if we would like to print a greeting to that user, then:
name = "Ravi"
print("Good morning, %s!" % name) # This statement prints "Good morning, Ravi!"
Output:
Good morning, Ravi!
Example 2: If we consider more than one variable, we must use a tuple of those variables as shown below:
a = 10
b = 20
str = "Hello"
print("The value of a = %d, b = %d and str = %s" %(a, b, str))
Output:
The value of a = 10, b = 20 and str = Hello
Example 3:
print("Total number of votes: %4d, Women votes: %2d" %(480, 70))
Output:
Total number of votes: _480, Women votes: 70 # Observe 1 leading blank space left before the first value and no leading blank space before the second value 
Let us understand the placeholders in the above example:
The first placeholder %4d is used for the first component of our tuple, i.e. 480. This number will be printed with 4 characters. As 480 consists only of three digits, the output is padded with 1 leading blank.
The second placeholder %2d is used for the second component of our tuple, i.e. 70. This number will be printed with 2 characters. As 70 consists two digits, the output does not have any leading blanks as both the blanks are occupied by the digits.

2. The output can also be presented in a more elegant way using the str.format()

This style of string formatting eliminates the usage of % operator (string modulo operator).

The general syntax of str.format() function is:
{}{}.format(value1, value2,...,valuen)

where,

{}{} are place holders created by the user in the string.

value1,value2,...,valuen They could be variables, integers, floating-point numbers, strings, characters etc. 


Note:The number of values passed as arguments in .format(arg1,arg2..) method should always be equal to the number of placeholders {} created by the user in the string.
The following are some basic argument specifiers used with str.format():
{} - String (or any object with a string representation, like numbers)
{0:<number of digits>d} - Integers
{0:.<number of digits>f} - Floating point numbers with a fixed amount of digits for the decimal part.
{0:X} or {0:x} - Integers in hex representation (uppercase/lowercase)
{0:o} - Octal representation

Click on  button to know about string formatting using format method in Python

Example 1:
a = 10
b = 20
str = "Hello"
print("The value of a = {}, b = {} and str = {}".format(a, b, str))
Output:
The value of a = 10, b = 20 and str = Hello
Here the curly braces {} are used as placeholders in the format string. We can also use the tuple indices within each of the curly braces which correspond to its respective value in the argument list of format() as shown below.

Example 2:
a = 10
b = 20
str = "Hello"
print("The value of a = {0}, b = {1} and str = {2}".format(a, b, str))
Output:
The value of a = 10, b = 20 and str = Hello
Here, the index 0 corresponds to the variable represented by a. Likewise the indices 1 and 2 for b and str.

Follow the instructions given in comment lines and write the program to understand format method.
````python

a=int(input("a: "))# Take an integer input from the user and store it in variable "a"

b=int(input("b: "))# Take an integer input from the user and store it in variable "b"

# print "a" value at 0 index and "b" value at 1 index


"""print("a = {0} b = {1}".format(a, b))
print("a = {} b = {}".format(b, a))"""

# print by changing the index postions of "a" and "b" and observe the output



print(f"a = {a} b = {b}")
print(f"a = {b} b = {a}")

````

9.1.4. % - formatting and str.format() function
19:02
Follow the instructions given and write a program to print the user-given number in different formats using the format specifier.



If we want to limit the decimal places of a certain value, we use the format {.nf} where n is the count of the decimal places.



Example: If the variable is assigned with number 6 and the format is taken as "{0:.4f}".format(variable) then it results in 6.0000.



Also, If we want to print a number X after n spaces, we use the format {:(number of digits of X + n)d}.



Let's say, we want to print the number 12 after 4 spaces, we use the format {:(2 + 4)d} which can be justified as the number of digits of 12 is 2 and we require 4 spaces.



More Examples:

print("{0:10d}".format(5)) will print 5 after 9 spaces/blanks.
print("{0:3d}".format(123)) will print 123 after 0 spaces/blanks.


Use the format specifiers concept and write the program in the given editor by following the comment lines. Observe the output.



Sample Input and Output:

a: 3
3.00
3.000000
b: 15
15
15
 15
octal: 17
hex: F


````python
"""
# take float number from the user
a = float(input("a: "))
# print up to 2 decimal points
print("{:.2f}".format(a))
# print up to 6 decimal points
print("{:.6f}".format(a))
# take int number from the user
b = int(input("Enter b value: "))
# print the number with one space
print("{:1d}".format(b))
# print the number with two spaces
print("{:2d}".format(b))
# print the number with three spaces
print("{:3d}".format(b))
# print the given number b in octal form
print(f"octal: {b:o}")
# print the given input b in hexadecimal form
print(f"hex: {b:X}")


"""
# take float number from the user
a = float(input("a: "))
# print up to 2 decimal points
print(f"{a:.2f}")
# print up to 6 decimal points
print(f"{a:.6f}")
# take int number from the user
b = int(input("Enter b value: "))
# print the number with one space
print(f"{b:1}")
# print the number with two spaces
print(f"{b:2}")
# print the number with three spaces
print(f"{b:3}")
# print the given number b in octal form
print(f"octal: {b:o}")
# print the given input b in hexadecimal form
print(f"hex: {b:X}")


````
______
# Unit 1 - Lesson 10
____
10.1.1. Arithmetic Operators - An overview
00:57
Python supports the following 7 arithmetic operators.

Operator		Operation												Expression and its result

+				Adds values on either side of the operator.				10 + 20 = 30

-				Subtracts right hand operand from left hand operand.	20 - 10 = 10

*				Multiplies values on either side of the operator		11 * 11 = 121

/				Divides left hand operand by right hand operand			23 / 2 = 11.5

**				Performs exponential (power) calculation on operators	2 ** 3 = 8

%				Divides left hand operand by right hand operand 
				and returns remainder									12 % 5 = 2

//				Floor Division - The division of operands where the 
				result is the quotient in which the digits after the 	23 // 2 = 11 (Integer division)
				decimal point are removed. But if one of the operands	9.0 // 2.0 = 4.0 
				is negative, the result is floored, i.e., rounded away 	-11 // 3 = -4
				from zero (towards negative infinity).					-11.0 // 3 = -4.0	

10.1.2. Using Arithmetic Operators
01:27
Write a program to read two int inputs from the user and display the results of the following arithmetic operations:

Sample Input and Output:
num1: 12
num2: 4
12 + 4 = 16
12 - 4 = 8
12 * 4 = 48
12 / 4 = 3.0
12 ** 4 = 20736
12 % 4 = 0
12 // 4 = 3

````python
#Arithmetic Operators are +, -, *, /, **, %, //
num1 = int(input("num1: "))
num2 = int(input("num2: "))

# print num1+num2
print('%d + %d =' %(num1, num2), num1+num2   )
# print num1-num2
print('%d - %d =' %(num1, num2), num1-num2   )
# print num1*num2
print('%d * %d =' %(num1, num2), num1*num2   )
# print num1/num2
print('%d / %d =' %(num1, num2), num1/num2   )
# print num1**num2
print('%d ** %d =' %(num1, num2), num1**num2   )
# print num1%num2
print('%d %% %d =' %(num1, num2), num1%num2   )
# print num1//num2
print('%d // %d =' %(num1, num2), num1//num2   )
````
10.1.3. Writing a program on arithmetic operators
02:20
Write a program to read two int inputs from the user and perform the following arithmetic operations addition, subtraction, multiplication, and division and print the result.

Sample Input and Output:
Addition of 40 and 10 = 50
Subtraction of 40 and 10 = 30
Multiplication of 40 and 10 = 400
Division of 40 and 10 =  4.0

````python
num1 = int(input ("num1: "))
num2 = int(input ("num2: "))


# Print the addition of num1 and num2
print('Addition of %d and %d =' %(num1, num2), num1+num2)
# Print the subtraction of num1 and num2
print('Subtraction of %d and %d =' %(num1, num2), num1-num2)
# Print the multiplication of num1 and num2
print('Multiplication of %d and %d =' %(num1, num2), num1*num2)
# Print the division of num1 and num2
print('Division of %d and %d =' %(num1, num2), num1/num2)

````
10.1.4. Some more arithmetic operators
02:07
Write the program to read two integer inputs from the user and perform the following arithmetic operations over it.
 Calculate Exponent of num1 and num2
 Calculate Modulus Division
 Calculate Floor Division
During execution, the program should print the message on the console as mentioned in the sample test case

Sample Input and Output:
num1: 10
num2: 5
Exponent of 10 with 5 = 100000
Modulus of 10 and 5 = 0
Floor Division of 10 and 5 = 2

````
num1 = int(input("num1: "))
num2 = int(input("num2: "))

# Print the exponenet of num1 to the power of num2
print('Exponent of %d with %d =' %(num1, num2), num1**num2)
# Print the modulous function of num1 and num2
print('Modulus of %d and %d =' %(num1, num2), num1%num2)
# Print the floor division function of num1 and num2
print('Floor Division of %d and %d =' %(num1, num2), num1//num2)
````

10.1.5. Writing a program on some more arithmetic operators
11:32
Write a program that uses the following arithmetic operators.



** Exponent Operator



% Modulus Division



// Floor Division



The program should take two integer inputs from the user and print the result of the above-mentioned arithmetic operators.



Sample Input:

num1: 20

num2: 10

Sample Output:

Exponent of 20 with 10 = 10240000000000

Modulus of 20 and 10 = 0

Floor Division of 20 and 10 = 2

````
num1 = int(input("num1: "))
num2 = int(input("num2: "))
print("Exponent of %d with %d =" %(num1, num2),num1**num2)
print(f"Modulus of {num1} and {num2} = {num1%num2}" )
print("Floor Division of %d and %d =" %(num1, num2),num1//num2)
````

10.1.6. Explanation of divmod function
25:53
Write a program to find quotient and remainder of the given two values using divmod().

Sample Input and Output:
num1: 45
num2: 3
45 // 3 = 15
45 % 3 = 0

````python

#Program to illustrate divmod() function
# Input num1 with message "Enter number-1: "
num1 = int(input("num1: "))

# Input num2 with message "Enter number-2: "
num2 = int(input("num2: "))


# use divmod() and store results in 2 variables x, and y
x, y = divmod(num1, num2)

# replace variables in () and print the results
print(f"{num1} // {num2} = {x}")
print(f"{num1} % {num2} = {y}")
````

### Comparison Operators
10.2.1. Comparison Operators - An overview
05:17
Python supports the following comparison operators.The result of these comparison operators is either True or False.

Operator	Operation												Expression (Result)				

==			If the values of two operands are equal, 				23 == 34 (False)
			then the condition becomes True.						10 == 10 (True)

!=			If the values of two operands are not equal, 			23 != 34 (True)
			then the condition becomes True.						10 != 10 (False)

<			If value of left operand is less than value				10 < 20 (True) 
			of right operand, then condition becomes true.			20 < 5 (False)				

>			If value of left operand is greater than value			10 > 20 (False) 
			of right operand, then condition becomes true.			20 > 5 (True)				

<=			If value of left operand is less than or equal to 		10 <= 20 (True) 
			value of right operand, then condition becomes true.	20 <= 20 (True)				

>=			If value of left operand is greater than or equal to	10 >= 20 (False) 
			value of right operand, then condition becomes true.		    20 >= 20 (True)				
 
The symbols are read as follows :

> - Greater than

< - Less than

== - Is equal To

!= - Not equal To

>= - Greater than or equal to

<= - Less than or equal to

Write a program to understand the comparison operators in Python and perform the following operations >, <, ==, !=, <=, >= and print the result. Take two int inputs from the user.

Sample Input and Output :
Is 40 greater than 10 = True
Is 40 less than 10 = False
Is 40 equal to 10 = False
Is 40 not equal to 10 = True
Is 40 less than or equal to 10 = False
Is 40 greater than or equal to 10 = True


num1 = int(input("num1: "))
num2 = int(input("num2: "))

# Print Is num1 greater than num2.
print('Is %d greater than %d =' %(num1, num2), num1> num2    )
# Print Is num1 less than num2.
print('Is %d less than %d =' %(num1, num2),   num1<num2    )
# Print Is num1 equal to num2.
print('Is %d equal to %d =' %(num1, num2),  num1==num2    )
# Print Is num1 not equal to num2.
print('Is %d not equal to %d =' %(num1, num2), num1!=num2      )
# Print Is num1 less than or equal to num2.
print('Is %d less than or equal to %d =' %(num1, num2),  num1<=num2    )
# Print Is num1 greater than or equal to num2.
print('Is %d greater than or equal to %d =' %(num1, num2),  num1>=num2     )


10.2.2. Using Comparison operators
01:50
Take two integers as input from the console using input() function. For each comparison operator ( >, <, ==, !=, >=, <= ), print to the console, the result of the two input numbers as shown in the example.

Sample Input and Output:
num1: 20
num2: 10
Is 20 greater than 10 = True
Is 20 less than 10 = False
Is 20 equal to 10 = False
Is 20 not equal to 10 = True
Is 20 greater than or equal to 10 = True
Is 20 less than or equal to 10 = False

# Comparision Operators >, <, ==, !=, >=, <= on numbers
num1 = int(input("num1: "))
num2 = int(input("num2: "))

# Print Is num1 greater than num2.
print('Is %d greater than %d =' %(num1, num2), num1> num2    )
# Print Is num1 less than num2.
print('Is %d less than %d =' %(num1, num2),   num1<num2    )
# Print Is num1 equal to num2.
print('Is %d equal to %d =' %(num1, num2),  num1==num2    )
# Print Is num1 not equal to num2.
print('Is %d not equal to %d =' %(num1, num2), num1!=num2      )

# Print Is num1 greater than or equal to num2.
print('Is %d greater than or equal to %d =' %(num1, num2),  num1>=num2     )
# Print Is num1 less than or equal to num2.
print('Is %d less than or equal to %d =' %(num1, num2),  num1<=num2    )


10.2.3. Comparison operators with strings
03:52
All the comparison operators work on strings also. The result is either True or False.

Python compares strings using Unicode value of the characters (lexicographical).

The comparison is made taking the ordinal values of each character in the string and compare it with the ordinal values of the character at the same position in the other string.

If the ordinal value of the character in the first string is greater than the ordinal value of the character in the second string, then the comparison stops and the first string is declared as greater than the second string. The length of the string does not matter.

In Python, the ordinal value of a character can be found using the ord() function, which takes the character as an argument.

Note: You do not have to use ord() function. Python uses it to compare the strings internally.

Write a program to understand the use of comparison operators using conditional parameters. Take input from user using input() method.

Sample Input and Output
str1: Oliver
str2: Ethan
Oliver > Ethan = True
Oliver < Ethan = False
Oliver == Ethan = False
Oliver != Ethan = True
Oliver >= Ethan = True
Oliver <= Ethan = False


# write your code here
num1 = input("str1: ")
num2 = input("str2: ")

# Print Is num1 greater than num2.
print('%s > %s =' %(num1, num2), num1 > num2 )
print('%s < %s =' %(num1, num2), num1 < num2 )
print('%s == %s =' %(num1, num2), num1 == num2 )
print('%s != %s =' %(num1, num2), num1 != num2 )
print('%s >= %s =' %(num1, num2), num1 >= num2 )
print('%s <= %s =' %(num1, num2), num1 <= num2 )


10.2.4. Writing Comparison Operators on Strings
01:33
Take two strings as input from the console using input() function. For each of the comparison operators ( >, <, ==, !=, >=, <=), print to the console, the result of the comparison of the two input strings as shown in the example below.

Sample Input Output
str1: Code
str2: Tantra
Is Code greater than Tantra = False
Is Code less than Tantra = True
Is Code equal to Tantra = False
Is Code not equal to Tantra = True
Is Code greater than or equal to Tantra = False
Is Code less than or equal to Tantra = True

str1 = input("str1: ")
str2 = input("str2: ")

# Print Is str1 greater than str2
print('Is %s greater than %s =' %(str1, str2),      str1> str2 )
# Print Is str1 less than str2
print('Is %s less than %s =' %(str1, str2),  str1< str2    )
# Print Is str1 is equal to str2
print('Is %s equal to %s =' %(str1, str2),  str1== str2     )
# Print Is str1 not equal to str2
print('Is %s not equal to %s =' %(str1, str2),      str1!= str2 )
# Print Is str1 greater than or equal to str2
print('Is %s greater than or equal to %s =' %(str1, str2),  str1>= str2      )
# Print Is str1 less than or equal to str2
print('Is %s less than or equal to %s =' %(str1, str2),  str1<= str2      )

___
# Unit 1 - Lesson 11
___
Assignment Operators
11.1.1. Assignment Operators - overview
03:58
Assignment Operators are used to assign values to variables.

a = 52 is a simple assignment operator that assigns the value 52 on the right-hand side to the variable a on the left-hand side.

Note: An assignment operator assigns the value located on the right-hand side of the operator to the variable located on the left-hand side. The right side of the operator can be an operand or an expression that results in a value. The left hand side should be a variable.

Python programming language supports the following assignment operators :

Operator

Description

Expression

=

Assigns values from right-side operands to left-side operands.

c = a + b assigns value of a + b into c to left side operand

+=

Adds the right operand to the left operand and assigns the result to the left operand.

c += a, equivalent to c = c + a

-=

Subtracts the right operand from the left operand and assigns the result to the left operand.

c -= a, equivalent to c = c - a

*=

Multiplies the right operand with the left and assigns the result to the left operand.

c *= a, equivalent to c = c * a

/=

Divides the left operand with the right and assigns the result to the left operand.

c /= a, equivalent to c = c / a

**=

Performs exponential calculation on the left and right operands and assigns the result to the left operand.

c **= a, equivalent to c = c ** a

%=

Performs modulo division of left and right operands and assigns the result to the left operand.

c %= a, equivalent to c = c % a

//=

Performs floor division on left and right operands and assign the result to left operand

c //= a, equivalent to c = c // a



Take two integers as input from the console using input() function. For each assignment operator (+=, -+, *=, /=, **=, //=, %=, =), print to the console, the result of the two input numbers as shown in the example.

Sample Input and Output:
x: 40
y: 30
x +=y: x = 70 and y = 30
x -= y: x = 10 and y = 30
x *= y: x = 1200 and y = 30
x /= y: x = 1.3333333333333333 and y = 30
x **= y: x = 1152921504606846976000000000000000000000000000000 and y = 30
x //= y: x = 1 and y = 30
x %= y: x = 10 and y = 30
x = y: x = 30 and y = 30
Note: Before every assignment operation, set the values of x and y to the initially read values.

a = int(input("x: "))
b = int(input("y: "))
x = a
y = b
# calculate the value of x += y, assign it to x and print the x, y values
x+=y
print('x += y: x =', x   , 'and y =',  y   )
x = a
y = b
# calculate the value of x -= y, assign it to x and print x, y values

x -= y
print('x -= y: x =', x   , 'and y =',   y   )
x = a
y = b
# calculate the value of x *= y, assign it to x and print x, y values

x *= y
print('x *= y: x =', x    , 'and y =',   y  )
x = a
y = b
# calculate the value of x /= y, assign it to x and print x, y values
x /= y

print('x /= y: x =', x    , 'and y =', y    )
x = a
y = b
# calculate the value of x **= y, assign it to x and print x, y values

x **= y
print('x **= y: x =', x   , 'and y =',  y   )
x = a
y = b
# calculate the value of x //= y, assign it to x and print x, y values

x //= y
print('x //= y: x =', x   , 'and y =',  y   )
x = a
y = b
# calculate the value of x %= y, assign it to x and print x, y values

x %= y
print('x %= y: x =', x   , 'and y =',  y   )
x = a
y = b
# assign the value of x = y, assign it to x and print x, y values

x = y
print('x = y: x =',   x  , 'and y =', y    )


11.1.2. Write a program on assignment operators =,+=,-= and *=
06:06
Take two integers x and y as inputs from the console using input() function. For each assignment operator ( = , +=, -=, and *= ), print to the console, the result of applying these operators on the two input integers as shown in the example.

Assumption:
 y is a non-zero integer
Sample Input and Output:
x: 20
y: 30
x = y: 30
x += y: 50
x -= y: -10
x *= y: 600
Hint: Before every assignment operation, reset the values of x and y to the initial values.

# Assignment Operators =, +=, -=, *=
x=int(input("x: "))
y=int(input("y: "))
a=x
b=y
x = y
print("x = y:",x)
x=a
y=b
x += y
print("x += y:",x)
x=a
y=b
x -= y
print("x -= y:",x)
x=a
y=b
x *= y
print("x *= y:",x)

11.1.3. Write a program on operators /=,%=,**=
01:24
Take two integers x and y as inputs from the console using input() function. For each assignment operator ( /= , %=, **=, and //= ), print to the console, the result of applying these operators on the two input integers as shown in the example.

Assumption:
 y is a non-zero integer
Sample Input and Output:
x: 20
y: 10
x /= y: 2.0
x %= y: 0
x **= y: 10240000000000
x //= y: 2
Hint: Before every assignment operation, reset the values of x and y to the initial values.

# Assignment Operators  /= , %=, **=, //=
a = int(input("x: "))
b = int(input("y: "))
# assign the value of a to x and b to y and perform the mentioned operations on x, y
x=a
y=b
x /= y
print("x /= y:" , x  )
x=a
y=b
x %= y
print("x %= y:" ,  x )
x=a
y=b
x **= y
print("x **= y:" , x  )
x=a
y=b
x //= y
print("x //= y:" ,  x )

Bitwise Operators

11.2.1. Bitwise operators - an overview
00:36
Numbers can be used in many forms like decimal, hexadecimal, octal and binary. Computers store the numbers in binary format.



Numbers in binary format :

2 is "10"

3 is "11"

4 is "100"

678 is "1010100110"



Python Bitwise Operators take one or two operands, and operate on them bit by bit, instead of whole. Following are the bitwise operators in Python



1. << (Left shift):

Shifts the left-side operand bits towards the left side for the given number of times in the right operand.
This operation effectively multiplies the left-hand operand by 2 raised to the power of the number of positions shifted.
Example:

x = 12 = 0000 1100 ---> (Binary representation)
x << 2 = 0011 0000 ---> 48 
x = 12 and x << 2 will return 48 i.e. (12 * (2 ** 2))


2. >> (Right shift):

Shifts the left-side operand bits are moved towards the right side for the given number of times.
This operation is equivalent to dividing the left-hand operand by 2 raised to the power of the number of positions shifted.
Example:

x = 48 = 0011 0000 ---> (Binary representation)
x >> 3 = 0000 0110 ---> 6
x = 48 and x >> 3 will return 6 i.e. (48 / (2 ** 3))


3. & (AND):

Results bit 1, if both operand bits are 1; otherwise, results bit 0.
Example:

If the bit in x and the corresponding bit in y are 1, then the bit in the result will be 1. Otherwise, it will be zero

x = 10 = 1010
y = 4  = 0100
x & y  = 1010
    	&
         0100
      = 0000
      = 0 (Decimal)


4.| (OR):

Results bit 1 if any of the operand bits is 1; otherwise, results bit 0.
Example:

If the bit in both operands is zero, then the resulting bit is zero. otherwise, it is 1.

x = 10 = 1010
y = 4 = 0100
x | y = 1010
        |
       0100
     = 1110
     = 14 (Decimal)


5.~(NOT):

It is a unary operation that performs logical negation on each bit, forming the one's complement of the given binary value. Bits that are 0 become 1, and those that are 1 become 0.
Example:

x = 5
 x = 00000101
~ x = 11111010
~ x = -00000110 (in signed form)
Therefore ~x = -6 (in signed form)


6.^(XOR):

Results bit 1, if any of the operand bits is 1 but not both, otherwise results bit 0.
Example:

x = 10 = 1010
y = 4 = 0100 
x ^ y = 1010
        ^
        0100
      = 1110
      = 14 (Decimal)
      
11.2.2. Using Bitwise operators
07:00
Take two integers x and y as inputs form the console using input() function. For each bitwise operator ( >> and << ), print to the console, the result of applying these operators on the two input integers as shown in the example.

Assumption:
 Make sure the value of y is < 100 as this will be taken as power of 2
Sample Input and Output:
x: 12
y: 3
12 >> 3 is 1
12 << 3 is 96

#Program to illustrate bit wise operators >>, <<
x = int(input("x: "))
y = int(input("y: "))
a=x>>y
print(f"{x} >> {y} is {a}")
b=x<<y
print(x,"<<",y,"is",b)

11.2.3. Write a program using 'and' & 'or' Bitwise operators
03:26
Take two integers x and y as inputs from the console using input() function. For each bitwise operator ( & , | ), print to the console, the result of applying these operators on the two input integers as shown in the example.

Click on the  button to know and operator.

Click on the  button to know or operator.

Sample Input and Output:
x: 6
y: 3
6 & 3: 2
6 | 3: 7

#Program to illustrate the bitwise operators &, |
x = int(input("x: "))
y = int(input("y: "))
a=x&y
print(f"{x} & {y}: {a}")
b=x|y
print("%d | %d: %d"%(x,y,b))

11.2.4. Understanding Bitwise Complement Operator
00:17
The format for usage of one's complement ( ~ ) operator is:

~operand
Here, operand should be a primitive integral type.

This operator works on the binary representation of the given number.

It flips all the 1's to 0's and 0's to 1's.

Click on the  button to know not operator.

For example, if the ~ operator is applied on binary number 110, the result will be 001.


11.2.5. Writing Bitwise operators ~ and ^
07:25
Take two integers x and y as inputs from the console using input() function. For each bitwise operator ( ~ , ^ ), print to the console, the result of applying these operators on the two input integers as shown in the example.

Assumption:
Perform ~ on input x
Sample Input and Output:
x: 25
y: 6
~ 25: -26
25 ^ 6: 31

Are you surprised with the result of ~(not) operator? (~25 = -26 or in general ~(x) = -(x + 1) if x is positive and ~(x) = -(x) - 1, if x is negative.

This is because -ve numbers are represented in the computer in 2's complement form. 

#Program to illustrate bitwise operators ~, ^
x = int(input("x: "))
y = int(input("y: "))

print(f"~ {x}: {~x}")
b=x|y
print("%d ^ %d: %d"%(x,y,x^y))

11.2.6. Bitwise operators - an overview
00:54
Take two integers x and y as inputs from the console using input() function. For each bitwise operator ( >> , <<, &, |, ~, and ^ ), print to the console, the result of applying these operators on the two input integers as shown in the example.

Sample Input and Output:
x: 52
y: 20
52 >> 20 is 0
52 << 20 is 54525952
52 & 20 is 20
52 | 20 is 52
~ 52 is -53
52 ^ 20 is 32

x = int(input("x: "))
y = int(input("y: "))
# calculate the value of x >> y and print it

print ('%d >> %d is' %(x, y), x >> y     )

# calculate the value of x << y and print it

print ('%d << %d is' %(x, y),  x << y     )

# calculate the value of x & y and print it

print ('%d & %d is' %(x, y),  x & y     )

# calculate the value of x | y and print it

print ('%d | %d is' %(x, y), x | y      )

# calculate the value of ~x and print it

print ('~ %d is' %(x),    ~x    )

# calculate the value of x ^ y and print it

print ('%d ^ %d is' %(x, y),  x ^ y      )


11.2.7. Understanding Two's Complement
02:30
Two's complement is used to store a negative numbers in the memory.

The two's complement of a negative number is determined through these steps:
Calculate the one's complement of the given negative number.
Add binary 1 to the one's complement to obtain the two's complement.

Below are the steps for arriving at the two's complement of a value -14
Binary value of 14 ⟹ 00001110
One's complement of 14 ⟹ 11110001
                 Add 1 ⟹        1
Two's complement value ⟹ 11110010

Subtraction on binary values is performed using addition. For example in the below code:
int x = 2
int y = 1
int diff 
diff = y - x
diff = y - x
This is internally performed using addition as

diff = y + (-x) #The -x is arrived at using two's complement.
Click on the  button to know the working of two's complement in Python.

Note: Do try out converting different negative values in the above Live Demo and observe how the carry-on bit is used.

Take two integers num1 and num2 as inputs from the console using input() function. Perform two's complement on given two input integers, print the result to the console as shown in the example.

Sample Input and Output:
num1: 77
num2: 5
difference: 72

x = int(input("num1: "))
y = int(input("num2: "))

print("difference: %d"%(x-y))

___
# Unit 1 - Lesson 12
___

12.1.1. Logical Operators - An overview
00:10
Logical Operators : A logical operator is derived from boolean algebra where the result is either True or False.

It is generally used to represent logical comparison the way it is done in real life.

1 represents True and 0 represents False. (Internally 0 represents False and anything else represents True)

The logical operators supported in Python are similar to the logic gates and are as follows:

1. and - Logical AND : The result is True, only if both the operands are True. ( 1 and 1 is the only condition where the result is 1, any other combination results in 0.)

2. or - Logical OR : The result is True, if any one of the operands is True. ( 0 and 0 is the only condition where the result is 0, any other combination results in 1.)

3. not - Logical NOT : The result negates the operand, i.e if the operand is True, the result is False and vice versa


12.1.2. Logical Operators - An overview
20:03
The logical operators are used primarily in the expression evaluation to make a decision. They allow you to create complex conditions and control the flow of your program using conditional statements like if-else statements.



The if-else statement provides two different paths of execution depending on the result of the condition.

The body of if is executed when the condition associated with the expression is true.
The body of else part is executed when the condition is evaluated to false.
Indentation is used to separate both the if and else blocks.

Below is the general syntax for the if-else statement :

if(expression):
	body of If
else:
	body of else

Below is an example to illustrate the if-else construct.

if(marks > distinction_marks):
	print("User secured distinction")
else:
	print("User did not secure distinction")


This is an example for how control statements works. Understand the example given above and solve the question given. We will learn more about if-else in coming lessons.



Take two inputs from the user using the input() function, one is the gender of the person either M or F in string format and another one is the age of the person in integer format. Write a simple program to see whether the given person is eligible for concession or not and print the result as shown in the examples:



Follow these instructions to identify whether the person is eligible for the concession or not.

If the person is male and age >=65, Eligible for concession.
If the person is female and age >= 60, Eligible for concession.
In all other cases, the person is not eligible for concession.
Sample Input and Output 1:
M or F: F
age: 70
Eligible

Sample Input and Output 2:M or F: M
age: 63
Not Eligible

mf = input("M or F: ")
age = int(input("age: "))


# Check for concession and print the result
if mf=='M':
	if ( age>=65    ):
		print("Eligible")
	else:
		print("Not Eligible")
else:
	if ( age>=60):
		print("Eligible")
	else:
		print("Not Eligible")
		
12.1.3. Writing a program using logical "and"
07:30
Write a program to understand the logical and operator. Take three integers as input from the user using input() function. The program should print True if a is 6 and b is 6 and c is not 6, otherwise it should print False.

Sample Input and Output 1:
a: 6
b: 6
c: 1
True
Sample Input and Output 2:
a: 2
b: 3
c: 5
False

# write your code here
a = int(input("a: "))
b = int(input("b: "))
c = int(input("c: "))

if a==6 and b==6 and c!=6 : #write the condition
	print('True')
else:
	print('False')


12.1.4. Using Logical "or"
03:44
Write a program to understand the logical or operator. Take two integers a and b as inputs from the console using input() function. The program should print True if either of the inputs is 6, their sum is 6, or their difference is 6, Otherwise it should print False.

Sample Input and Output1:
a: 59
b: 6
True

Sample Input and Output2:
a: 30
b: 30
False

a = int(input("a: "))
b = int(input("b: "))
c=a+b
d=a-b
# complete the code
if a==6 or b==6 or c==6 or d==6    :
	print("True")
else:
	print("False")
	
12.1.5. Using Logical "not"
02:30
The logical not operator negates the boolean operand given to it. E.g. not True is False. Similarly, not(a and b) is the expression which indicates True, only when both a and b are not True

Write a program to understand the logical not operator. The program should print Weekend if the day is either SAT or SUN, otherwise it should print Not Weekend. Take the input day from the user.

Sample Input and Output1:
Enter day: SAT
Weekend
Sample Input and Output2:
Enter day: MON
Not Weekend
Hint: Consider the days of the week are represented as MON, TUE, WED, THU, FRI, SAT, SUN

# Program to illustrate logical not
a = input("Enter day: ")

if a=="SAT" or a=="SUN":
	print("Weekend")
else:
	print("Not Weekend")
	
Membership Operators
12.2.1. The membership operators
06:14
The membership operators in Python are used to test the presence of an operand in a String, List, Tuple, etc. The result of this operator is a Boolean value (either True or False).

The membership operators in Python are:

in : Result is True if the left hand side operand exists in the right hand side operand.

Let us consider a simple example:
's' in "Python" # The result is False. 
not in: Result is True if the left hand side operand does not exist in the right hand side operand.

Let's consider a simple example:
's' not in "Python"    # The result is True.  

The right hand operand can be a string, list, tuple, set or dictionary.

The left-hand side operand should be a single element of the right-hand side object.

For strings, the Left Hand Side (LHS) can be any string. If this string exists in the RHS string, then True is returned. Otherwise False is returned.

For all other data types (Lists, Tuples, Sets, Dictionaries, etc.) the LHS should be a single element.

Let's consider an example for strings:

'am' in 'I am working'
will return True

'am' not in 'I am working'
will return False

'not' in 'I am working' 
will return False

'Hot' not in 'I am working'
will return True

"" in 'I am working'
will return True because empty strings are always considered to be a substring of any string

Let's consider an example for list:

1 in [9,7,5,3,1,2,4]
returns True

55 not in [1,2,3,4,5,67]
will return True

'code' in ['code', 'is', 'life']
will return True

'Life' in  ['code', 'is', 'life']
will return False

For tuples and sets, the example is similar to that of list

Let's consider an example for dictionary:

For dictionary the in operator checks existence of the key.

basket = {'apple':20, 'orange':30, 'apple':10, 'pear':15, 'banana':25}

'apple' in basket
returns True

'grape' in basket 
returns False


12.2.2. Membership Operators - an Overview
04:27
Take two strings as input from the console using input() function. Write a program using membership operators to check whether the given second string is present in the first string or not. Print the result of the two input strings to the console, as shown in the example.

Sample Input and Output1:
str1: Hello World Welcome To Python Programming
str2: Pro
Pro in Hello World Welcome To Python Programming: True

Sample Input and Output2:
str1: Regular Expression
str2: advanced
advanced in Regular Expression: False
Follow the instructions and write the code in the space provided

str1 = input("str1: ")
str2 = input("str2: ")

print(f"{str2} in {str1} :",str2 in str1)

12.2.3. Writing example using Membership operator in
01:06
Take two strings as input from the console using input() function. For each membership operator in and not in, print to the console, the result of the two input strings as shown in the example.

Sample Input and Output:
str1: Hello World
str2: worlds
worlds in Hello World is: False
worlds not in Hello World is: True

# Program to illustrate in and not in for strings
str1 = input("str1: ")
substr = input("str2: ")

# check whether substr in str1 and print the result
print(substr, "in", str1, "is:", substr in str1)

#check whether substr not in str1 and print the result
print(substr, "not in", str1, "is:",substr not in str1       )

12.2.4. Write an example using Membership operator not in
08:31
Let's write a simple program using the membership operator in and not in.

The below program has a predefined list. Take an input element from the user to check whether the given element is present in the list or not. Print the result as shown in the example.

Sample Input and Output:
['A', '123', 'Ramana', [1, 2], 34.56, '55']
element: A
A in ['A', '123', 'Ramana', [1, 2], 34.56, '55'] is: True
A not in ['A', '123', 'Ramana', [1, 2], 34.56, '55'] is: False

# Program to illustrate membership operators
L1 = ['A', '123', 'Ramana', [1, 2], 34.56, '55']
# for 34.56 returns False as output because, the input() takes the input as string.

# print L1
print(L1)
# take input for element
e=input("element: ")
# check whether the element is present in L1 and print the result
print(e, "in", L1 ,"is:",e in L1 )
# check whether the element is not present in L1 and print the result
print(e, "not in", L1, "is:",e not in L1 )




