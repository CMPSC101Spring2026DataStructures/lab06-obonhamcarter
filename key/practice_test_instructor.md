# CS101 Spring 2026 — Practice Midterm (Multiple Choice)
# INSTRUCTOR COPY — Answer Key

**Instructions:** Correct answers are indicated with `[ANSWER]`.

---

### 1. What does the following code produce?

```python
for i in range(2, 11, 3):
    print(i)
```

a) 2, 3, 4, 5, 6, 7, 8, 9, 10  
**b) 2, 5, 8** `[ANSWER]`  
c) 2, 4, 6, 8, 10  
d) 2, 9

**Correct answer: b**  
*`range(2, 11, 3)` produces 2, 5, 8 (start 2, stop before 11, step 3).*

---

### 2. Which of the following loops prints the numbers 8 down to 4?

a) `for i in range(8, 4, 1):`  
b) `for i in range(8, 4):`  
**c) `for i in range(8, 3, -1):`** `[ANSWER]`  
d) `for i in range(4, 8, -1):`

**Correct answer: c**  
*`range(8, 3, -1)` yields 8, 7, 6, 5, 4 — stopping before 3. Options a and b use a positive step with start > stop (empty range); option d has start < stop with negative step (empty range).*

---

### 3. For the code below, how many lines are printed?

```python
for x in range(2):
    for y in range(4):
        print(x, y)
```

a) 2  
b) 4  
**c) 8** `[ANSWER]`  
d) 16

**Correct answer: c**  
*The outer loop runs 2 times and the inner loop runs 4 times: 2 × 4 = 8 lines.*

---

### 4. What does the following return?

```python
def g(n):
    return n * 2, n ** 3
print(g(3))
```

a) 6  
b) 27  
c) Error  
**d) (6, 27)** `[ANSWER]`

**Correct answer: d**  
*Returning two values creates a tuple. `g(3)` returns `(6, 27)`, which is what `print` displays.*

---

### 5. Which algorithmic method checks candidates one-by-one within a range to find an exact integer solution?

a) Binary search  
**b) Exhaustive enumeration** `[ANSWER]`  
c) Newton's method  
d) Bisection method

**Correct answer: b**  
*Exhaustive enumeration (also called brute-force search) systematically tests every candidate in turn.*

---

### 6. What does the following code print?

```python
info = {"city": "Boston", "state": "MA", "zip": "02101"}
info["zip"] = "02134"
print(len(info))
```

a) 2  
**b) 3** `[ANSWER]`  
c) 4  
d) Error

**Correct answer: b**  
*Assigning to an existing key ("zip") updates its value — it does not add a new key. The dictionary still has 3 entries.*

---

### 7. The intersection of `{1, 3, 5, 7}` and `{5, 7, 9, 11}` is:

a) {1, 3}  
b) {9, 11}  
c) {1, 3, 5, 7, 9, 11}  
**d) {5, 7}** `[ANSWER]`

**Correct answer: d**  
*The intersection contains only elements present in both sets: 5 and 7.*

---

### 8. For `grades = {"Bob": 88, "Sue": 92, "Tom": 75}`, which code correctly prints both the name and grade for every entry?

a)
```python
for i in grades:
    print(i)
```

b)
```python
for name in grades.keys():
    print(grades[name])
```

**c)** `[ANSWER]`
```python
for name in grades:
    print(name, grades[name])
```

d)
```python
for name, grade in grades.values():
    print(name, grade)
```

**Correct answer: c**  
*Iterating over a dict yields keys; `grades[name]` retrieves the corresponding value. Option a prints only keys; option b prints only values; option d incorrectly tries to unpack integer values as tuples.*

---

### 9. What is the output of the following code?

```python
temp = 72
if temp > 90 or temp < 32:
    print("Extreme")
elif temp >= 60:
    print("Comfortable")
else:
    print("Cold")
```

a) Extreme  
**b) Comfortable** `[ANSWER]`  
c) Cold  
d) Nothing is printed

**Correct answer: b**  
*72 > 90 is False and 72 < 32 is False, so the first branch is skipped. 72 >= 60 is True, so "Comfortable" is printed.*

---

### 10. Which operator returns the **remainder** of a division?

a) //  
b) **  
**c) %** `[ANSWER]`  
d) /

**Correct answer: c**  
*`%` is the modulo operator (remainder). `//` is floor division; `**` is exponentiation; `/` is true division.*

---

### 11. Which of the following is a valid Python **integer** literal?

a) 3.14  
b) "42"  
c) True  
**d) 0xFF** `[ANSWER]`

**Correct answer: d**  
*`0xFF` is a valid hexadecimal integer literal (equal to 255). `3.14` is a float; `"42"` is a string; `True` is a boolean literal (a subclass of int, but not an integer literal).*

---

### 12. What does `print(f"Area: {4 ** 2}")` print?

a) Area: 8  
b) Area: 42  
**c) Area: 16** `[ANSWER]`  
d) Error

**Correct answer: c**  
*`4 ** 2` evaluates to 16, so the f-string produces "Area: 16".*

---

### 13. What is the output of the following code?

```python
values = (3, 5, 2, 8, 4)
total = 0
for v in values:
    total += v
print(total)
```

**a) 22** `[ANSWER]`  
b) 18  
c) 30  
d) 20

**Correct answer: a**  
*3 + 5 + 2 + 8 + 4 = 22.*

---

### 14. What is the output of the following code?

