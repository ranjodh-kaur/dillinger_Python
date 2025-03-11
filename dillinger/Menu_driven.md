#### Menu driven program like: Design a menu driven code that does the following: 
 -	If ‘1’ is entered, must be able to perform 'task1' 
 -	If ‘2’ is entered, must be able to perform 'task2'
 -	If any other integer is entered, code must be able to terminate with a suitable message. 
________________________


```python
def task1():
    print("Task 1 is being performed...")

def task2():
    print("Task 2 is being performed...")

while True:
    print("\nMenu:")
    print("1. Perform Task 1")
    print("2. Perform Task 2")
    print("Enter any other number to exit.")

    choice = int(input("Enter your choice: "))

    if choice == 1:
        task1()
    elif choice == 2:
        task2()
    else:
        print("Invalid choice! Exiting the program.")
        break
```

____


---

### **1️⃣ Menu-Driven Calculator**
```python
def add(a, b):
    return a + b

def subtract(a, b):
    return a - b

def multiply(a, b):
    return a * b

def divide(a, b):
    return a / b if b != 0 else "Cannot divide by zero"

while True:
    print("\nMenu:")
    print("1. Addition")
    print("2. Subtraction")
    print("3. Multiplication")
    print("4. Division")
    print("5. Exit")

    choice = int(input("Enter your choice: "))

    if choice in [1, 2, 3, 4]:
        num1 = float(input("Enter first number: "))
        num2 = float(input("Enter second number: "))

        if choice == 1:
            print("Result:", add(num1, num2))
        elif choice == 2:
            print("Result:", subtract(num1, num2))
        elif choice == 3:
            print("Result:", multiply(num1, num2))
        elif choice == 4:
            print("Result:", divide(num1, num2))
    elif choice == 5:
        print("Exiting the program. Goodbye!")
        break
    else:
        print("Invalid choice! Please try again.")
```

---

### **2️⃣ Menu-Driven Even/Odd Checker**
```python
while True:
    print("\nMenu:")
    print("1. Check Even or Odd")
    print("2. Exit")

    choice = int(input("Enter your choice: "))

    if choice == 1:
        num = int(input("Enter a number: "))
        if num % 2 == 0:
            print(f"{num} is Even")
        else:
            print(f"{num} is Odd")
    elif choice == 2:
        print("Exiting the program.")
        break
    else:
        print("Invalid choice! Please enter 1 or 2.")
```

---

### **3️⃣ Menu-Driven String Operations**
```python
while True:
    print("\nMenu:")
    print("1. Convert to Uppercase")
    print("2. Convert to Lowercase")
    print("3. Reverse String")
    print("4. Exit")

    choice = int(input("Enter your choice: "))

    if choice in [1, 2, 3]:
        text = input("Enter a string: ")

        if choice == 1:
            print("Uppercase:", text.upper())
        elif choice == 2:
            print("Lowercase:", text.lower())
        elif choice == 3:
            print("Reversed:", text[::-1])
    elif choice == 4:
        print("Exiting the program.")
        break
    else:
        print("Invalid choice! Please try again.")
```

---

### **4️⃣ Menu-Driven Factorial and Fibonacci**
```python
import math

def factorial(n):
    return math.factorial(n)

def fibonacci(n):
    fib = [0, 1]
    for i in range(2, n):
        fib.append(fib[-1] + fib[-2])
    return fib[:n]

while True:
    print("\nMenu:")
    print("1. Calculate Factorial")
    print("2. Generate Fibonacci Series")
    print("3. Exit")

    choice = int(input("Enter your choice: "))

    if choice == 1:
        num = int(input("Enter a number: "))
        print("Factorial:", factorial(num))
    elif choice == 2:
        num = int(input("Enter the number of Fibonacci terms: "))
        print("Fibonacci Series:", fibonacci(num))
    elif choice == 3:
        print("Exiting the program.")
        break
    else:
        print("Invalid choice! Please enter a valid option.")
```

---

### **5️⃣ Menu-Driven Student Management System**
```python
students = {}

while True:
    print("\nMenu:")
    print("1. Add Student")
    print("2. Display Students")
    print("3. Search Student")
    print("4. Exit")

    choice = int(input("Enter your choice: "))

    if choice == 1:
        roll_no = input("Enter Roll Number: ")
        name = input("Enter Student Name: ")
        students[roll_no] = name
        print("Student added successfully!")

    elif choice == 2:
        if students:
            print("\nStudent List:")
            for roll, name in students.items():
                print(f"Roll No: {roll}, Name: {name}")
        else:
            print("No students found!")

    elif choice == 3:
        roll_no = input("Enter Roll Number to Search: ")
        if roll_no in students:
            print(f"Student Found: {students[roll_no]}")
        else:
            print("Student not found!")

    elif choice == 4:
        print("Exiting the program.")
        break

    else:
        print("Invalid choice! Please enter a valid option.")
```

