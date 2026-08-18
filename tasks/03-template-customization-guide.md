# Task 03 — Template Customization Guide (user-facing doc)

## Goal
Write a doc (published as `docs/CUSTOMIZATION.md` and summarized/linked from the root
README) that lets a non-developer go from "download" to "my personalized PDF resume"
with no coding knowledge required.

## Content outline
1. **Pick a template** — link to the live gallery ([05-gallery-index-page.md](05-gallery-index-page.md)).
2. **Download it** — `git clone` the whole repo, or download just one folder via
   GitHub's folder-download / a direct ZIP link the gallery page provides.
3. **Open `index.html`** in any text editor (VS Code, Notepad, TextEdit) — explain it's
   just text, nothing to compile.
4. **Replace the placeholders** — walk through the HTML comments described in
   [02-design-system.md](02-design-system.md) (name, contact info, experience bullets,
   skills list).
5. **Change the colors/fonts** — edit the `:root { --color-primary: ... }` block at the
   top of `style.css`; suggest 2–3 free Google Fonts pairings.
6. **Preview** — double-click `index.html` to open it in a browser; refresh after edits.
7. **Export to PDF** — browser Print dialog → "Save as PDF", with recommended print
   settings (margins, background graphics on/off per template).
8. **(Optional) Host it online** — one paragraph pointing at GitHub Pages/Netlify
   drag-and-drop for people who want a shareable link instead of a PDF.

## Acceptance criteria
- A person with zero coding background, following only this doc, can produce a
  customized PDF in under 15 minutes (dogfood-test it against one finished template).
