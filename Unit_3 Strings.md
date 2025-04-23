# Unit 3 - Lesson 3
___________
- String Pattern Matching
- Introduction to Regular Expressions
- Overview of a string pattern
- More on meta characters
- Pattern methods
- Compilation flags
- Grouping
---------------

## Chapter: String Pattern Matching 

### 1. **Introduction to Regular Expressions (Regex)**

Regular Expressions, often abbreviated as **regex**, are powerful tools for pattern matching and text processing. They allow you to search, match, and manipulate strings based on patterns. In Python, the `re` module provides a variety of functions for working with regular expressions.

A **regular expression** is a sequence of characters that defines a search pattern. It can be used to search for specific sequences in a string, replace parts of a string, or even split a string based on certain conditions.

#### **Why Use Regular Expressions?**
- Quickly find matching patterns within large strings.
- Validate inputs like email addresses, phone numbers, etc.
- Extract specific information from texts.

### 2. **Overview of a String Pattern**

A **string pattern** is the expression you use to search for specific sequences in text. The pattern could be simple or complex depending on the criteria you want to match.

#### **Simple String Pattern Example**:
A basic pattern like `\d+` will match one or more digits in a string.

#### Example Code: Basic Pattern Matching

```python
import re

# Pattern to match digits in a string
pattern = r"\d+"  # One or more digits
text = "There are 123 apples and 45 oranges."

# Using re.search() to find the pattern
match = re.search(pattern, text)
if match:
    print(f"Found a match: {match.group()}")
else:
    print("No match found.")
```
**Output:**
```
Found a match: 123
```

### 3. **More on Meta Characters**

Meta characters are special characters in regular expressions that allow for flexible pattern matching. Here's a list of commonly used meta characters:

- **`.`** : Matches any single character except newline.
- **`\d`** : Matches any digit (0-9).
- **`\w`** : Matches any alphanumeric character (letters and digits).
- **`\s`** : Matches any whitespace character (spaces, tabs, newlines).
- **`*`** : Matches 0 or more of the preceding character.
- **`+`** : Matches 1 or more of the preceding character.
- **`?`** : Matches 0 or 1 of the preceding character.

#### Example Code: Using Meta Characters

```python
import re

# Pattern to match a sequence of digits followed by a space and a word
pattern = r"\d+\s\w+"  # One or more digits followed by a space and a word
text = "I have 3 apples and 10 oranges."

# Using re.findall() to get all matches
matches = re.findall(pattern, text)
print(f"Matches found: {matches}")
```
**Output:**
```
Matches found: ['3 apples', '10 oranges']
```


---

## 🔹 Meta Characters in Regular Expressions (Regex)

**Meta characters** are **special symbols** in regex. They don’t match literal characters — instead, they define **rules or patterns** to help search text more powerfully.

Imagine you want to find all phone numbers, emails, or words starting with capital letters — meta characters help you build patterns for that.

---

### 🔹 Common Meta Characters and Their Meanings

| Meta Character | Meaning                                 | Example                             |
|----------------|------------------------------------------|-------------------------------------|
| `.`            | Any character (except newline)           | `a.c` matches `abc`, `axc`          |
| `^`            | Start of a string                        | `^Hello` matches if string starts with "Hello" |
| `$`            | End of a string                          | `world$` matches if string ends with "world" |
| `*`            | 0 or more of the previous character      | `ab*` matches `a`, `ab`, `abb`, etc |
| `+`            | 1 or more of the previous character      | `ab+` matches `ab`, `abb`, not `a`  |
| `?`            | 0 or 1 of the previous character         | `ab?` matches `a`, `ab`             |
| `[]`           | Matches one character from the set       | `[aeiou]` matches any vowel         |
| `[^]`          | Matches anything **not** in the set      | `[^0-9]` matches any non-digit      |
| `{}`           | Matches a specific number of repetitions | `a{2}` matches `aa`, `a{2,3}` matches `aa` or `aaa` |
| `\`            | Escape special characters                | `\.` matches a dot `.`              |
| `|`            | OR operator                              | `cat|dog` matches `cat` or `dog`    |
| `()`           | Grouping and capturing                   | `(ab)+` matches `ab`, `abab`, etc   |

---



#### 1. `.` – Matches Any One Character

```python
import re

pattern = r"a.c"  # a, then any character, then c
text = "abc a-c a9c axc"

matches = re.findall(pattern, text)
print(matches)
```

**Output:**
```
['abc', 'a-c', 'a9c', 'axc']
```

---

#### 2. `^` and `$` – Start and End of Line

```python
# ^ checks if the string starts with "Hello"
re.match(r"^Hello", "Hello world")    # ✅ match
re.match(r"^Hello", "world Hello")    # ❌ no match

