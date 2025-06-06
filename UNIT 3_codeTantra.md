___________
# UNIT 3 (Lesson 1)
___________

#### 36.1.1. Introduction to Strings
Strings in python are represented with prefixing and suffixing the characters with quotation marks (either single quotes (') or double quotes (")).
- Characters in a string are accessed using an index which is an integer (either positive or negative).
- It starts from 0 to n-1, where n is the number of characters in a string.
- Strings are immutable which means contents cannot be changed once they are created.

The function input() in python is a string by default.


Write a code snippet that prompts the user to input a string using the input() function and print the entered string as shown in the sample test case.

**Sample Input and Output:**

````
str: Strings in Python are immutable

Strings in Python are immutable
````

````python
str=input("str: ")
print(str)


````

#### 36.2.1. Operations of Strings

In Python, there are 5 fundamental operations which can be performed on strings:
- Indexing
- Slicing
- Concatenation
- Repetition
- Membership
  
**Indexing:** To access a specific character from a string, we use its position called Index which is enclosed within square brackets[]. Index value always starts with 0. Python has two types of indexing:
-  Positive Indexing: It begins from the first character of a string, starting with 0.
- Negative Indexing: It begins from the last character of a string, starting with -1.

````
Consider the below example:
a = "HELLO"
print(a[0])     # Result: 'H'
print(a[-1])    # Result 'O'
````

Here, At index '0', the character 'H' is present, so Indexing starts from the left and increments to the right. At index '-1', the character 'O' is present, so Indexing starts from the right and increments to the left.

You're required to create a program that takes a string input from the user. Once the input is taken, perform the following actions:
1. Display the entire string.
2. Prints the second character of string from the beginning.
3. Prints the second character of string from the end.

Sample Input and Output:
````
String: Python Programming
Python Programming
Second character from first: y
Second character from end: n
````

````python
# Prompt the user to enter a string
str=input("String: ")
# Print entire string
print(str) 

# Print second character of string from beginning
print("Second character from first:", str[1] )

# Print second character of string from end 
print("Second character from end:",str[-2]  )
````

#### 36.2.2. Understanding Slicing Operator

Python provides many ways to extract a part of a string using a concept called Slicing. It is used to extract a specific part of a string using a startIndex and an endIndex.

The syntax for using the slice operation on a string is:
```` [startIndex : endIndex : step] 		````
where,
- startIndex is the index where you want to start extracting.
- endIndex is the index where you want to stop extracting (not included).
 - step is the interval between characters to include in the slice.

Key considerations to keep in mind when performing slicing operations:
- If you omit the startIndex, the slice starts from the beginning (index 0).
- If you omit the endIndex, the slice goes until the end of the string.
- Positive step means moving from left to right, incrementing the index by step.
- Negative step means moving from right to left, decrementing the index by step.
- startIndex, endIndex and step are optional parameters.


#### 36.2.3. Different examples on Slicing 

Let's consider below examples to understand about slicing briefly:

````Assume that a = "Python",````

Example1 - Slicing from a starting index to the end of the string:

````print(a[0:])      # Result: Python````

Example2 - Slicing from the beginning to an ending index (exclusive):

````print(a[:6])      # Result: Python````

Example3 - Specifying both start and end indexes:

````print(a[0:4])     # Result: Pyth````
This code snippet extracts a sub-string from a specified start index to the end index of the string.

Example4 - Using step for traversal:

````print(a[::1])     # Result: Python ````
````print(a[::-1])    # Result: nohtyP ````

Example5 - Using step with negative value for reversed traversal:

````print(a[-1::-3])   # Result: nt ````
````print(a[4:1:-1])   # Result: oht ````
````print(a[2:5:-1])   # Result: ' ' ````

In the last case, when trying to go from index 2 to 5 in reverse, it results an empty string because the direction and range conflicts.

Given a string strange = "ABCDEFGHIJKL", predict the result when result = strange[-9:-4] ? 

````Answer: "DEFGH"````

#### 36.2.4. Write a program to print a string after removing first and last characters

Write a program to take string as input from the user using input() function. Remove first and last characters of given string.

Print the result as shown in the sample test case.

Sample Input and Output:
````
Input str: Python
output: ytho
````

````python
str=(input("str: "))
l=len(str)
print("output:",str[1:l-1])
````

#### 36.2.5. Concatenation of strings

Concatenation of strings refers to the process of linking or combining two strings into a single string. The (+) operator joins the text on both sides of the operator.

**Write a program to take two strings as input from the console using input() function. Concatenate those two strings and print the result as shown in the sample test case.**

Sample Input and Output:
````
str1: Python
str2: Jython
Python Jython
Hint: Use (" ") for providing space between the two concatenated strings.
````
````python
str1=(input("str1: "))
str2=(input("str2: "))
print(str1+ " "+ str2)
````

#### 36.2.6. Program to perform concatenation on two strings.

Write a program that takes two input strings str1 and str2 and returns the result by concatenating them in the order str1str2str2str1.

Print the result as shown in the sample test case.

````
Sample Input and Output:
str1: Code
str2: Tantra
result: CodeTantraTantraCode
````

````python

# Type your content here...
str1=(input("str1: "))
str2=(input("str2: "))
print("result:",str1+str2+str2+str1)
````

#### 36.2.7. Program to remove a character from string based on integer value given by the user.

Write a program to remove a character from a string based on integer value given by the user. Treat the input as an index of a string.

Print the result as shown in the sample test cases.

Sample Input and Output 1:
````
str: Python Programming
num: 9
Python Prgramming
````

Sample Input and Output 2:
````
str: Strings
num: 10
num should be positive, less than the length of str
````
````python
# Type your content here...
str=(input("str: "))
num=(int(input("num: ")))
if num>len(str):
	print("num should be positive, less than the length of str")
else:
	print("output:",str[0:num]+str[num+1:])
````
 
#### 36.2.8. Program to print the concatenated string by excluding first character.

Write a program to take two strings as input from the user. Concatenate those two strings by removing the first character from both and print the result as shown in the sample test case.


Sample Input and Output 1:
````
str1: Python
str2: Java
output: ythonava
````
````
Sample Input and Output 2:
str1: a
str2: b
null
````

````python
# Type your code here...
str1=(input("str1: "))
str2=(input("str2: "))
if len(str1) > 1 and len(str2) > 1:
	print("output:", str1[1:] + str2[1:])
else:
	print("null")
````

#### 36.2.9. Program to swap first and last characters of given string and display the result

Write a program to take a string as input from the user. Swap the first and last characters of the given string. Print the resultant string as shown in the sample test case.

Follow the below constraints while writing the program:

- If the length of the string is 1 then print the input string as it is.
- If the length of the string is 0 (zero) then print null as output.


Sample Input and Output 1:
````
Input str: Active
output: ectivA
````

Sample Input and Output 2:
````
Input str: T
output: T
````

````python

# Type your code here...
s=(input("str: "))
l=len(s)
if l ==1:
	print(s)
elif l==0:
	print("null")
else:
	print("output:",s[-1]+s[1:-1]+s[0])
````

#### 36.2.10. Program to print first and last two characters of given string

Write a program to take a string as input from the user. Print the first and last two characters of a string. If the length of the string is less than 3 then print the input string as it is.

Print the result as shown in the sample test case.


Sample Input and Output 1:
````
input: Code Tantra
output: Cora
````

Sample Input and Output 2:
````
input: hi
output: hi
````
````python
# Type Content here...
str=input("input: ")
if len(str)<3:
	print("output:",str)
else:
	print('output:',str[0:2]+str[-2:])
````

 #### 36.2.11. Understanding Membership Operator

Membership Operators in and not in are used to check whether a certain element exits within a sequence such as string, list, tuple or set.
The in operator returns True if the specified element is found in the sequence. Otherwise, it returns False
The not in operator returns True if the specified element is not found in the sequence. Otherwise, it returns False
The results are based on case sensitivity.

Below are the examples which demonstrates the use of in and not in operators:
````python
s = "good morning" 
print("m" in s)           # Result: True
print("a" not in s)       # Result: True 
print("z" in s)           # Result: False
print("good" in s)        # Result: True
print("Morning" in s)     # Result: False
````

Consider the following statements about the string str = "Coding" and select the correct options:

````Answer: print('z' not in str) returns True````

#### 36.2.12. Repetitions of a String

We can use ( * ) operator to repeat a string several times. The format is <string> * <number>. This generates a new string containing the initial string duplicated as many times as indicated by the specified number.

**Example:**
````
a = "Mouse"
print(3 * a)   # Output: MouseMouseMouse 
print(a * 3)   # Output: MouseMouseMouse 
b = 3
print(((b - 2) * 2) * a)   # Output: MouseMouse (repeated 2 times) 
Note: 3 * str is same as str * 3
````

Write a program to input a string from the user. Print the string four times and also print it thrice in reverse as shown in the sample test case.

Sample Input and Output:
````
str: Python
PythonPythonPythonPython
nohtyPnohtyPnohtyP
````
````python
str=input("str: ")
print(4*str)
print(str[-1::-1]*3)
````

#### 36.2.13. Program to print 3 copies of first three characters of a string.

Write a program to take a string as input from the user. If the length of a given string is greater than or equal to 3 then print the first three characters 3 times. If not print the string as it is.

Print the result as shown in the sample test cases.

Sample Input and Output 1:
````
str: Python
result: PytPytPyt
````

Sample Input and Output 2:
````
str: Hi
result: Hi
````

````python
# Type your content here...
str=input("str: ")
if len(str)>=3:
	print("result:",str[0:3]*3)
else:
	print("result:",str)
````

#### 36.2.14. Program to print a given string which repeats 'n' times.

Write a program to take two inputs, string str and integer n from the user and print the given string str which repeats n times.

Print the result as shown in the sample test case.


Sample Input and Output:
````
str: Python
num: 5
result: PythonPythonPythonPythonPython
````
````python
# Type your content here...
str=input("str: ")
n=int(input("num: "))
print("result:",str*n)
````

#### 36.2.15. Program to repeat first n characters of the given string n times

Write a program to read a string str, an integer n and print the first n characters of the string which repeats n times. Here integer value n works like a index of a string.

Assumption:

- Index n is always positive and less than the length of the string.
- If user gives a negative index value print the error message as shown in the Sample test case 2.
- Print the result to the console as shown in the sample test cases.


Sample Input and Output 1:
````
str: python
num: 5
result: pythopythopythopythopytho
````

Sample Input and Output 2:
````
str: Java
num: -1
num should be positive, less than length of str
````

````python
# Type your code here...
str=input("str: ")
n=int(input("num: "))
if n>0 and n<len(str):
	print("result:",str[0:n]*n)
else:
	print("num should be positive, less than length of str")

````

#### 36.2.16. Understanding String Immutability

Python strings are "immutable". Means, we can't reassign or change a value of a string once it is created. The [ ] operator cannot be used on the left side of an assignment.

Consider the below example:
````python
str = "Python"
str[0] = 'J'    # Attempt to change the 0th index 'P' with 'J'
````
Due to string immutability, this results a TypeError: 'str' object does not support item assignment.


However, we can create a new string:
````python
newstr = "J" + str[1:]
print(newstr)   # Output: "Jython"
Deleting a particular character in a string is not possible. We can delete the entire string by using del.
del str[0]      # Raises TypeError: 'str' object doesn't support item deletion
del str
print(str)      # Raises NameError: name 'str' is not defined
````
After deleting a string variable, trying to access it leads to NameError due to the variable's deletion.

In Python, why does attempting to delete a character at a specific index within a string result in an error?

````Answer: Deleting characters within strings violates the immutability principle of strings.````

___________
# UNIT 3 (Lesson 2)
___________
#### Built-in String Methods
#### 37.1.1. Functions of String Data Type

Python provides the following built-in string methods (operations that can be performed with string objects).
````python
Syntax to execute these methods is: stringobject.methodname()
````

Given an input string ````a = "hello python"````, now understand the working principles of the following methods:

1) capitalize() - Capitalizes first letter of a string.

````print(a.capitalize())    # Result: Hello python````

2) upper() - Converts the string to uppercase.
````
print(a.upper())         # Result: 'HELLO PYTHON'
````
4) lower() - Converts the string to lowercase.

