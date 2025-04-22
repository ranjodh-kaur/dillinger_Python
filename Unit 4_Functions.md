**Basics of functions in Python** with examples:

---

##  What is a Function?
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


###  Types of Arguments

1. **Positional Arguments** (Order matters)
2. **Keyword Arguments** (Use names)
   ```python
   def display(name, age):
       print(name, age)

   display(age=25, name="Ravi")  # Keyword
   ```
3. **Default Arguments**
   ```python
   def greet(name="Guest"):
       print("Hello", name)

   greet()  # Output: Hello Guest
   ```
4. **Variable-Length Arguments**
   - `*args` for multiple positional arguments
   - `**kwargs` for multiple keyword arguments

   ```python
   def total(*numbers):
       print(sum(numbers))

   total(1, 2, 3, 4)  # Output: 10
   ```

---

 **Types of Arguments in Python Functions**—with **easy explanations and examples**.

---

## 🔹 1. **Positional Arguments**
These are the most common type. The order **matters** when passing values.

```python
def greet(name, age):
    print(f"Hello {name}, you are {age} years old.")

greet("Ravi", 25)  # Correct
# greet(25, "Ravi")  # Incorrect meaning
```

> The arguments are matched **position by position**.

---

## 🔹 2. **Keyword Arguments**
You use the **parameter name explicitly** while calling the function.

```python
def greet(name, age):
    print(f"Hello {name}, you are {age} years old.")

greet(age=25, name="Ravi")  # Order doesn't matter here
```



---

## 🔹 3. **Default Arguments**
You assign a **default value** to a parameter in case it's not passed.

```python
def greet(name, city="Delhi"):
    print(f"Hello {name}, from {city}.")

greet("Meena")             # Uses default city
greet("Arjun", "Chennai")  # Overrides default
```

> 💡 Always place default arguments **after** required ones.

---

## 🔹 4. **Variable-Length Arguments**
Used when the number of arguments is **not fixed**.

### 🟢 `*args` → For **Non-Keyword** Variable Arguments (like a tuple)
```python
def add_numbers(*nums):
    total = sum(nums)
    print("Sum:", total)

add_numbers(10, 20)
add_numbers(1, 2, 3, 4, 5)
```

### 🟢 `**kwargs` → For **Keyword** Variable Arguments (like a dictionary)
```python
def print_details(**info):
    for key, value in info.items():
        print(f"{key}: {value}")

print_details(name="Ravi", age=25, city="Mumbai")
```

> 🔁 `*args` collects extra **positional** arguments,  
> 🔁 `**kwargs` collects extra **keyword** arguments.

---

## Summary Table

| Argument Type     | Syntax         | Use When...                            |
|-------------------|----------------|----------------------------------------|
| Positional        | `f(x, y)`      | You know the exact order               |
| Keyword           | `f(x=10, y=20)`| You want to be explicit or reorder     |
| Default           | `def f(x=0)`   | You want optional parameters           |
| Variable Length   | `*args` / `**kwargs` | You want to handle many arguments |

---



____

### ⛏️ Scope of Variables

- **Local**: Defined inside the function, used only there.
- **Global**: Defined outside the function, accessible anywhere.

---

### 🧪 Example Putting It All Together

```python
def calculator(a, b, operation="add"):
    if operation == "add":
        return a + b
    elif operation == "subtract":
        return a - b
    else:
        return "Invalid operation"

print(calculator(10, 5))               # 15
print(calculator(10, 5, "subtract"))   # 5
```

---


---

## 🔹 1. **Lambda Functions (Anonymous Functions)**

A **lambda** function is a small, one-line function **without a name**.

### 🔸 Syntax:
```python
lambda arguments: expression
```

### 🔸 Example:
```python
square = lambda x: x * x
print(square(5))  # Output: 25
```

### 🔸 Use Case:
Often used when you need a short function just once, especially with `map()`, `filter()`, or `sorted()`.

```python
nums = [1, 2, 3, 4]
squares = list(map(lambda x: x ** 2, nums))
print(squares)  # Output: [1, 4, 9, 16]
```

---

## 🔹 2. **Recursion**

A function that **calls itself** is called a recursive function.

### 🔸 Example: Factorial
```python
def factorial(n):
    if n == 0:
        return 1
    else:
        return n * factorial(n - 1)

print(factorial(5))  # Output: 120
```

### 🔸 Note:
Be careful! Every recursion needs a **base case** to stop. Without it, your program will crash.

---

## 🔹 3. **Nested Functions**

You can define a function **inside another function**.

### 🔸 Example:
```python
def outer():
    print("Inside outer function")

    def inner():
        print("Inside inner function")

    inner()

outer()
```

---

## 🔹 4. **The `pass` Keyword in Functions**

If you want to define a function but don’t want to write the logic yet:

```python
def to_be_defined_later():
    pass
```

---

## 🔹 5. **`*args` and `**kwargs` Recap**

These let you pass **multiple arguments** to a function.

```python
def show(*args, **kwargs):
    print("Args:", args)
    print("Kwargs:", kwargs)

show(10, 20, name="Arjun", age=25)
```

### Output:
```
Args: (10, 20)
Kwargs: {'name': 'Arjun', 'age': 25}
```

---

## 🔹 6. **Functions as First-Class Citizens**

Functions in Python can be:
- Assigned to a variable
- Passed as an argument
- Returned from another function

### 🔸 Example:
```python
def greet(name):
    return f"Hello, {name}"

def call_func(func, value):
    return func(value)

print(call_func(greet, "Krishna"))  # Output: Hello, Krishna
```

---

---

##  Mini Quiz (Basics of Functions)

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
 **real-world examples and practice questions** 
---

## ✅ **Example 1: Calculator Using Functions**
```python
def add(a, b):
    return a + b

def subtract(a, b):
    return a - b

def multiply(a, b):
    return a * b

def divide(a, b):
    if b == 0:
        return "Cannot divide by zero!"
    return a / b

# Usage
print("Sum:", add(10, 5))
print("Difference:", subtract(10, 5))
print("Product:", multiply(10, 5))
print("Quotient:", divide(10, 0))
```

---

## ✅ **Example 2: Count Vowels in a String**
```python
def count_vowels(text):
    vowels = 'aeiouAEIOU'
    count = 0
    for ch in text:
        if ch in vowels:
            count += 1
    return count

print(count_vowels("Hello World"))  # Output: 3
```

---

## ✅ **Example 3: Check Prime Number**
```python
def is_prime(n):
    if n <= 1:
        return False
    for i in range(2, int(n**0.5) + 1):
        if n % i == 0:
            return False
    return True

print(is_prime(7))  # Output: True
```

---

## ✅ **Example 4: Greet Multiple People using `*args`**
```python
def greet_all(*names):
    for name in names:
        print(f"Hello, {name}!")

greet_all("Ravi", "Meena", "Arjun")
```

---

## ✅ **Example 5: Use of `lambda` in Sorting**
```python
students = [("Arjun", 90), ("Meena", 85), ("Ravi", 92)]
students.sort(key=lambda x: x[1])
print(students)  # Sorted by marks
```

---

## Practice Questions for You

Try writing the following programs:

1. **Function to reverse a string.**
2. **Function that takes a list and returns the sum of even numbers.**
3. **Recursive function to compute Fibonacci sequence.**
4. **Function to check whether a number is a palindrome.**
5. **Use `lambda` and `filter` to get only odd numbers from a list.**

---


