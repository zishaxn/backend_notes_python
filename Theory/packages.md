

# 📦 Packages in Python

When your project grows, one file (module) is not enough.

You need multiple related modules grouped together.

That group is called a **package**.

---

## Define Package Clearly

A package is:

> A folder that contains multiple Python modules.

Usually, it includes a file named:

```
__init__.py
```

This tells Python that the folder should be treated as a package.

---

## Why Do We Need Packages?

If everything is in one file:

```
main.py  (500+ lines)
```

It becomes messy and hard to manage.

Packages help:

- Organize code
- Separate responsibilities
- Structure large projects
- Prepare for real backend development

---

## Example Project Structure

```
project/
│
├── main.py
└── utils/
    ├── __init__.py
    ├── math_utils.py
    └── string_utils.py
```

Here:

- `utils` → package
- `math_utils.py` → module
- `string_utils.py` → module

---

## Example Module Inside Package

### math_utils.py

```python
def add(a, b):
    return a + b
```

---

## Importing From a Package

In `main.py`:

```python
from utils.math_utils import add

print(add(5, 3))
```

Explain:

- `utils` → package
- `math_utils` → module inside package
- `add` → function inside module

---

## Clean Mental Hierarchy

```
Package
   └── Module
         └── Function / Class
```

---

## Relationship Between Module and Package

- Module = single Python file
- Package = folder containing multiple modules

So:

```
One file → Module
Multiple related files → Package
```

---

---

## Important Notes

- `__init__.py` can be empty.
- It marks the folder as a package.
- Python creates `__pycache__` automatically when modules are used.
- Packages help keep large projects clean and maintainable.

---

## Quick Comparison

| Concept           | Meaning                            |
| ----------------- | ---------------------------------- |
| Built-in function | Works without import (`print()`)   |
| Module            | Single Python file (`math.py`)     |
| Package           | Folder containing multiple modules |



If you create a folder and put multiple Python files inside it, you are structuring it like a package.
When you add **init**.py, Python officially treats that folder as a package.
So yes, creating multiple modules inside a folder is exactly how we build packages.


---
