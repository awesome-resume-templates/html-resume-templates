# Task 06 — CONTRIBUTING.md

## Goal
Let outside contributors submit new templates without breaking conventions.

## Content
- How to propose a template (open an issue first, avoid duplicating an existing style).
- Folder/naming convention: `templates/NN-slug/` (`NN` = next available two-digit index).
- Required files: `index.html`, `style.css`, `thumbnail.png` (recommended size, e.g.
  800×1000, showing the template full-page).
- Must satisfy every rule in [02-design-system.md](02-design-system.md) (link it) and
  pass [09-qa-accessibility-checklist.md](09-qa-accessibility-checklist.md).
- Must add a row to the README gallery table and a card to `docs/index.html`.
- PR checklist (checkboxes) mirroring the QA checklist.
- Short code-of-conduct statement (be respectful, no spam PRs) or link to one.

## Acceptance criteria
- A contributor unfamiliar with the repo can read this file alone and submit a
  compliant PR without back-and-forth.
