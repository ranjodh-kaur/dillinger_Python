_______
# Unit 1 - Lesson 1
____

##### 1.1.1. What is a computer programming language?

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

##### 1.1.2. The genesis of Python

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

##### 1.1.3. Python Program Life Cycle

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

##### 1.1.4. Difference between Compiler and Interpreter

|Compiler|	Interpreter|
|----|-----|
|Compiler takes entire program as input|	Interpreter takes single instruction as input|
|Intermediate object code is generated|	No Intermediate object code is generated|
|Conditional control statements execute faster|	Conditional control statements are slower in execution|
|Memory Requirement is More(Since Object code is generated)|	Memory Requirement is Less|
|Program need not be compiled every time|	Every time higher level program is converted into lower level program|
|Errors are displayed after entire program is checked|	Errors are displayed for every instruction interpreted (if any)|
|Example : C compiler|	Example : Python|

##### 1.1.5. High level language categories

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

##### 1.1.8. Other usages of print function

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

##### 1.1.10. Features of Python

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
##### Types of Errors

##### 2.1.1. Syntax Error

An error in programming is generally a bug in the code introduced by the developer. There are generally three types of errors Syntax, Logical, and Runtime. To correct these known errors, exception-handling mechanisms are used.

Let's understand about Syntax Errors: These errors are mistakes that happen when there is an incorrect format in the code. These programs are not executed as the compiler of the program raises the errors that need to be corrected. Compiler identifies the line of error and provides an error message.

**Common Python syntax errors are:**
1. Missing a required keyword.
2. Missing symbol, such as a colon or comma.
3. Misspelling a keyword.
4. Wrong indentation.

##### 2.1.2. Logical Errors

**Logical Errors:** These are also known as semantic errors and are tough to identify. These errors occur when a program compiles and runs but doesn’t produce the expected output. They are often due to incorrect logic or misuse of a language’s syntax.

**Common Python logical errors are:**
1. Usage of the wrong variable name.
2. Indentation of a block to the wrong level.
3. A boolean logic gone wrong.
4. Integer division instead of floating-point division.
5. Working on operator precedence in a wrong way.

##### 2.1.3. RunTime Errors
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
##### 3.1.1. Understanding Python Comments

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

##### 3.1.3. Understanding Docstring in Python

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

##### 3.2.1. Understanding Identifiers in Python

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
