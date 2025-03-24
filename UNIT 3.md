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

Given a string strange = "ABCDEFGHIJKL", predict the result when result = strange[-9:-4] ? Answer: "DEFGH"

#### 36.2.4. Write a program to print a string after removing first and last characters

Write a program to take string as input from the user using input() function. Remove first and last characters of given string.

Print the result as shown in the sample test case.

````python
Sample Input and Output:
Input str: Python
output: ytho
````


