# CS101 Spring 2026 — Practice Midterm (Multiple Choice)

Name: Add Your Name Here  
Date: Add Date Here

**Instructions:** For each question, record your answer by replacing `TODO` with
the letter of the single best response (a, b, c, or d). 

---

### 1. What does the following code produce?

```python
for i in range(2, 11, 3):
    print(i)
```

a) 2, 3, 4, 5, 6, 7, 8, 9, 10  
b) 2, 5, 8  
c) 2, 4, 6, 8, 10  
d) 2, 9

**Your answer:** TODO

---

### 2. Which of the following loops prints the numbers 8 down to 4?

a) `for i in range(8, 4, 1):`  
b) `for i in range(8, 4):`  
c) `for i in range(8, 3, -1):`  
d) `for i in range(4, 8, -1):`

**Your answer:** TODO

---

### 3. For the code below, how many lines are printed?

```python
for x in range(2):
    for y in range(4):
        print(x, y)
```

a) 2  
b) 4  
c) 8  
d) 16

**Your answer:** TODO

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
d) (6, 27)

**Your answer:** TODO

---

### 5. Which algorithmic method checks candidates one-by-one within a range to find an exact integer solution?

a) Binary search  
b) Exhaustive enumeration  
c) Newton's method  
d) Bisection method

**Your answer:** TODO

---

### 6. What does the following code print?

```python
info = {"city": "Boston", "state": "MA", "zip": "02101"}
info["zip"] = "02134"
print(len(info))
```

a) 2  
b) 3  
c) 4  
d) Error

**Your answer:** TODO

---

### 7. The intersection of `{1, 3, 5, 7}` and `{5, 7, 9, 11}` is:

a) {1, 3}  
b) {9, 11}  
c) {1, 3, 5, 7, 9, 11}  
d) {5, 7}

**Your answer:** TODO

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

c)
```python
for name in grades:
    print(name, grades[name])
```

d)
```python
for name, grade in grades.values():
    print(name, grade)
```

**Your answer:** TODO

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
b) Comfortable  
c) Cold  
d) Nothing is printed

**Your answer:** TODO

---

### 10. Which operator returns the **remainder** of a division?

a) //  
b) **  
c) %  
d) /

**Your answer:** TODO

---

### 11. Which of the following is a valid Python **integer** literal?

a) 3.14  
b) "42"  
c) True  
d) 0xFF

**Your answer:** TODO

---

### 12. What does `print(f"Area: {4 ** 2}")` print?

a) Area: 8  
b) Area: 42  
c) Area: 16  
d) Error

**Your answer:** TODO

---

### 13. What is the output of the following code?

```python
values = (3, 5, 2, 8, 4)
total = 0
for v in values:
    total += v
print(total)
```

a) 22  
b) 18  
c) 30  
d) 20

**Your answer:** TODO

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
d) (10, 20, 10, 20)

**Your answer:** TODO

---

### 15. Which list comprehension produces `[0, 1, 4, 9, 16]`?

a) `[i ** 2 for i in range(1, 6)]`  
b) `[i * 2 for i in range(5)]`  
c) `[i ** 2 for i in range(5)]`  
d) `[i + i for i in range(5)]`

**Your answer:** TODO

---

### 16. For `word = "Programming"`, what is `word[3:7]`?

a) Prog  
b) mmit  
c) gram  
d) rogram

**Your answer:** TODO

---

### 17. What does `"hello world".title()` return?

a) HELLO WORLD  
b) hello world  
c) Hello World  
d) Error

**Your answer:** TODO

---

### 18. What does the following print?

```python
f = lambda x, y: x - y if x > y else x + y
print(f(3, 7))
```

a) -4  
b) 4  
c) 21  
d) 10

**Your answer:** TODO

---

### 19. After `items = [10, 20]; items += [30, 40, 50]`, what does `print(items)` produce?

a) [10, 20]  
b) [30, 40, 50]  
c) Error  
d) [10, 20, 30, 40, 50]

**Your answer:** TODO

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
d) {'p': 3, 'q': 4, 'r': 12}

**Your answer:** TODO

---

### 21. What is the value of `3 ** 2 ** 2`?

a) 36  
b) 9  
c) 16  
d) 81

**Your answer:** TODO

---

### 22. Slice `letters = ['a', 'b', 'c', 'd', 'e', 'f']` to get `['b', 'd', 'f']`:

a) `letters[::2]`  
b) `letters[1::2]`  
c) `letters[1:5:2]`  
d) `letters[2::2]`

**Your answer:** TODO

---

### 23. What does `len((1, 2, 3, 4, 5))` return?

a) 0  
b) 4  
c) Error  
d) 5

**Your answer:** TODO

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
c) False, True  
d) Error

**Your answer:** TODO

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
d) [1, 3, 5, 7, 9]

**Your answer:** TODO

---

-- End of Practice Test --
(Did you remember to add your name to the top of this document?)