````print(a.lower())         # Result: 'hello python'````

5) title() - Converts the string to title case. i.e., first characters of all the words of string are capitalized.

````print(a.title())         # Result: 'Hello Python'````

6) swapcase() - Swap the case of characters. i.e., lowercase into uppercase and vice versa.

````print(a.swapcase())      # Result: 'HELLO PYTHON'````

7) split() function returns a list of words separated by space.

````print(a.split())         # Result: ['hello', 'python']````

8) center(width,"fillchar") Center the string within a specified width using a fill character. Observe the below example:

````print(a.center(20, '*'))   # Result: '****hello python****'````

Here, width is 20 and string length is 12, so now we need to fill the remaining width(20 - 12 = 8) with '*' special character.

Select all the correct statements among the provided options.

````python
Answer: 
In Python, we can convert strings of Uppercase letters into lower case and lower case to upper case using swapcase() method.

Answer: 
print('abcpyxyzpython', 3, 10) - Outputs: abcpyxyzpython 3 10.
````

#### 37.1.2. Methods Of Strings - count(), replace(), join()

Consider an input string 
````python
a = "hello happy birthday happy birthday life is happy",
````
 let's understand the working principles of the following methods:

8) count(substring) - Returns the count of occurrences of the substring in a string. If the substring does not exist, it returns zero.
````python
print(a.count('happy'))     # Result: 3 (happy word occurred 3 times)
````

