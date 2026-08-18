# Task 00 — Project Overview & Tech Decisions

## Goal
Build **awesome-html-resume-templates**: a free, open-source collection of 20
hand-crafted HTML/CSS resume templates, packaged in a repo that ranks well for
"html resume templates" and "free html resume templates", and that a non-developer
can customize by editing plain text in a file.

## Tech decision
**Plain HTML5 + CSS3 per template. No build step, no framework, no `npm install`.**

- Why: the target user is often not a developer — they need to open a file, change
  text, and print/export to PDF. A build pipeline (React/Vite/Tailwind build) adds a
  step that can break and that non-developers can't debug.
- Each template is a **self-contained folder** (`index.html` + `style.css` +
  `thumbnail.png`) so a user can download *one folder* and have everything they need.
- CSS custom properties (`--color-primary`, `--font-heading`, etc.) at the top of each
  `style.css` act as the "theme" a non-technical user edits. See
  [02-design-system.md](02-design-system.md).
- Optional shared, non-blocking piece: a `/docs` gallery site (static HTML) for live
  demos, hosted on GitHub Pages. See [05-gallery-index-page.md](05-gallery-index-page.md).
- No backend, no database, no analytics beyond what GitHub Pages provides by default.

## Success criteria
- 20 templates live in `templates/`, each opens correctly from `file://` and when hosted.
- Root `README.md` carries strong on-page SEO signals: keyword-rich H1/intro, gallery
  table, FAQ (see [04-readme-seo.md](04-readme-seo.md)).
- A person with no coding background can follow
  [03-template-customization-guide.md](03-template-customization-guide.md) and produce
  a personalized resume in under 15 minutes.
- All templates pass [09-qa-accessibility-checklist.md](09-qa-accessibility-checklist.md).

## Out of scope (for now)
- Template builder UI / live in-browser editor (possible future v2).
- Server-side PDF generation (users export via browser print-to-PDF instead).
- CMS or JSON-driven templating (adds complexity contrary to the "easy to customize" goal).