```python
x = (10, 20)
y = x
print(x + y)
```

a) (20, 40)  
b) (10, 20)  
c) Error  
**d) (10, 20, 10, 20)** `[ANSWER]`

**Correct answer: d**  
*`y` refers to the same tuple as `x`. Adding two tuples concatenates them: `(10, 20) + (10, 20)` = `(10, 20, 10, 20)`.*

---

### 15. Which list comprehension produces `[0, 1, 4, 9, 16]`?

a) `[i ** 2 for i in range(1, 6)]`  
b) `[i * 2 for i in range(5)]`  
**c) `[i ** 2 for i in range(5)]`** `[ANSWER]`  
d) `[i + i for i in range(5)]`

**Correct answer: c**  
*`range(5)` gives 0–4; squaring each: 0, 1, 4, 9, 16. Option a starts at 1, giving 1,4,9,16,25; options b and d both produce [0,2,4,6,8].*

---

### 16. For `word = "Programming"`, what is `word[3:7]`?

a) Prog  
b) mmit  
**c) gram** `[ANSWER]`  
d) rogram

**Correct answer: c**  
*Indices: P(0)r(1)o(2)g(3)r(4)a(5)m(6)m(7)… Slice [3:7] picks indices 3,4,5,6 → 'g','r','a','m' = "gram".*

---

### 17. What does `"hello world".title()` return?

a) HELLO WORLD  
b) hello world  
**c) Hello World** `[ANSWER]`  
d) Error

**Correct answer: c**  
*`.title()` capitalises the first letter of each word.*

---

### 18. What does the following print?

```python
f = lambda x, y: x - y if x > y else x + y
print(f(3, 7))
```

a) -4  
b) 4  
c) 21  
**d) 10** `[ANSWER]`

**Correct answer: d**  
*3 > 7 is False, so the `else` branch executes: 3 + 7 = 10.*

---

### 19. After `items = [10, 20]; items += [30, 40, 50]`, what does `print(items)` produce?

a) [10, 20]  
b) [30, 40, 50]  
c) Error  
**d) [10, 20, 30, 40, 50]** `[ANSWER]`

**Correct answer: d**  
*`+=` on a list extends it in-place, appending all elements of the right-hand list.*

---

### 20. What is the result of the following?

```python
d = {"p": 3, "q": 4}
d["r"] = d["p"] * d["q"]
print(d)
```

a) {'p': 3, 'q': 4}  
b) Error  
c) {'r': 12}  
**d) {'p': 3, 'q': 4, 'r': 12}** `[ANSWER]`

**Correct answer: d**  
*`d["r"] = 3 * 4 = 12` adds a new key "r" while keeping the existing entries.*

---

### 21. What is the value of `3 ** 2 ** 2`?

a) 36  
b) 9  
c) 16  
**d) 81** `[ANSWER]`

**Correct answer: d**  
*Exponentiation is right-associative: `3 ** (2 ** 2)` = `3 ** 4` = 81.*

---

### 22. Slice `letters = ['a', 'b', 'c', 'd', 'e', 'f']` to get `['b', 'd', 'f']`:

a) `letters[::2]`  
**b) `letters[1::2]`** `[ANSWER]`  
c) `letters[1:5:2]`  
d) `letters[2::2]`

**Correct answer: b**  
*`letters[1::2]` starts at index 1 ('b') and steps by 2: indices 1,3,5 → 'b','d','f'. Option a gives ['a','c','e']; option c gives only ['b','d'] (stops before index 5); option d gives ['c','e'].*

---

### 23. What does `len((1, 2, 3, 4, 5))` return?

a) 0  
b) 4  
c) Error  
**d) 5** `[ANSWER]`

**Correct answer: d**  
*The tuple has 5 elements; `len` works on tuples as well as lists.*

---

### 24. What does the following code print?

```python
class Book:
    def __init__(self, title, pages):
        self.title = title
        self.pages = pages

b1 = Book("Python Basics", 300)
b2 = Book("Data Structures", 450)

for b in [b1, b2]:
    print(b.pages > 400)
```

a) Python Basics, Data Structures  
b) 300, 450  
**c) False, True** `[ANSWER]`  
d) Error

**Correct answer: c**  
*300 > 400 evaluates to False; 450 > 400 evaluates to True. Each boolean is printed on its own line.*

---

### 25. What does the following code produce?

```python
nums = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
odds = [x for x in nums if x % 2 != 0]
print(odds)
```

a) [2, 4, 6, 8, 10]  
b) [1, 3, 5, 7, 9, 10]  
c) Error  
**d) [1, 3, 5, 7, 9]** `[ANSWER]`

**Correct answer: d**  
*`x % 2 != 0` selects odd numbers: 1, 3, 5, 7, 9. Option a lists even numbers; option b incorrectly includes 10.*

---

-- End of Instructor Answer Key --

## Summary Answer Key

| Q  | Answer |
|----|--------|
| 1  | b      |
| 2  | c      |
| 3  | c      |
| 4  | d      |
| 5  | b      |
| 6  | b      |
| 7  | d      |
| 8  | c      |
| 9  | b      |
| 10 | c      |
| 11 | d      |
| 12 | c      |
| 13 | a      |
| 14 | d      |
| 15 | c      |
| 16 | c      |
| 17 | c      |
| 18 | d      |
| 19 | d      |
| 20 | d      |
| 21 | d      |
| 22 | b      |
| 23 | d      |
| 24 | c      |
| 25 | d      |
