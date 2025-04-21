**basics of functions in Python** with examples:

---

## 🧠 What is a Function?
A **function** is a **block of reusable code** that performs a specific task.

---

## 🔹 Why Use Functions?
- To **avoid repetition** of code
- To **organize** the code better
- To **reuse** logic across multiple parts of the program

---

## 🔹 Defining a Function
```python
def greet():
    print("Hello, welcome!")
```

- `def` is the keyword used to define a function.
- `greet()` is the function name.
- Code inside the function is **indented**.

---

## 🔹 Calling a Function
```python
greet()   # Output: Hello, welcome!
```

---

## 🔹 Function with Parameters
You can pass values to a function.

```python
def greet(name):
    print("Hello", name)

greet("Alice")   # Output: Hello Alice
```

---

## 🔹 Function with Return Value
Functions can return a value using the `return` keyword.

```python
def add(a, b):
    return a + b

result = add(5, 3)
print(result)    # Output: 8
```

---

## 🔹 Function with Default Parameter
```python
def greet(name="Guest"):
    print("Hello", name)

greet()          # Output: Hello Guest
greet("Ravi")    # Output: Hello Ravi
```

---

## 🔹 Function with Multiple Parameters
```python
def multiply(x, y):
    return x * y

print(multiply(4, 5))  # Output: 20
```

---

## 🔹 Types of Functions
- **Built-in functions**: `print()`, `len()`, `type()`, etc.
- **User-defined functions**: The ones you define using `def`.

---


---

## 🧠 Mini Quiz (Basics of Functions)

**Q1.** What keyword is used to define a function in Python?  
a) function  
b) def  
c) fun  
d) define  

**Q2.** What will this code print?
```python
def say_hello():
    print("Hello!")

say_hello()
```
a) say_hello  
b) Hello!  
c) Error  
d) Nothing  

**Q3.** Which of the following defines a function that returns the square of a number?  
a) `def square(x): print(x * x)`  
b) `def square(x): return x * x`  
c) `def square: return x * x`  
d) `function square(x): return x * x`  

---

## 💻 Coding Challenge

Write a Python function named `is_even()` that:
- Accepts a number as input
- Returns `"Even"` if the number is even
- Returns `"Odd"` if the number is odd

📌 **Sample Output:**
```python
print(is_even(4))  # Output: Even
print(is_even(7))  # Output: Odd
```

---
