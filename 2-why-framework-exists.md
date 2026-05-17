# Why Web Frameworks Exist

Now you know:

```text id="jlwm23"
Browser → Request → Server → Response
```

Question:

```text id="jlwm24"
Why can’t we just write plain Python?
```

Technically, we can.

But it becomes painful very quickly.

---

# Imagine Building a Restaurant

Without a framework:

Every time a customer comes:

* you build the kitchen
* create the menu
* install lights
* train staff

again and again.

That’s inefficient.

---

# Same Problem in Web Development

Every website needs:

* routing (which URL goes where)
* handling requests
* generating responses
* database connection
* authentication
* security
* sessions
* forms
* admin panel

Without a framework:

```text id="jlwm25"
You build all this manually every project
```

Huge waste of time.

---

# What a Framework Does

A framework gives you:

```text id="jlwm26"
Pre-built structure + tools + rules
```

So instead of building foundation every time:

you focus on:

```text id="jlwm27"
actual product logic
```

---

# Real Analogy

Framework is like:

```text id="jlwm28"
A fully equipped kitchen
```

You still cook the food.

But:

* stove exists
* fridge exists
* plates exist

You don’t reinvent them.

---

# What Django Gives You

Out of the box:

* URL routing
* ORM
* authentication
* admin panel
* templates
* security protections
* form handling

---

# Without Framework

To create even simple login:

you must manually handle:

```text id="jlwm29"
password hashing
cookies
sessions
security
database queries
```

That’s dangerous and slow.

---

# With Django

You focus on:

```text id="jlwm30"
business logic
```

Example:

```text id="jlwm31"
Food ordering system
Blog
E-commerce
Dashboard
```

---

# Important Insight

Framework is NOT magic.

It is:

```text id="jlwm32"
organized reusable code
```

written by experienced engineers.

---

# Why Frameworks Are Opinionated

Frameworks force structure.

Example:

```text id="jlwm33"
views go here
templates go here
models go here
```

Why?

Because large projects become chaos otherwise.

---

# Core Benefit

Frameworks solve:

```text id="jlwm34"
repeated engineering problems
```

so developers can solve:

```text id="jlwm35"
product problems
```

---

# Mental Model

```text id="jlwm36"
Language = Python
Framework = organized system built using Python
```

Django is:

```text id="jlwm37"
a backend framework built in Python
```

---

# Important Clarification

Framework ≠ library.

Framework controls the flow.

You plug your code INTO the framework.

More on this in next step.
