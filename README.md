# SiLKiE — Standardized List for Kit & Equipment

*Inventory, loadouts and SOPs for people who keep gear ready.*

**SiLKiE is live in beta at [silkie.io](https://silkie.io).**

SiLKiE started as a checklist builder and grew into a full application for
tracking what you own, building repeatable loadouts, and writing the standard
operating procedures that go with them. It's for shooters, campers,
preparedness-minded households, and anyone whose packing list currently lives
across four notes apps and a group chat.

This repository is a **public progress tracker**, not the source code. The
application itself is private; this exists so friends, collaborators and anyone
curious can follow along without me exposing the codebase.

---

## 🧭 Where the project is

Development began December 2025. The application is deployed, in beta, and
taking real users.

| Area | State |
| :--- | :--- |
| Backend API | 🟢 Live |
| Web app | 🟢 Live |
| Accounts & sign-in | 🟢 Live |
| Inventory & wizard | 🟢 Live |
| SOP builder & PDF export | 🟢 Live |
| Events | 🟢 Live |
| Community features | 🟢 Live |
| Subscriptions | 🟢 Live |
| Beta programme | 🟢 Open |
| Mobile apps | ⚪ Not started |

Full detail in **[progress.md](progress.md)**.

---

## 🧩 What works today

**Inventory**
Track gear down to the item, with nested sub-items, bulk actions, filtering and
search. A guided wizard walks you through building a kit from scratch by
category rather than staring at an empty list.

**SOPs & checklists**
Build structured procedures — sections and items — that pull from your
inventory, then export a clean PDF for printing or sharing.

**Events**
A shared calendar with regional filtering, plus RSVPs and a personal view of
what you're organising and attending.

**Community**
Find people to train with, connect, and message them one-to-one or in group
chats. Groups get shared inventories. There's a friends system, a following
feed, notifications, and moderation tooling behind it.

**Accounts & billing**
Email or Google sign-in, profile and avatar management, password reset, and
subscription handling.

---

## 🛠 How it's built

React 19, TypeScript, Vite and Tailwind on the front. Django 5 and Django REST
Framework on the back, PostgreSQL in production. Media on Cloudflare R2,
payments through Stripe, the site served from Cloudflare.

Every push runs a CI pipeline that lints and tests both halves. There is also an
autonomous build harness that works overnight on queued tasks and is not
permitted to merge anything that fails the same gates — you can see its output
on my [profile page](https://github.com/CGGrimsley).

---

## 🗺 What's next

Near-term work is listed in [progress.md](progress.md). The headline items:

- Expanded account self-service
- Route-level code splitting to cut first-load weight
- Broader end-to-end test coverage
- Continued mobile polish

---

## ✨ About this repo

No source code lives here — just milestones and status, updated as things ship.
If you're following SiLKiE, this and [silkie.io](https://silkie.io) are the
places to look.

Questions or beta access: **[support@silkie.io](mailto:support@silkie.io)**

[Instagram](https://www.instagram.com/silkie.io/) · [X](https://x.com/Silkieio)
