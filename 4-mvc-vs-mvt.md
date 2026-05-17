# What is MVC?

MVC is a design pattern used to organize web applications.

Its goal is simple:

```text id="jlwm56"
Separate responsibilities
```

So code does not become chaos.

---

# MVC Stands For

```text id="jlwm57"
Model
View
Controller
```

Each part has one job.

---

# Imagine a Restaurant

This analogy works perfectly.

---

# 1. Model = Kitchen + Storage

Model handles:

```text id="jlwm58"
data
database
business rules
```

Example:

* customers
* orders
* products

In Django:

```python id="jlwm59"
class Product(models.Model):
    name = models.CharField(...)
```

Model talks to database.

---

# Important

Model does NOT care about:

* HTML
* buttons
* webpage design

Only data.

---

# 2. View = What User Sees

View handles:

```text id="jlwm60"
presentation
UI
display
```

Example:

* HTML page
* product list
* profile page

In traditional MVC:

```text id="jlwm61"
View = frontend display
```

---

# 3. Controller = Middle Manager

Controller handles:

```text id="jlwm62"
requests
logic
coordination
```

It receives request and decides:

```text id="jlwm63"
“What should happen?”
```

Example:

* fetch products
* validate form
* save order

Then:

* talks to Model
* sends data to View

---

# Full MVC Flow

```text id="jlwm64"
User clicks page
    ↓
Controller receives request
    ↓
Controller asks Model for data
    ↓
Model gets database data
    ↓
Controller sends data to View
    ↓
View renders HTML
    ↓
User sees webpage
```

---

# Why MVC Exists

Without separation:

```text id="jlwm65"
HTML
database
logic
routing
```

all mix together into one giant mess.

MVC keeps code organized.

---

# Important Django Clarification

Django is NOT pure MVC.

Django uses something very similar called:

```text id="jlwm66"
MVT
```

---

# Django’s MVT

```text id="jlwm67"
Model
View
Template
```

---

# Mapping MVC → Django

## MVC Model

Same as Django Model.

Handles database/data.

---

## MVC View

In Django this becomes:

```text id="jlwm68"
Template
```

because template handles display.

---

## MVC Controller

In Django this becomes:

```text id="jlwm69"
View
```

Django views contain request-handling logic.

---

# Why Django Renamed Things

Because Django views are NOT visual pages.

They are:

```text id="jlwm70"
request handlers
```

This confuses beginners heavily.

---

# Real Django Flow

```text id="jlwm71"
Browser request
    ↓
URL
    ↓
Django View
    ↓
Model
    ↓
Template
    ↓
HTML Response
```

---

# Simple Mental Model

## Model

```text id="jlwm72"
Data
```

---

## View (Django)

```text id="jlwm73"
Logic
```

---

## Template

```text id="jlwm74"
Presentation
```

---

# Core Principle

MVC/MVT are about:

```text id="jlwm75"
separating concerns
```

Each component should have:

```text id="jlwm76"
one responsibility
```

That principle matters more than the acronym itself.
