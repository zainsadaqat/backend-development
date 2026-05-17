# Create First Django Project

## Part 1 — Virtual Environment

Explain:

```text id="jlwm77"
Every project should have isolated dependencies
```

Commands:

```bash id="jlwm78"
python -m venv venv
```

Activate:

Mac/Linux:

```bash id="’wini79"
source venv/bin/activate
```

---

# Part 2 — Install Django

```bash id="’wini80"
pip install django
```

Explain:

```text id="’wini81"
pip installs Python packages from PyPI
```

---

# Part 3 — Create Django Project

```bash id="’wini82"
django-admin startproject food_delivery
```

Explain:

```text id="’wini83"
Project = entire backend system
```

---

# Part 4 — Open Project Structure

Now discuss:

```text id="’wini84"
manage.py
settings.py
urls.py
```

High-level only.

---

# Part 5 — Run Development Server

```bash id="’wini85"
python manage.py runserver
```

Then open:

```text id="’wini86"
http://127.0.0.1:8000
```

Critical moment psychologically:

```text id="’wini87"
“My backend server is running”
```

---

# Part 6 — Explain What Just Happened

Very important.

When running server:

```text id="’wini88"
Django starts listening for HTTP requests
```

Browser sends request:

```text id="’wini89"
GET /
```

Django responds with page.

Tie it back to:

```text id="’wini90"
request → processing → response
```

---

# Part 7 — Create First App

```bash id="’wini91"
python manage.py startapp menu
```

Explain:

```text id="’wini92"
Project = whole system
App = modular feature/component
```

Example:

```text id="’wini93"
users app
orders app
payments app
```

---

# Part 8 — Register App

In `settings.py`:

```python id="’wini94"
INSTALLED_APPS = [
    ...
    'menu',
]
```

Explain:

```text id="’wini95"
Django must know this app exists
```

---

# Part 9 — First View

In `views.py`:

```python id="’wini96"
from django.http import HttpResponse

def home(request):
    return HttpResponse("Hello Maciek")
```

---

# Part 10 — URL Routing

Explain:

```text id="’wini97"
URLs decide which view handles which request
```

Connect URL to view.

---

# Final Mental Model

By end of this lesson he should understand:

```text id="’wini98"
Browser
→ URL
→ Django View
→ Response
```

This is the backbone of all backend development.

---

# Important Teaching Advice

Do NOT rush into:

* models
* templates
* ORM
* forms

yet.

First stabilize:

```text id="’wini99"
request/response cycle
project/app structure
routing
views
```

Otherwise Django becomes memorization instead of architecture.
