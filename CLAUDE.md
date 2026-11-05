# Notes for agents working in this repo

This is SiLKiE's **public** progress tracker. The app's source lives in the private `CGGrimsley/silkie` repo; the claude-loop harness there sends tasks here with a `Code repo: CGGrimsley/silkie_public_progress` line.

- Two files only: `README.md` (overview) and `progress.md` (phased roadmap with checkboxes). Don't add files unless the task asks.
- Everything here is public. Never include code, file paths, endpoint names, security details, user data, vendor account details, internal task ids or unreleased pricing. Describe shipped features in plain user terms.
- Tick an item `[x]` only when it is merged to silkie `main` and deployed. When you change any status, update the "Last reviewed" date at the top of `progress.md`.
- Keep the existing tone, headings and status emoji (🟢 complete/live, 🟡 ongoing, ⚪ planned/not started).
- Checks: `git diff --check origin/main...HEAD` (no CI here). Preview the Markdown before handing back.
