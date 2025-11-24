# Backend Development

## Frontend vs backend
Frontend controls what the user sees and interacts with. Backend handles data, logic and communication with the database.

## Backend usage
It stores data, processes logic, enforces rules, handles authentication and sends responses to the client.

## Request response cycle
Client sends a request. Server processes it. Server returns a response with data and status. This repeats for every action.

## Why we need a framework
Doing it manually means writing your own routing, request parsing, validation, security and database handling. A framework gives these tools so you can focus on actual features.

## Virtual environment
A separate isolated Python environment so project dependencies do not conflict with system packages or other projects.

## Minimal Django folder structure
- projectname
- settings.py config for your project
- urls.py main router
- wsgi.py entry point for servers
- appname
- views.py request handlers
- models.py database tables
- urls.py routes for the app
