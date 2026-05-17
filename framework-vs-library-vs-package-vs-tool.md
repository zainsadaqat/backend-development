# Framework vs Library vs Package vs Tool

These words confuse beginners because people use them loosely.

Understand them through **control and responsibility**.

---

# 1. What is a Library?

A library is:

```text id="jlwm38"
Code you call when you need help
```

You stay in control.

---

## Example

```python id="jlwm39"
import math

math.sqrt(16)
```

You are telling the library:

```text id="jlwm40"
“Hey, calculate square root for me”
```

Library responds and leaves.

---

# Key Idea

```text id="jlwm41"
YOU control the flow
```

The library is just assistance.

---

# Real Life Analogy

Library = calculator.

You decide:

* when to use it
* where to use it
* how to use it

---

# 2. What is a Framework?

Framework is bigger.

A framework says:

```text id="jlwm42"
“I control the structure and flow.
You plug your code into me.”
```

---

## Example in Django

You don’t manually start request handling.

Django says:

```text id="jlwm43"
“When request comes,
I will call your view function”
```

So Django controls the flow.

---

# Key Idea

```text id="jlwm44"
Framework controls the application lifecycle
```

This is called:

```text id="jlwm45"
Inversion of Control
```

---

# Real Life Analogy

Framework = restaurant kitchen system.

The restaurant decides:

* kitchen layout
* workflow
* stations

You work inside the system.

---

# 3. What is a Package?

Package is simply:

```text id="jlwm46"
A bundle of reusable code
```

Usually installable.

Example:

```bash id="jlwm47"
pip install requests
```

`requests` is a package.

---

# Important

A package can be:

* a library
* a framework
* utilities
* anything reusable

---

# 4. What is a Tool?

Tool helps developers perform tasks.

Not necessarily part of app runtime.

Examples:

* VS Code
* Git
* Docker
* Postman

---

# Real Analogy

```text id="jlwm48"
Tool = screwdriver
```

Helps you build.

But not part of the house itself.

---

# Quick Comparison

## Library

```text id="jlwm49"
You call it
```

Example:

* requests
* math

---

## Framework

```text id="jlwm50"
It calls you
```

Example:

* Django
* React
* FastAPI

---

## Package

```text id="jlwm51"
Reusable installable code
```

Example:

* numpy
* requests
* django

---

## Tool

```text id="jlwm52"
Helps development workflow
```

Example:

* Git
* VS Code
* Postman

---

# Most Important Insight

Frameworks impose:

```text id="jlwm53"
structure
rules
flow
architecture
```

Libraries do not.

---

# Simple Mental Model

```text id="jlwm54"
Library → helper
Framework → system
Package → distributable code
Tool → developer utility
```

---

# Why Django Matters

Django is:

```text id="jlwm55"
Framework
```

because:

* it controls request lifecycle
* defines project structure
* routes requests
* manages application flow

You write code INSIDE Django’s system.