9) replace(old, new) - Replace all occurrences of old substring with new substring. If the old substring does not exist, no modifications will be done.
````python
print(a.replace('happy' ,'joyful'))   # Result: 'hello joyful birthday joyful birthday life is joyful'
````

10) join(iterable) - Concatenate the elements of the iterable using the string as the separator. (“L1” is iterable in the below example.)
````python
b = '.'
L1 = ["www", "codetantra", "com"]
print(b.join(L1))    # Concatenates each item in the list with '.' Result: 'www.codetantra.com'
````

**Write a program to demonstrate string methods using a user input. Follow the instructions provided in the comment lines.**

Print the result as shown in the sample test cases.
````
Test case 1
str: Python is high level language	
PYTHON IS HIGH LEVEL LANGUAGE⏎	
Python Is High Level Language⏎	
['Python', 'is', 'high', 'level', 'language']⏎	
width: 25	
fillchar: %	
Python is high level language⏎	
python is high level language⏎	
Enter a joining character:·@	
P@y@t@h@o@n@·@i@s@·@h@i@g@h@·@l@e@v@e@l@·@l@a@n@g@u@a@g@e⏎	
old substring: high	
new substring: low	
Python is low level language⏎
````

````python
str1 = input("str: ")
# Convert the string to uppercase
print(str1.upper())
# Convert the string to title case
print(str1.title())
# Split the string into a list of words
print(str1.split())
width = int(input("width: "))
fill_char = input("fillchar: ")
# Center align the string with given width and fill character
print(str1.center(width, fill_char))
# Convert the string to lowercase
print(str1.lower())
str2 = input("Enter a joining character: ")
# Join the characters of the string with the given character
print(str2.join(str1))
replace_old = input("old substring: ")
replace_new = input("new substring: ")
# Replace occurrences of old substring with new substring
print(str1.replace(replace_old,replace_new))
````

