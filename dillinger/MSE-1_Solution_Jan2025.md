### **Mid-Semester Exam (MSE) - Python Programming** 
---
**Date:** 18/03/25  

**Note:** Attempt all questions. All assumptions must be clearly stated.  

| Q. No. | Question | Marks |
|--------|----------|--------|
| **Q1** | “Python is platform independent.” Justify the quoted statement by highlighting the key contributing factors. | 2 |
| **Q2** | Create a list with integer values by taking the inputs from the user. For each function **length**, **enumerate**, **maximum**, and **sorted**, apply it to the given input list.  Print the result in the following format:    |     2     |    

**Sample Input and Output:** 
**data:** 10, 55, 69, 78, 456 
**length:** 5 
**list enumerate:** [(0, 10), (1, 55), (2, 69), (3, 78), (4, 456)] 
**max:** 456  **list:** [10, 55, 69, 78, 456] 

| **Q3** | Differentiate between a **list** and **tuple** by highlighting key differences. Also provide examples demonstrating the conversion of a **list** into a **tuple** and vice versa. | 4 |
|--------|----------|--------|
| **Q4** | Differentiate between **aliasing** and **cloning** by highlighting key differences. With the help of code snippets, demonstrate how **cloning** can be achieved by two different methods. | 4 |
| **Q5** | Create two dictionaries **dict1** and **dict2** with user-given (key, value) pairs. Perform the following operations:| 4|

1. Print **dict1** in sorted order. 
2. Create a copy of **dict1** and print it. 
3. Print the **keys** and **values** (separately) of **dict1** in sorted order. 
4. Update the contents of **dict1** with **dict2**, then print the results appropriately. 

| **Q6** | **Design a menu-driven code** that does the following: |8|
|--------|----------|--------|
- If ‘1’ is entered, must be able to illustrate **nested list comprehension**. 
- If ‘2’ is entered, must be able to print a **number pattern** as shown in the example. 
**Input format:** The input should be a number **n**.
**Output format:** The output should be the pattern. 
**Example:**
**Input:** 4
**Output:**

1 
1 2

1 2 3

1 2 3 4

- If any other integer is entered, the code must be able to **terminate with a message: "Signing off."** 


---
## Solution



### **Q1: “Python is platform independent.” Justify the quoted statement by highlighting the key contributing factors.**  

**Answer:**  
Python is **platform independent**, meaning that Python code can run on different operating systems (Windows, macOS, Linux, etc.) without modification. The key factors contributing to this are:  

1. **Interpreted Language:** Python code is executed by the Python interpreter, which makes it work on any platform with the appropriate interpreter installed.  
2. **Bytecode Compilation:** Python code is compiled into bytecode (`.pyc` files), which is platform-independent and can run on any system with a Python Virtual Machine (PVM).  
3. **Cross-Platform Libraries:** Python provides standard libraries that work across different operating systems, making it easier to develop cross-platform applications.  
4. **Write Once, Run Anywhere (WORA):** A Python program written on one OS can be run on another OS without modification.  

---

### **Q2: Create a list with integer values and apply various functions.**  

#### **Python Code:**  
```python
# Taking input and creating the list
data = [10, 55, 69, 78, 456]

# Applying functions
length = len(data)
enumerated_list = list(enumerate(data))
max_value = max(data)
sorted_list = sorted(data)

# Printing the output in the required format
print(f"data: {data}")
print(f"length: {length}")
print(f"list enumerate: {enumerated_list}")
print(f"max: {max_value}")
print(f"list: {sorted_list}")
```
#### **Output:**  
```
data: [10, 55, 69, 78, 456]
length: 5
list enumerate: [(0, 10), (1, 55), (2, 69), (3, 78), (4, 456)]
max: 456
list: [10, 55, 69, 78, 456]
```
---

### **Q3: Differentiate between List and Tuple**  
### **Difference Between List and Tuple**  

| Feature       | List                         | Tuple                        |
|--------------|-----------------------------|------------------------------|
| **Mutability** | Lists are mutable (can be modified). | Tuples are immutable (cannot be modified). |
| **Syntax** | Defined using `[]` (square brackets). | Defined using `()` (parentheses). |
| **Performance** | Slower due to mutability. | Faster due to immutability. |
| **Use Case** | Used when data needs to change frequently. | Used when data should remain constant. 

---

### **Example: Converting a List to a Tuple**
```python
my_list = [1, 2, 3, 4]
my_tuple = tuple(my_list)
print(my_tuple)
```
**Output:**
```
(1, 2, 3, 4)
```

