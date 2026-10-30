# Architecture and Design Decisions

GreenSpace Lite follows a lightweight, modular MVC (Model-View-Controller) inspired structure tailored for Flask applications.

## 1. System Architecture Overview
- **Backend Framework:** Flask handles HTTP routing, business logic, and request/response lifecycles.
- **Database & ORM:** SQLite3 acts as the relational database, managed via lightweight SQL queries or an ORM layer for portability and zero-configuration setup.
- **Templates:** Jinja2 templating engine renders dynamic HTML pages directly on the server side.

## 2. Project Folder Structure
greenspace-lite/
├── app.py                # Main application entry point & routes
├── database.db           # SQLite database file (local)
├── requirements.txt      # Python dependencies (Flask, etc.)
├── templates/            # HTML views (dashboard, add_plant, etc.)
├── static/               # CSS stylesheets & client-side assets
└── docs/                 # Project documentation (Sprint 0 artifacts)
    ├── PROCESS.md
    ├── ENVIRONMENT.md
    ├── BACKLOG.md
    ├── UX.md
    └── ARCHITECTURE.md