#### 37.1.3. Methods Of Strings - isupper(), islower(), isalpha(), isalnum()

11) isupper() - Checks if all characters in the string are uppercase or not. If yes returns True, otherwise False.

12) islower() - Checks if all characters in the string are lowercase or not. If yes returns True, otherwise False.

13) isalpha() - Checks if the string contains alphabetic characters only or not. If yes returns True, otherwise False.
Space is not considered as alphabet character, it will fall in the category of special characters.

14) isalnum() - Checks if the string contains alphanumeric characters only or not. If yes returns True, otherwise False.
Characters those are not alphanumeric are: (space) ! # % & ? etc.
Numerals (0-9), alphabets (A-Z, a-z) will fall into the category of alphanumeric characters.

Now, let's understand these methods with small example. Assume there is an string ````python a = "HELLOWORLD123"````. Observe the output:
````python
print(a.isupper())     # Result: True
print(a.islower())     # Result: False
print(a.isalpha())     # Result: False
print(a.isalnum())     # Result: True
````
Select all the correct statements among the provided options.
 
- print("Hello123".isalpha()) returns False.
- str = '123', the below code is correct to convert string into int. print(int(str)) # 123.
- str = "hello world", print(str.isalnum()) returns False.

#### 37.1.4. Methods of Strings - isdigit(), isspace(), istitle()

