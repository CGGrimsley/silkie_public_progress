# SiLKiE Development Roadmap & Progress

---

# Phase 0 — Planning & Foundation

### Goals
Clarify what SiLKiE needs to do, outline the user experience, and establish the core system design.

- [x] Define the purpose of SiLKiE  
- [x] Identify core features (checklist builder, inventory wizard, dashboard)  
- [x] Outline main user flows  
- [x] Draft early interface sketches  
- [x] Identify initial data models (SOP, Section, Item, InventoryItem)  
- [x] Establish structured WBS for staged development  
- [ ] Finalize the full feature list  
- [ ] Define non-functional requirements  
- [ ] Draft public-facing architecture diagrams  

---

# Phase 1 — Backend Core (Django REST API)

This phase covers the creation of the backend skeleton, project structure, models, and API fundamentals.

## 1.1 Backend Project Setup
- [x] Initialized Django project (`silkie_backend`)  
- [x] Created modular Django apps: accounts, sops, inventory, core  
- [x] Set up environment structure and settings layout  
- [x] Added Django REST Framework to the project  
- [x] Created base URL routing for API v1  
- [x] Verified backend boots cleanly with `runserver`  
- [x] Set up development environment and virtual environment  
- [ ] Add global exception handler  
- [ ] Add production settings structure  

## 1.2 Testing Infrastructure
- [x] Installed and configured `pytest` + `pytest-django`  
- [x] Created initial test directories and structure  
- [x] Resolved test discovery issues (`tests.py` vs `tests/` conflict)  
- [x] Verified clean test run (`1 passed`)  
- [ ] Add backend feature tests  
- [ ] Add factories & mock data  
- [ ] Begin writing API endpoint tests  

## 1.3 Accounts & Authentication
- [x] Defined required user information  
- [ ] Implement registration endpoint  
- [ ] Implement login/logout  
- [ ] Implement profile retrieval/update  
- [ ] Add authentication (JWT or session)  

## 1.4 SOP / Checklist System
- [x] Defined structure: SOP → Section → Item  
- [ ] Implement models  
- [ ] Add CRUD endpoints  
- [ ] Add duplication endpoint  
- [ ] Add draft/publish workflow  

## 1.5 Inventory Wizard System
- [x] Defined interactive flow  
- [x] Identified data structure for categories/items  
- [ ] Implement inventory models  
- [ ] Build wizard logic endpoints  
- [ ] Add export-friendly output  

---

# Phase 2 — Frontend App (React)

## 2.1 Frontend Setup
- [x] Initialized React app using Vite  
- [x] Installed and configured Tailwind CSS  
- [ ] Add routing (React Router)  
- [ ] Add global layout (Navigation + Sidebar)  
- [ ] Add global theme (light/dark mode)  

## 2.2 Dashboard & Navigation
- [ ] Create dashboard screen  
- [ ] Add sidebar navigation  
- [ ] Implement persistent layout components  

## 2.3 Checklist Builder UI
- [ ] List overview page  
- [ ] SOP editor (sections/items)  
- [ ] Reordering capability  
- [ ] Template picker  

## 2.4 Inventory Wizard UI
- [ ] Wizard question interface  
- [ ] Category builder  
- [ ] Final summary + export  

---

# Phase 3 — Testing & Stability

## Backend Testing
- [x] pytest installed and validated  
- [ ] Expand test coverage for accounts  
- [ ] Add SOP API tests  
- [ ] Add Inventory Wizard API tests  
- [ ] Increase coverage to >70%  

## Frontend Testing
- [ ] Add Jest/Vitest  
- [ ] Add component tests  
- [ ] Add integration tests  

## End-to-End Testing
- [ ] Add Playwright/Selenium setup  

---

# Phase 4 — Pre-Release Preparation

- [ ] Improve UI consistency  
- [ ] Add onboarding tooltips  
- [ ] Prepare minimal documentation  
- [ ] Configure deployment pipeline  
- [ ] Prepare alpha testing instructions  

---

# 🎉 Phase 5 — Beta Launch

- [ ] Invite first testers  
- [ ] Gather user feedback  
- [ ] Fix early UX issues  
- [ ] Prepare for wider release  

---

# 📅 Overall Project Status

| Phase | Status |
|-------|--------|
| Phase 0 – Planning | 🟢 Complete / Minor items left |
| Phase 1 – Backend | 🟡 In Progress |
| Phase 2 – Frontend | ⚪ Not Started |
| Phase 3 – Testing | ⚪ Not Started |
| Phase 4 – Prep | ⚪ Not Started |
| Phase 5 – Beta | ⚪ Not Started |

---

# 🔄 How This Document Updates
Progress will be updated here as milestones are completed. Check back anytime to see what’s new.
