# Glossary & Risk List

## 1. Glossary (Project Terminology)
- **Flask:** A lightweight web application framework written in Python, used to handle HTTP routing, requests, and server-side logic for GreenSpace Lite.
- **Scrumban:** A hybrid agile project management framework combining Scrum principles (iterative development) with Kanban visual workflow management.
- **SQLite3:** A self-contained, serverless, zero-configuration SQL database engine embedded directly into the application for local data persistence.
- **PAT (Personal Access Token):** A secure alternative to using account passwords for authenticating Git operations against the remote GitHub repository.
- **MVP (Minimum Viable Product):** The core version of GreenSpace Lite containing essential features (authentication, adding plants, status dashboard, and watering action) required to satisfy initial project requirements.

## 2. Risk List & Mitigation Strategies
- **Risk 1: Authentication & Credential Conflicts on Shared/Local Environments**
  - *Impact Level:* Medium
  - *Mitigation:* Utilizing project-scoped Personal Access Tokens (PAT) and secure local configuration to isolate Git operations and prevent authorization failures.
- **Risk 2: Scope Creep during Sprint Execution**
  - *Impact Level:* High
  - *Mitigation:* Strict adherence to the prioritized Product Backlog and focusing purely on MVP core requirements before considering optional enhancements (e.g., care notes).
- **Risk 3: Database Integrity and State Loss**
  - *Impact Level:* Medium
  - *Mitigation:* Utilizing structured local SQLite database tracking combined with unit tests (`pytest`) to ensure data models and user states persist correctly across server restarts.