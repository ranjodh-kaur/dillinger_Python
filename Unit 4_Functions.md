**Basics of functions in Python** with examples:

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


### 🧮 Types of Arguments

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