15) isdigit() - Checks if the string contains only digits or not. If yes returns True, otherwise False.
````python
a = "123hello"
print(a.isdigit())    # Result : False
````

16) isspace() - Checks whether the string contains only spaces or not. If yes returns True, otherwise False.
````python
a = "       "
print(a.isspace())    # Result: True
a = " h "
print(a.isspace())    # Result : False
````

17) istitle() - Checks whether every word of a string starts with upper case letter or not.
````python
a = "Hello Python"
print(a.istitle())    # Result: True
````

Given an incomplete program. Your task is to complete the if conditions which performs specific checks on the input string and display the corresponding messages.

````python
str = input("str: ")
# Complete below condition and check whether string contains only digits or not.
if str.isdigit():
	print("str contains only digits")
else:
	print("str does not contains only digits")

# Complete below condition and check whether string contains only spaces or not.
if str.isspace():
	print("str contains only space")
else:
	print("str does not contains only space")

# Complete below condition and check if the string is in title case or not.
if str.istitle():
	print("str is in title case")
else:
	print("str is not in title case")
````

#### 37.1.5. Escape Sequences in Strings

Escape characters are used to solve the problem of using special characters inside a string declaration. It directs the interpreter to take suitable actions mapped to that character. We denote escape characters with a backslash (\) at the beginning.

Let us discuss escape characters one by one:
````python
\n - Used for providing a new line.
print("hello\npython")      
hello                   # Output
python
````
````python
\\ - Used to represent backslash. It returns one single backslash.
print("hello\\how are you")  
hello\how are you       # Output 
````

````python
\' - Used to print a Single Quote( ' ).
print("It\'s very powerful") 
It's very powerful      # Output
````

````python
\" - Used to represent double Quote( " ).
print("We can represent Strings using \" ") 
We can represent Strings using " # Output
````

````python
 \t is used to provide a tab space.
print("Hello\tPython") 
Hello	Python          # Output
````
Which of the following code will generate the displayed text.
This is a string with a double quote character.

````python
print("This is a string with a double quote character.")
````

#### 37.1.6. Escape Sequences

Escape sequences can sometimes be printed as they are, without being treated as special characters. To achieve this, you can use the repr() function or the r / R prefix.
````python
Example using repr():
str = "Hello\tPython\nPython is very interesting"
print(str)  # will print result as follows
Hello       Python       
Python is very interesting

print(repr(str)) # will print result as follows
'Hello\tPython\nPython is very interesting'

