# GreenSpace Lite — Plant Care Tracker

## 1. Product Goal
To provide a lightweight, accessible web-based plant care and watering tracker that helps users manage watering schedules, prevent plant neglect, and track their indoor garden effortlessly.

## 2. Target Users
- **Primary User:** Busy plant hobbyists, students, and apartment residents who need a simple, fast way to track watering intervals without complex configurations.
- **Secondary User:** Course instructors and reviewers evaluating software engineering processes, Agile practices, and clean implementation.

## 3. Scope
- **In-Scope (MVP):** 
  - User registration and login (authentication).
  - Adding, editing, and listing plants with custom watering intervals (in days).
  - Dashboard displaying plant status (🟢 Healthy / 🔴 Needs Watering).
  - Manual "Water Plant" action that resets the next watering date.
  - Automated unit tests (`pytest`) and CI/CD pipeline (GitHub Actions).
- **Out-of-Scope (Future / Post-MVP):**
  - Weather API integration, push notifications, and photo uploads.


  ## 4. Setup Instructions

```
git clone https://github.com/Ahmetonursabancilar01/greenspace-lite.git
cd greenspace-lite
python -m venv venv
venv\Scripts\activate
pip install -r requirements.txt
python -m pytest
```

On macOS/Linux, activate the virtual environment with `source venv/bin/activate`.

## 5. Test and CI Result

- Local: `python -m pytest` gives `1 passed`.
- CI: GitHub Actions workflow in `.github/workflows/ci.yml` runs the tests on every push to `main` and every pull request. Passing run: pull request #11.

## 6. Deliverables Index

| Requirement | Location |
|---|---|
| Product goal, users, scope | Sections 1-3 of this README |
| Prioritized backlog, acceptance criteria, quality scenarios | [docs/BACKLOG.md](docs/BACKLOG.md) |
| Method choice and rationale | [docs/PROCESS.md](docs/PROCESS.md) |
| Team agreement and Definition of Done | [docs/TEAM_AGREEMENT.md](docs/TEAM_AGREEMENT.md) |
| Glossary and risk list | [docs/GLOSSARY_AND_RISKS.md](docs/GLOSSARY_AND_RISKS.md) |
| Architecture sketch | [docs/ARCHITECTURE.md](docs/ARCHITECTURE.md) |
| Setup instructions | Section 4 of this README |
| First reviewed pull request | [PR #8](https://github.com/Ahmetonursabancilar01/greenspace-lite/pull/8) |
| Test file | [PR #10](https://github.com/Ahmetonursabancilar01/greenspace-lite/pull/10) |
| CI workflow and passing result | [PR #11](https://github.com/Ahmetonursabancilar01/greenspace-lite/pull/11) |
| Issue board | [GitHub Projects board](https://github.com/users/Ahmetonursabancilar01/projects/4) |
| Sprint 0 review and retrospective | [docs/RETROSPECTIVE.md](docs/RETROSPECTIVE.md) |

## 7. Access

This repository is public and read-only for everyone except the owner. No access request or invitation is needed to inspect it. Changes to `main` are made only by the owner through pull requests. No credentials are included in the repository or in the submission.
