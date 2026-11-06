# Architecture and Design Decisions

GreenSpace Lite follows a lightweight, modular MVC (Model-View-Controller) inspired structure tailored for Flask applications.

## 1. System Architecture Overview
- **Backend Framework:** Flask handles HTTP routing, business logic, and request/response lifecycles.
- **Database & ORM:** SQLite3 acts as the relational database, managed via lightweight SQL queries or an ORM layer for portability and zero-configuration setup.
- **Templates:** Jinja2 templating engine renders dynamic HTML pages directly on the server side.

## 2. Project Directory Structure
```text
greenspace-lite/
├── .github/
│   └── workflows/
│       └── ci.yml            # GitHub Actions: installs dependencies, runs pytest (exists)
├── docs/                     # Sprint 0 documentation (exists)
│   ├── PROCESS.md
│   ├── ENVIRONMENT.md
│   ├── BACKLOG.md
│   ├── UX.md
│   ├── ARCHITECTURE.md
│   ├── TEAM_AGREEMENT.md
│   ├── GLOSSARY_AND_RISKS.md
│   └── RETROSPECTIVE.md
├── tests/
│   └── test_smoke.py         # Smoke test (exists)
├── .gitignore                # Keeps venv, *.db and .env out of Git (exists)
├── README.md                 # Entry point and deliverables index (exists)
├── requirements.txt          # Python dependencies (exists)
├── app.py                    # Application entry point and routes (planned, Sprint 1)
├── templates/                # Jinja2 HTML views (planned, Sprint 1)
├── static/                   # CSS and client-side assets (planned, Sprint 1)
└── database.db               # SQLite file, created locally at runtime, not committed
```

Items marked "exists" are in the repository now. Items marked "planned" will be added during Sprint 1.