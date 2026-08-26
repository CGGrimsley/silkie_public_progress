# SiLKiE Development Roadmap & Progress

*Last reviewed: 26 August 2026. Development began 2 December 2025.*

The original version of this document was written at project kickoff and stopped
being accurate somewhere around Phase 1. This is a full re-audit against what is
actually deployed.

The short version: **the app is live in beta at [silkie.io](https://silkie.io)**.
Phases 0–5 are done. The product also grew well past its original scope — events,
a community layer and subscriptions were never in the first plan and are now
shipped, so they get their own phases below.

---

# 📅 Overall Project Status

| Phase | Status |
| :--- | :--- |
| Phase 0 — Planning & foundation | 🟢 Complete |
| Phase 1 — Backend core | 🟢 Complete |
| Phase 2 — Frontend app | 🟢 Complete |
| Phase 3 — Testing & stability | 🟢 Complete |
| Phase 4 — Pre-release prep | 🟢 Complete |
| Phase 5 — Beta launch | 🟢 Live |
| Phase 6 — Events | 🟢 Complete |
| Phase 7 — Community | 🟢 Complete |
| Phase 8 — Subscriptions | 🟢 Complete |
| Phase 9 — Hardening & polish | 🟡 Ongoing |
| Phase 10 — Wider release | ⚪ Planned |

---

# Phase 0 — Planning & Foundation

- [x] Define the purpose of SiLKiE
- [x] Identify core features (checklist builder, inventory wizard, dashboard)
- [x] Outline main user flows
- [x] Draft early interface sketches
- [x] Identify initial data models
- [x] Establish structured WBS for staged development
- [x] Finalize the full feature list
- [x] Define non-functional requirements
- [ ] Draft public-facing architecture diagrams

---

# Phase 1 — Backend Core

## 1.1 Project setup
- [x] Django project and modular apps
- [x] Django REST Framework wired up
- [x] Environment/settings layout
- [x] Versioned API routing
- [x] Environment-driven production configuration
- [x] API documentation schema
- [ ] Global exception handler

## 1.2 Testing infrastructure
- [x] pytest + pytest-django configured
- [x] Test layout and discovery resolved
- [x] Backend feature tests
- [x] API endpoint tests
- [x] Seed/demo data command

## 1.3 Accounts & authentication
- [x] Registration
- [x] Login / logout
- [x] Google sign-in
- [x] JWT authentication
- [x] Profile retrieval and update
- [x] Avatar upload
- [x] Email confirmation
- [x] Password reset
- [x] Change password while signed in
- [x] Account deletion

## 1.4 SOP / checklist system
- [x] Structure: SOP → Section → Item
- [x] Models implemented
- [x] CRUD endpoints
- [x] Inventory-linked items
- [x] PDF export
- [ ] Duplication endpoint
- [ ] Draft/publish workflow
- [ ] Template picker

## 1.5 Inventory system
- [x] Inventory models with nested items
- [x] Guided wizard endpoints
- [x] Category-driven setup flow
- [x] Undo a wizard session
- [x] Bulk operations
- [x] Item photos
- [x] Export-friendly output

---

# Phase 2 — Frontend App

## 2.1 Setup
- [x] React + Vite
- [x] Tailwind configured against a shared token set
- [x] Routing
- [x] Global layout and navigation
- [x] Theme and design system

## 2.2 Dashboard & navigation
- [x] Dashboard screen
- [x] Responsive navigation with mobile drawer
- [x] Persistent layout components
- [x] Notifications

## 2.3 Checklist builder UI
- [x] List overview page
- [x] SOP editor with sections and items
- [x] Section reordering
- [x] PDF export from the UI
- [ ] Template picker

## 2.4 Inventory wizard UI
- [x] Wizard question interface
- [x] Category builder
- [x] Summary and export
- [x] Full inventory management screen

---

# Phase 3 — Testing & Stability

- [x] Backend test suite across every app
- [x] Frontend component and integration tests (39 files, 207 tests)
- [x] End-to-end tests with Playwright
- [x] Continuous integration on every push — lint, test and build, both halves
- [ ] Expand end-to-end coverage beyond the core flows

---

# Phase 4 — Pre-Release Preparation

- [x] UI consistency pass against a single token set
- [x] Onboarding tour and tooltips
- [x] Privacy policy, terms and cookie policy
- [x] Cookie/tracking consent
- [x] Deployment pipeline
- [x] Production hosting and custom domain

---

# 🎉 Phase 5 — Beta Launch

- [x] Beta programme with a capped invite list
- [x] First testers invited
- [x] In-app beta banner and feedback route
- [x] Early UX fixes from feedback
- [ ] Open signup beyond the cap

---

# Phase 6 — Events

- [x] Event models and API
- [x] Shared calendar with agenda view
- [x] Regional and type filtering
- [x] Event creation and editing
- [x] RSVPs
- [x] Personal "my events" view for organisers and attendees
- [x] Visibility controls and organiser groups

---

# Phase 7 — Community

- [x] Profiles with photos and bios
- [x] Discovery and matching
- [x] Friends system with requests
- [x] Following feed
- [x] Direct messaging
- [x] Group chats
- [x] Groups with shared inventories
- [x] Reporting and moderation tooling
- [x] Blocking

---

# Phase 8 — Subscriptions

- [x] Stripe integration
- [x] Plans and pricing page
- [x] Subscription management
- [x] Webhook handling

---

# Phase 9 — Hardening & Polish (ongoing)

This is where the work currently sits. Most of it is unglamorous.

- [x] Mobile pass: touch targets, safe-area insets, overflow
- [x] Accessibility pass: contrast, focus indicators, reduced-motion support
- [x] Performance: route-level code splitting, a long-lived vendor chunk,
      lazy-loaded heavy dependencies, polling that pauses on hidden tabs
- [x] Security headers and transport hardening
- [x] Self-serve account data export
- [x] Affirmative consent and age attestation at signup

---

# Phase 10 — Wider Release (planned)

- [ ] Open registration
- [ ] Public launch
- [ ] Mobile applications

---

# 🔄 How this document updates

Reviewed as milestones land rather than on a schedule. For a running view of
day-to-day activity, see my [profile page](https://github.com/CGGrimsley) — it's
regenerated nightly from the private repository.