# $ checks if the string ends with "world"
re.search(r"world$", "Hello world")   # ✅ match
re.search(r"world$", "world Hello")   # ❌ no match
```

---

#### 3. `*` – Zero or More Repetitions

```python
pattern = r"ab*"
text = "a ab abb abbb abbbb"
print(re.findall(pattern, text))
```

**Output:**
```
['a', 'ab', 'abb', 'abbb', 'abbbb']
```

---

#### 4. `+` – One or More Repetitions

```python
pattern = r"ab+"
text = "a ab abb abbb abbbb"
print(re.findall(pattern, text))
```

**Output:**
```
['ab', 'abb', 'abbb', 'abbbb']
```

---

#### 5. `[]` – Character Set

```python
pattern = r"[aeiou]"
text = "Hello, how are you?"
print(re.findall(pattern, text))
```

**Output:**
```
['e', 'o', 'o', 'a', 'e', 'o', 'u']
```

---

#### 6. `[^]` – Negated Character Set

```python
pattern = r"[^aeiou\s]"  # Match all characters except vowels and space
text = "Hello world"
print(re.findall(pattern, text))
```

**Output:**
```
['H', 'l', 'l', 'w', 'r', 'l', 'd']
```

---

#### 7. `{}` – Repetition Count

```python
pattern = r"a{2,3}"
text = "a aa aaa aaaa"
print(re.findall(pattern, text))
```

**Output:**
```
['aa', 'aaa', 'aaa']
```

---

#### 8. `|` – OR Operator

```python
pattern = r"cat|dog"
text = "I love my cat and my dog."
print(re.findall(pattern, text))
```

**Output:**
```
['cat', 'dog']
```

---

#### 9. `()` – Grouping

```python
pattern = r"(ha)+"
text = "hahaha haha ha"
print(re.findall(pattern, text))
```

**Output:**
```
['ha', 'ha', 'ha']
```

---

### 4. **Pattern Methods**

Python's `re` module provides several methods to work with patterns. Here are the most commonly used ones:

#### **1. `re.match()`**

- Tries to match the pattern at the **beginning** of the string.
- Returns a match object if the pattern matches the start of the string.

```python
import re

pattern = r"apple"
text = "apple pie"

# Match pattern at the beginning of the string
match = re.match(pattern, text)
if match:
    print(f"Match found: {match.group()}")
else:
    print("No match found.")
```
**Output:**
```
Match found: apple
```

#### **2. `re.search()`**

- Scans the string for the first location where the pattern matches.
- Returns a match object if the pattern is found anywhere in the string.

```python
import re

pattern = r"apple"
text = "I love apple pie!"

# Search for the pattern anywhere in the string
match = re.search(pattern, text)
if match:
    print(f"Match found: {match.group()}")
else:
    print("No match found.")
```
**Output:**
```
Match found: apple
```

#### **3. `re.findall()`**

- Returns a list of all non-overlapping matches in the string.

```python
import re

pattern = r"\d+"  # Matches one or more digits
text = "There are 123 apples, 456 oranges, and 789 bananas."

matches = re.findall(pattern, text)
print(f"All digit matches: {matches}")
```
**Output:**
```
All digit matches: ['123', '456', '789']
```

#### **4. `re.sub()`**

- Replaces all occurrences of the pattern with a specified string.

```python
import re

pattern = r"\d+"  # Matches one or more digits
text = "My number is 12345."

# Replace digits with '#'
replaced_text = re.sub(pattern, "#", text)
print(f"Replaced text: {replaced_text}")
```
**Output:**
```
Replaced text: My number is #####.
```

### 5. **Compilation Flags**

Regular expressions in Python can be modified using **flags**, which change how the patterns behave. Here are some common flags:

- **`re.IGNORECASE`**: Makes the pattern case-insensitive.
- **`re.MULTILINE`**: Changes the behavior of `^` and `$` to match the start and end of each line.
- **`re.DOTALL`**: Makes the dot (`.`) match newlines as well.

#### Example Code: Using Flags

```python
import re

pattern = r"hello"
text = "Hello world!"

# Use re.IGNORECASE flag for case-insensitive matching
match = re.search(pattern, text, re.IGNORECASE)
if match:
    print(f"Match found: {match.group()}")
else:
    print("No match found.")
```
**Output:**
```
Match found: Hello
```

### 6. **Grouping**

Grouping in regular expressions allows you to capture part of the matched string. You can use parentheses `()` to define groups. After matching, you can access each group separately.

#### Example Code: Using Grouping

```python
import re

pattern = r"(\d+)-(\d+)-(\d+)"  # Grouping phone number parts
text = "My phone number is 123-456-7890."

match = re.search(pattern, text)
if match:
    print(f"Area code: {match.group(1)}")
    print(f"Prefix: {match.group(2)}")
    print(f"Line number: {match.group(3)}")
else:
    print("No match found.")
```
**Output:**
```
Area code: 123
Prefix: 456
Line number: 7890
```