Example using 'r' and 'R':
print(r"Hello\tPython\nPython is very interesting")  # will print result as follows
Hello\tPython\nPython is very interesting

print(R"Hello\tPython\nPython is very interesting") # will print result as follows
Hello\tPython\nPython is very interesting 
````

Which of the following statements about escape sequences in Python is true?
- Escape sequences can be printed as they are, without being interpreted as special characters, by using the repr() function or the r / R prefix.

#### 37.1.7. Methods of Strings - startswith(), endswith(), find(), len(), min(), max()

Consider a string a = "hello python", Let us explore more string methods:

18) startswith(substring) - Checks whether the main string starts with given sub string. If yes it returns True, otherwise False.
````print(a.startswith('h'))  # Result: True````

19) endswith(substring) - Checks whether the string ends with the substring or not.
````print(a.endswith('n'))    # Result: True````

20) find(substring) - Returns the index of the first occurrence of the substring, if it is found, otherwise it returns -1
````print(a.find('py'))       # Result: 6````
````print(a.find('java'))     # Result: -1````

21) len() - Returns the length of the string.
````print(len(a))          # Result: 12````

22) min() - Returns the minimum character in the string
````print(min(a))          # Result: ''````
Here it returns white space because in the given string white space is the minimum of all characters.

23) max() - Returns the maximum character in the string.
````print(max(a))         # Result: y````

Given an incomplete code which demonstrates about string methods. Your task is to fill the necessary parts as instructed in the comment lines.

Print the result as shown in the sample test cases.
````python
str = input("str: ")
start_substring = input("start_substring: ")
end_substring = input("end_substring: ")
search_substring = input("search_substring: ")

print(str.startswith(start_substring)) # Check if the string starts with the given starting substring
print( str.endswith(end_substring) ) # Check if the string ends with the given ending substring
print(str.find(search_substring) ) # Find and display the index of the search substring
print(len(str)  ) # Display length of the main string
print( min(str) ) # Display the minimum character in main string
print( max(str) ) # Display the maximum character in main string
````

#### 37.1.8. Program to enclose the longer string with-in the shorter string and display the result.

Write a program to take two strings of different lengths as input from the user and enclose the longer string with-in the shorter string.

Print the result as shown in the sample test cases.

Sample Input and Output 1:
````
str1: Big Data
str2: Hadoop
HadoopBig DataHadoop
Here, len(Big Data) is 8 and len(Hadoop) is 6 so Big Data is enclosed with Hadoop.
````

Sample Input and Output 2:
````
str1: Django
str2: Django
strings are same length
````

````python
str1 = input("str1: ")
str2 = input("str2: ")

# Calculate the lengths of the input strings
l1 = len(str1)
l2 = len(str2)

# Print strings are equal if the both lengths are equal
if l1==l2:
	print("strings are same length")
	
# If the length of str1 is shorter than the length of str2, print the concatenation
elif l1< l2:
	print(str1+str2+str1)
	
# If the length of str1 is longer than the length of str2, print the concatenation
else:
	print(str2+str1+str2)
	
````

#### 37.1.9. Write a program to find whether a given string starts with 'Python' or not.

Write a program to take string as input from the user and check whether the given input begins with Python or not. If yes, print the input string as it is, otherwise add Python to input string.

Print the result as shown in the sample test cases.

Sample Input and Output 1:
````
str: Python
str is: Python
````

Sample Input and Output 2:
````
str: World
str after adding 'Python': Python World
````
###### Note: Python and python are different.

````python
str = input("str: ")
# write yur code here
if str.startswith("Python"):
    print("str is:",str)
else:
    print("str after adding 'Python':","Python " + str)
````

#### 37.1.10. More String methods

A module is a file containing Python definitions, functions and statements.Standard library of Python is extended as modules. To use modules, we need to import them. After importing a module, we can use its functions and variables in our code. Python offers numerous standard modules. We will learn about modules in detail later.

