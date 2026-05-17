# How the Web Works

Forget frameworks and Django for now.

First understand:

```text id="jlwml1"
How the browser and server talk to each other
```

Everything in web development is built on this.

---

# Imagine Ordering Food

You open a food app and click:

```text id="jlwml2"
“Show me burgers”
```

What happens behind the scenes?

---

# 1. Browser Sends a Request

Your browser says:

```text id="jlwml3"
“Hey server, give me the burgers page”
```

This is called:

```text id="jlwml4"
HTTP Request
```

---

# 2. Server Receives the Request

A server is just:

```text id="jlwml5"
A computer running backend code
```

It listens for requests all day.

---

# 3. Server Processes the Request

Server may:

* read database
* run Python code
* check login
* fetch products

Example:

```text id="jlwml6"
Fetch burgers from database
```

---

# 4. Server Sends Back a Response

The server replies:

```text id="jlwml7"
“Here’s the HTML page”
```

This is called:

```text id="jlwml8"
HTTP Response
```

---

# 5. Browser Displays It

Browser renders:

* text
* images
* buttons
* layout

Now user sees webpage.

---

# Full Flow

```text id="jlwml9"
Browser
   ↓ request
Server
   ↓ response
Browser
```

---

# Real Example

You visit:

```text id="jlwm10"
youtube.com
```

Browser sends:

```text id="jlwm11"
GET /homepage
```

Server responds:

```text id="jlwm12"
HTML + data + videos
```

Browser displays YouTube homepage.

---

# Important Insight

The web is basically:

```text id="jlwm13"
Request → Processing → Response
```

That’s it.

Everything else:

* Django
* React
* APIs
* databases

are layers built around this cycle.

---

# What Is HTTP?

HTTP is just:

```text id="jlwm14"
A communication language between browser and server
```

Like:

```text id="jlwm15"
“Give me this page”
“Here’s your data”
```

---

# Common HTTP Methods

## GET

```text id="jlwm16"
“Give me data”
```

Example:

```text id="jlwm17"
Open homepage
```

---

## POST

```text id="jlwm18"
“Send data”
```

Example:

```text id="jlwm19"
Submit login form
```

---

# What Django Actually Does

Django helps manage:

```text id="jlwm20"
Request → Python logic → Database → Response
```

Without Django, you’d manually handle everything.

---

# Mental Model To Keep Forever

```text id="jlwm21"
Frontend (browser) asks
Backend (server) responds
Database stores
```

That is the entire web at a high level.

---

Next step should be:

```text id="jlwm22"
Why web frameworks exist?
```

Because now the pain of doing everything manually will make sense.
