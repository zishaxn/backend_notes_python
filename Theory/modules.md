
When you install Python, you get:

1. **Built-in functions**

   - Example: `print()`, `len()`, `type()`
   - These work without importing anything.

2. **Standard Library Modules**

   - These are files containing related functions.
   - You must import them to use them.

Example:

```python
import math
```

The `math` module contains:

- `sqrt()`
- `sin()`
- `cos()`
- `pi`

So instead of writing your own square root logic, you reuse:

```python
math.sqrt(25)
```

---

## Define Module Clearly

A module is:

> A Python file that contains related functions, variables, or classes.

That’s it.

Example:

- `math` → mathematical functions
- `json` → JSON handling
- `os` → operating system interaction

---


### Step 1 — Built-in Function

```python
print("Hello")
```

No import needed.

### Step 2 — Module Usage

```python
import math
print(math.sqrt(16))
```

Explain:

- `math` = module
- `sqrt` = function inside module

---

# Efficiency Upgrade

Draw this mentally:

```
Python
│
├── Built-in functions
│   └── print(), len()
│
└── Modules
    ├── math
    ├── json
    └── os
```

That hierarchy prevents confusion.

---