Syntax:
````python
import module_name
Here we use all functions of the string module.
import string
print(string.punctuation) # Result: !"#$%&'()*+,-./:;<=>?@[\]^_`{|}~
print(string.digits)      # Result: 0123456789
print(string.printable)   # Result: 0123456789abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ!"#$%&'()*+,-./:;<=>?@[\]^_`{|}~
print(string.capwords('hello python')) # Result: Hello Python
print(string.hexdigits)   # Result: 0123456789abcdefABCDEF
print(string.octdigits)   # Result: 01234567
````
For more information on string module refer to: String Modules

Write a program to take string as input from the user and reverse the given string using slicing operator(:).

Hint: Recall the previous lessons.

Sample Input and Output:
````
str: Strings in python are immutable
elbatummi era nohtyp ni sgnirtS
````

````python
# Take a string input form the user
str=input("str: ")
l=len(str)
# Reverse the string using slicing operator
print(str[::-1])
````

#### 37.1.11. Write a program to remove all digit in given string.

Below given is the program to remove all punctuation's in a string and print the result.
````python
import string
punctuations = string.punctuation
result = " "
str = "List - []\n tuple - ()\n Dictionary - {}\n Comment - #\n Multiply - *\n not - !\n and - &\n or - |\n
              format specifier - %\n String - " " $ @ ; : ' / + = "  
for i in str:
	if i not in punctuations:
		result = result + i
print("String after removing all Punctuation's:", result)
````
Here,
We are importing string module to know the list of punctuation's using string.punctuation.
-  Then we compare punctuations in the given string with the string.punctuation module and remove them from the input string and print the resultant string.
-  str variable contains input string.
- for clause to iterate over the list of characters in the input string.
- if condition to check if a punctuation of the input string exists in punctuation variable or not.

Output:
- Set of punctuations in string.punctuation is: !"#$%&'()*+,-./:;<=>?@[\]^_`{|}~
- String after removing all Punctuation's is:  List  
 tuple  
 Dictionary  
 Comment  
 Multiply  
 not  
 and  
 or  
 format specifier  
 String           

Now build a program to take string (combination of characters and digits) as input from the user and remove all the digits from the given string.
````python
# import string module
import string
str = input("str: ")  
result = ""  # Initializing an empty string to store the result

d=string.digits
# Iterate through each character in string (str), and if the character is not a digit, add it to the result.
for i in str:
	if i not in d:
		result = result + i

# Print the result after removing all digits
print("String after removing all digits:", result )
````

#### 37.1.12. Write a program to find number of times a particular sub string appears in a given string.

Write a program to count the number of times the second string occurs in the first string.

Print the result to the console as shown in the sample test case.

Sample Input and Output:
````
str1: Python is easy programming
str2: easy
count: 1
````
````python
str1 = input("str1: ")
str2 = input("str2: ")
print("count:",str1.count(str2)) # print the count count of str2 occured in str1
````

#### 37.1.13. Write a program to print every character of a string twice.

Write a program to print every character of the given input string twice.

Print the result to the console as shown in the sample test case.

Sample Input and Output:
````
str: Lists
result:  LLiissttss
````

````python
str = input("str: ")
r=""
# write your code here to print the every character in the given string twice
print("result:  ",end="")
for x in str:
	# r=r+x*2
	r=r+"".join(x*2)
print(r)
````

#### 37.1.14. Write a program to print half of a given string.

Write a program to calculate the length of the string, If the length is even print the first half of the string, if the length is odd remove the middle character.

Print the second half of the string as shown in the sample test case.

Sample Input and Output 1:
````
str: Python
first half str of even length: Pyt
````

Sample Input and Output 2:
````
str: Hello World
second half str of odd length: World
````

Sample Test Cases
````
Test case 1
str:·Python	
first·half·str·of·even·length:·Pyt⏎	
Test case 2
str:·PythonWorld	
second·half·str·of·odd·length:·World⏎
````

