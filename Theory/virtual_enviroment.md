

# 🧪 Virtual Environment (venv)

When working on multiple Python projects, different projects may need:

- Different libraries
- Different versions of the same library

Installing everything globally causes conflicts.

A **virtual environment** solves this problem.

---

## Define Virtual Environment Clearly

A virtual environment is:

> An isolated Python environment for a specific project.

It has:

- Its own Python interpreter
- Its own installed packages
- Its own `site-packages` folder

---

## Why Do We Need It?

Without venv:

- All packages install globally
- Version conflicts happen
- Projects interfere with each other

With venv:

- Each project has its own isolated dependencies
- No conflicts between projects
- Cleaner system Python

---

## Creating a Virtual Environment

Inside your project folder:

```bash
python -m venv venv
```

This creates a folder named `venv/`.

---

## Activating the Virtual Environment

### Windows

```bash
venv\Scripts\activate
```

When activated, your terminal changes to show:

```
(venv)
```

This means you are inside the isolated environment.

---

## Installing Packages Inside venv

```bash
pip install requests
```

This installs the package only inside that virtual environment.

Not globally.

---

## Deactivating

```bash
deactivate
```

You return to the global Python environment.

---

## Requirements File

To save installed packages:

```bash
pip freeze > requirements.txt
```

To reinstall later:

```bash
pip install -r requirements.txt
```

This ensures:

- Same versions
- Same environment on another machine

---

## Clean Mental Model

```
Global Python  → Main system
Virtual Environment → Private project workspace
```

Packages installed inside venv:

- Exist only inside that project
- Do not affect other projects

---

## Quick Comparison

| Without venv      | With venv                 |
| ----------------- | ------------------------- |
| Global installs   | Project-specific installs |
| Version conflicts | Isolated versions         |
| Hard to manage    | Clean and controlled      |

---
