#### 36.1.1. Introduction to Strings
Strings in python are represented with prefixing and suffixing the characters with quotation marks (either single quotes (') or double quotes (")).
- Characters in a string are accessed using an index which is an integer (either positive or negative).
- It starts from 0 to n-1, where n is the number of characters in a string.
- Strings are immutable which means contents cannot be changed once they are created.

The function input() in python is a string by default.


Write a code snippet that prompts the user to input a string using the input() function and print the entered string as shown in the sample test case.

**Sample Input and Output:**

````str: Strings in Python are immutable````

````Strings in Python are immutable````

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
````python
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
