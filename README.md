# python-internals-for-loop
Understand how Python for-loops really work using iterators, generators, and exception handling.


# 🔍 Python Internals: How `for` Loops Work

This mini project explains what happens *under the hood* when we use a Python `for` loop. We explore:

- ✅ List Comprehensions
- ✅ Generator Functions & Expressions
- ✅ Iterators using `iter()` and `next()`
- ✅ How `for` uses `try`/`except` with `StopIteration` internally

Each topic is demonstrated using Jupyter notebooks with step-by-step explanations and examples.

---

## 📘 Notebooks Included

| No. | Topic                           | File                               |
|-----|---------------------------------|------------------------------------|
| 1   | List Comprehensions             | `01_list_comprehensions.ipynb`     |
| 2   | Generators & Iterators          | `02_generators_and_iterators.ipynb`|
| 3   | Internals of `for` Loop         | `03_for_loop_internals.ipynb`      |

---

## 💡 Why This Project?

We all use `for` loops in Python daily, but few understand how they work internally. This project helps bridge that gap by showing:

``python
for item in iterable:
    print(item)

..is actually doing this behind the scenes:

iterator = iter(iterable)
while True:
    try:
        item = next(iterator)
        print(item)
    except StopIteration:
        break ...

### 🧠 Skills Practiced
Python fundamentals

Iteration protocol

Exception handling

Clean, educational notebook writing



## 👨‍💻 Author
This project is part of my learning journey to deeply understand how Python works.

Feel free to ⭐ this repo or fork it to explore further.
