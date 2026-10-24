# 📄 Python Cheat Sheet

Everything from the course on one page.

## Day 1: Output and comments
```python
print("Hello World")        # text needs quotes
print(2026)                 # numbers don't
print(5 + 3)                # 8
print("Age:", 20)           # commas add a space
print()                     # empty line
# This is a comment — Python ignores it
```

## Day 2: Variables, types, input, operators
```python
name = "Ali"                # str   (text)
age = 20                    # int   (whole number)
gpa = 3.5                   # float (decimal)
is_student = True           # bool  (True / False)

type(age)                   # <class 'int'>
x, y = 10, 20               # multiple assignment
score += 10                 # score = score + 10

name = input("Name: ")              # always returns a string!
age = int(input("Age: "))           # convert to int
price = float(input("Price: "))     # convert to float
str(20)                             # "20"

print(f"{name} is {age}")   # f-string
```
| `+` | `-` | `*` | `/` | `//` | `%` | `**` |
|---|---|---|---|---|---|---|
| add | subtract | multiply | divide (→ decimal) | whole-number divide | remainder | power |
| `7+2`→9 | `7-2`→5 | `7*2`→14 | `7/2`→3.5 | `7//2`→3 | `7%2`→1 | `7**2`→49 |

## Day 3: Decisions
```python
if score >= 80:
    print("A")
elif score >= 50:
    print("Pass")
else:
    print("Fail")

if age >= 18 and has_ticket: ...
if day == "Sat" or day == "Sun": ...
if not is_raining: ...
```
Comparison: `==` `!=` `>` `<` `>=` `<=`. Remember: `=` stores a value, `==` compares.

## Day 4: while loops
```python
count = 1
while count <= 5:
    print(count)
    count += 1          # don't forget, or it loops forever!

while True:
    answer = input("Password: ")
    if answer == "python":
        break           # leave the loop
```
`continue` skips to the next round. Stop an infinite loop with **■ / Ctrl + C**.

## Day 5: for loops
```python
for i in range(5):          # 0 1 2 3 4
for i in range(1, 6):       # 1 2 3 4 5
for i in range(0, 11, 2):   # 0 2 4 6 8 10
for i in range(5, 0, -1):   # 5 4 3 2 1
for letter in "hello":      # h e l l o

total = 0
for n in range(1, 101):
    total += n              # accumulator

print("*", end=" ")         # stay on the same line
```

## Day 6: Strings
```python
s = "Python"
s[0]          # 'P'        s[-1]     # 'n'
s[0:3]        # 'Pyt'      s[::-1]   # 'nohtyP'
len(s)        # 6
s.upper()     s.lower()    s.title()     s.strip()
s.replace("P", "J")        s.count("o")  s.find("t")
"a b c".split()            # ['a', 'b', 'c']
"-".join(["a", "b"])       # 'a-b'
"th" in s                  # True
f"{3.14159:.2f}"           # '3.14'
"\n" = new line   "\t" = tab
```

## Day 7: Lists
```python
fruits = ["apple", "banana"]
fruits[0]                 # 'apple'
fruits.append("cherry")   # add to end
fruits.insert(0, "mango") # add at position
fruits.remove("banana")   # remove by value
fruits.pop()              # remove last
"apple" in fruits         # True
len(fruits)  sum(nums)  min(nums)  max(nums)  sorted(nums)

for fruit in fruits:
    print(fruit)
for i, fruit in enumerate(fruits, start=1):
    print(i, fruit)
```

## Day 8: Functions
```python
def greet(name, greeting="Hello"):
    """Say hello to someone."""
    return f"{greeting}, {name}!"

message = greet("Ali")
print(greet("Sara", "Hi"))
```
`print` *shows* a value. `return` *gives it back* (and ends the function).

## Day 9: Dictionaries and tuples
```python
student = {"name": "Ali", "age": 20}
student["name"]                 # 'Ali'
student.get("email", "none")    # safe: no crash
student["city"] = "Kabul"       # add / change
del student["age"]              # delete
"name" in student               # True
for key, value in student.items():
    print(key, value)

point = (3, 5)                  # tuple — can't be changed
x, y = point                    # unpacking
```

## Day 10: Handling errors
```python
try:
    age = int(input("Age: "))
except ValueError:
    print("Please type a number!")
```

## 🐛 Common errors

| Error | Usual cause |
|---|---|
| `SyntaxError` | Missing `:`, quote or bracket |
| `IndentationError` | Code inside `if`/loop/function isn't indented |
| `NameError` | Spelling mistake, `Print` instead of `print`, or the variable wasn't created |
| `TypeError` | Mixing types, e.g. `"Age: " + 20` or comparing `input()` text with a number |
| `ValueError` | `int("hello")`: the text can't be converted |
| `IndexError` | List/string index too big |
| `KeyError` | The dictionary doesn't have that key. Use `.get()` |
| `ZeroDivisionError` | Dividing by 0 |