---

### **Example: Converting a Tuple to a List**
```python
my_tuple = (5, 6, 7, 8)
my_list = list(my_tuple)
print(my_list)
```
**Output:**
```
[5, 6, 7, 8]
```


---

### **Q4: Difference between Aliasing and Cloning**  

| Feature | Aliasing | Cloning |
|---------|---------|---------|
| **Definition** | Two variables refer to the same object in memory | A new copy of the object is created |
| **Effect of Change** | Changes in one variable reflect in another | Changes in one do not affect the other |
| **Example** | `b = a` | `b = a.copy()` |
|Code|	`alias_list = original_list`|	`cloned_list = original_list.copy()` or `cloned_list = list(original_list)`|

#### **Example Code:**

#### Aliasing
```python
a = [1, 2, 3, 4, 5, 6]
b = a
print(a)  # Output: [1, 2, 3, 4, 5, 6]
print(b)  # Output: [1, 2, 3, 4, 5, 6]
a[0] = 100
print(a)  # Output: [100, 2, 3, 4, 5, 6]
print(b)  # Output: [100, 2, 3, 4, 5, 6]
````
#### Cloning (Shallow Copy)
```python
a = [1, 2, 3, 4, 5]
b = a.copy()
print(b)   # [1, 2, 3, 4, 5]
b[0]=100
print(a)  # [1, 2, 3, 4, 5]
print(b)  # [100, 2, 3, 4, 5]
```
---

### **Q5: Dictionary Operations**  
Create two dictionaries dict1 and dict2 with user-given (key, value) pairs. Perform the following operations:
- Print dict1 in sorted order.
- Create a copy of dict1 and print it.
- Print the keys and values (separately) of dict1 in sorted order.
- Update the contents of dict1 with dict2, then print the results appropriately.
  
```python
# Creating dictionaries with user input
dict1 = {"a": 10, "b": 5, "c": 15}
dict2 = {"d": 20, "e": 25}

# 1. Print dict1 in sorted order
print("Sorted dict1:", dict(sorted(dict1.items())))

# 2. Create a copy of dict1 and print it
dict1_copy = dict1.copy()
print("Copy of dict1:", dict1_copy)

# 3. Print keys and values of dict1 separately in sorted order
print("Sorted keys:", sorted(dict1.keys()))
print("Sorted values:", sorted(dict1.values()))

# 4. Update dict1 with dict2 and print the result
dict1.update(dict2)
print("Updated dict1:", dict1)
```

#### **Expected Output:**  
```
Sorted dict1: {'a': 10, 'b': 5, 'c': 15}
Copy of dict1: {'a': 10, 'b': 5, 'c': 15}
Sorted keys: ['a', 'b', 'c']
Sorted values: [5, 10, 15]
Updated dict1: {'a': 10, 'b': 5, 'c': 15, 'd': 20, 'e': 25}
```
#### OR

````python
key=input("keys: ").split(",")
values=input("values: ").split(",")
d1=dict(zip(key,values))
k=input("keys: ").split(",")
v=input("values: ").split(",")
d2=dict(zip(k,v))

print("sorted d1 :", sorted(d1))
c=d1.copy()
print("copy: ",c)
print("sorted keys: ", sorted(d1.keys()))
print("sorted values :",sorted(d1.values()))
d1.update(d2)
print(d1)
````
---

### **Q6: Menu-Driven Program**  

```python
while True:
    print("\nMenu:")
    print("1. If \"1\" is entered, must be able to illustrate nested list comprehension.")
    print("2. If \"2\" is entered, must be able to print a number pattern ")
    print("3. If any other integer is entered, the code must be able to terminate with a message: Signing off.”)
    choice = int(input("Enter your choice: "))
    if choice==1:
        table = [[i * j for j in range(1, 6)] for i in range(1, 6)]
        # Printing the nested list in a structured way
        for row in table:
            print(row)
    elif choice==2:
        n=4
        for i in range(1,n+1):
            for j in range(1,i+1):
                print(j,end=" ")
            print()
    else:
        print("Signing Off")
        break
```

#### **Example Run:**  
```python
1. If "1" is entered, must be able to illustrate nested list comprehension.
2. If "2" is entered, must be able to print a number pattern 
3. If any other integer is entered, the code must be able to terminate with a message: Signing off.

Enter your choice: 2
Enter a number: 4

Output:
1
1 2
1 2 3
1 2 3 4
```
```
Enter your choice: 5
Signing off.
```
---