````python
str = input("str: ")

# write your code here
l=len(str)
half=l//2
if l%2==0:
	print("first half str of even length:",str[:half])
else:
	print("second half str of odd length:",str[half+1:])
````

#### 37.1.15. Write a Program to print a character and skip the next character, follow this till the end of string.

Write a program to divide the string into two substrings by taking the alternate characters and print both the strings. Again from these two substrings, make the original string.

- If length is zero then, the program should print 'null'
- If the length is 1 then, the program should print the message on the console as shown in the sample test case 3.
- Print the result as shown in the sample test cases.



Sample Input and Output 1:
````
str: Python
first: Pto
second: yhn
original:  Python
````
Sample Input and Output 2:
````
str: null
first: 
second: 
original:
````
Sample Input and Output 3:
````
str: H
H
first: H
second: 
original:  H
````


#### 37.1.16. Write a program to print each character of a string in incremental order.

Write a program to print each character of a string in incremental order as shown in the sample test cases.

Test case 1

````
str:·Key	
incremental·order:·KKeKey⏎	
````
Test case 2
````
str:·Python	
incremental·order:·PPyPytPythPythoPython
````

#### 37.1.17. Write a program to remove hyphens from a given string.

Take a string as input from the user using input() function. Write a program to remove hyphens from the given string if it contains any hyphens. Print the result as shown in the example

Sample Input and Output:
````
str with hyphens: Python-programming
Pythonprogramming
````
Python provides more builtin modules Let us consider a simple example:
````
str = input("str with hyphens: ")
for i in str.split('-'):
	print(i, end = " ")
````
Here str variable refers a given string.

- 'for clause' to iterate over the number of characters of a string.

- 'split()' used to separate or break the given string based on separator and add the separated data to a string array using a defined separator.

Here our separator is ' - '

- If we are not specifying any separator then it takes 'white space' as default separator.

- The end = ' ' is used to provide space after the end of the statement instead of a new line character.

- If you don't provide end = ' ' in print() statement then all separated strings are printed on new lines one after the other like as below:

- Python
- provides
- more
- builtin
- modules

#### 37.1.18. Program to print ASCII values of the characters within the given range..

isprintable() - This method returns True if all the characters are printable, otherwise False.
The printable characters include alphabets, digits, symbols, punctuation and white space.
 '\n' is not an alphabet character so isprintable() returns False.

ASCII (American Standard Code for Information Interchange) is a character encoding standard that represents characters as numeric codes. Each character is assigned a unique number between 0 and 127 (or 0 to 255 in extended ASCII), allowing computers to represent and manipulate text.
For example, the ASCII code for the letter 'A' is 65.

Write a python program that takes a start and end character as input from the user and displays a table showing the ASCII codes of characters in the given range.
If the input is not a single character, the program should display an error message as shown in the sample test case.

For example, if the user enters 'A' as the start character and 'D' as the end character, the program should output the following:
````
Character   ASCII Code
A           65
B           66
C           67
D           68
````

#### 37.1.19. Write a program to find how many times each character is repeated in a given string.

Take string as input from the console using input() function. Write a program to find how many times each character is repeated in a given string. Print each character in the string in sorted order with a number of times it is repeated as shown in the example.

Sample Input and Output:
````
str: Hello Python!
' '	1
'!'	1
'H'	1
'P'	1
'e'	1
'h'	1
'l'	2
'n'	1
'o'	2
't'	1
'y'	1
[' ', '!', 'H', 'P', 'e', 'h', 'l', 'n', 'o', 't', 'y']
````

#### 37.1.20. Write a program to find how many times a single digit is repeated in a given number.

Write a program to find how many times a single digit is repeated in a given number, and print the result as shown in the example.

Sample Input and Output:
````
str: 11454
1 	 2
4 	 2
5 	 1
````

Note: The output should be printed in the order of the appearance of digits in the given number.


