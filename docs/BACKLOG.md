# Initial Product Backlog

This backlog contains the initial prioritized user stories for GreenSpace Lite, broken down into manageable deliverables for Sprints 1 through 3.

## 1. High Priority (MVP Core)
- **US01 - User Authentication:** As a user, I want to register and log in so that my plant data is saved securely.
  - *Acceptance Criteria:* User must provide a valid email and password (min 6 chars). Successful login redirects to dashboard.
- **US02 - Add Plant:** As a user, I want to add a plant with a name and watering frequency (in days) so that I can track its schedule.
  - *Acceptance Criteria:* Plant name cannot be empty; watering interval must be a positive integer.
- **US03 - View Plant Status Dashboard:** As a user, I want to see a list of my plants with visual indicators (🟢 Healthy / 🔴 Needs Water) so that I know which plants require attention.
  - *Acceptance Criteria:* Dashboard automatically calculates status based on current date vs. next watering date.
- **US04 - Water Plant Action:** As a user, I want to click a "Water" button on a plant so that its last watered date resets to today.
  - *Acceptance Criteria:* Clicking "Water" updates database timestamp instantly and changes status indicator to 🟢 Healthy.

## 2. Medium Priority (Enhancements)
- **US05 - Edit / Delete Plant:** As a user, I want to update a plant's details or remove it if I no longer have it.
- **US06 - Filter Plants:** As a user, I want to filter my dashboard to show only plants that need watering today.

## 3. Low Priority (Post-MVP / Optional)
- **US07 - Plant Care Notes:** As a user, I want to add short notes to a plant (e.g., "needs indirect sunlight").

---

## 4. Measurable Quality Scenarios
- **NFR-01 (Performance):** The plant status dashboard must load all user plant records within 500ms under standard local operating conditions.
- **NFR-02 (Reliability/Data Integrity):** The SQLite database must retain user authentication tokens and plant status correctly across web server restarts with 0% data loss.