---

### **6️⃣ Menu-Driven Temperature Converter**
```python
def celsius_to_fahrenheit(c):
    return (c * 9/5) + 32

def fahrenheit_to_celsius(f):
    return (f - 32) * 5/9

while True:
    print("\nMenu:")
    print("1. Convert Celsius to Fahrenheit")
    print("2. Convert Fahrenheit to Celsius")
    print("3. Exit")

    choice = int(input("Enter your choice: "))

    if choice == 1:
        celsius = float(input("Enter temperature in Celsius: "))
        print("Temperature in Fahrenheit:", celsius_to_fahrenheit(celsius))

    elif choice == 2:
        fahrenheit = float(input("Enter temperature in Fahrenheit: "))
        print("Temperature in Celsius:", fahrenheit_to_celsius(fahrenheit))

    elif choice == 3:
        print("Exiting the program.")
        break

    else:
        print("Invalid choice! Please enter a valid option.")
```


---

### **7️⃣ Menu-Driven Prime Number Operations**
```python
def is_prime(n):
    if n < 2:
        return False
    for i in range(2, int(n ** 0.5) + 1):
        if n % i == 0:
            return False
    return True

def prime_numbers(n):
    primes = [x for x in range(2, n+1) if is_prime(x)]
    return primes

while True:
    print("\nMenu:")
    print("1. Check if a number is prime")
    print("2. Display prime numbers up to N")
    print("3. Exit")

    choice = int(input("Enter your choice: "))

    if choice == 1:
        num = int(input("Enter a number: "))
        if is_prime(num):
            print(f"{num} is a Prime number.")
        else:
            print(f"{num} is NOT a Prime number.")
    elif choice == 2:
        num = int(input("Enter the range (N): "))
        print("Prime numbers:", prime_numbers(num))
    elif choice == 3:
        print("Exiting the program.")
        break
    else:
        print("Invalid choice! Please try again.")
```

---

### **8️⃣Menu-Driven Stack Implementation**
```python
stack = []

while True:
    print("\nMenu:")
    print("1. Push to Stack")
    print("2. Pop from Stack")
    print("3. Display Stack")
    print("4. Exit")

    choice = int(input("Enter your choice: "))

    if choice == 1:
        element = input("Enter element to push: ")
        stack.append(element)
        print(f"{element} pushed to stack.")
    elif choice == 2:
        if stack:
            print(f"Popped element: {stack.pop()}")
        else:
            print("Stack is empty!")
    elif choice == 3:
        print("Stack:", stack)
    elif choice == 4:
        print("Exiting the program.")
        break
    else:
        print("Invalid choice! Please enter a valid option.")
```

---

### **9️⃣ Menu-Driven Contact Book**
```python
contacts = {}

while True:
    print("\nMenu:")
    print("1. Add Contact")
    print("2. View Contact")
    print("3. Display All Contacts")
    print("4. Exit")

    choice = int(input("Enter your choice: "))

    if choice == 1:
        name = input("Enter Name: ")
        phone = input("Enter Phone Number: ")
        contacts[name] = phone
        print("Contact added successfully!")
    elif choice == 2:
        name = input("Enter Name to search: ")
        print(f"Phone: {contacts.get(name, 'Contact not found!')}")
    elif choice == 3:
        print("\nContacts List:")
        for name, phone in contacts.items():
            print(f"{name}: {phone}")
    elif choice == 4:
        print("Exiting the program.")
        break
    else:
        print("Invalid choice! Please enter a valid option.")
```

---

### **️🔟  Menu-Driven Bank Account System**
```python
balance = 0

while True:
    print("\nMenu:")
    print("1. Deposit Money")
    print("2. Withdraw Money")
    print("3. Check Balance")
    print("4. Exit")

    choice = int(input("Enter your choice: "))

    if choice == 1:
        amount = float(input("Enter deposit amount: "))
        balance += amount
        print(f"Deposited: ${amount}")
    elif choice == 2:
        amount = float(input("Enter withdrawal amount: "))
        if amount <= balance:
            balance -= amount
            print(f"Withdrawn: ${amount}")
        else:
            print("Insufficient balance!")
    elif choice == 3:
        print(f"Current Balance: ${balance}")
    elif choice == 4:
        print("Exiting the program.")
        break
    else:
        print("Invalid choice! Please enter a valid option.")
```

---

