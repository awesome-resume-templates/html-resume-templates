# Task 02 — Shared Design System / Conventions

## Goal
Define the rules every one of the 20 templates must follow, so the collection feels
consistent and stays trivially easy to customize — without sharing actual code between
templates (each folder stays self-contained per [00-overview.md](00-overview.md)).

## Rules

1. **Theme via CSS custom properties**, declared at the top of each template's `style.css`:
   ```css
   :root {
     --color-bg: #ffffff;
     --color-text: #1a1a1a;
     --color-primary: #2563eb;
     --color-muted: #6b7280;
     --font-heading: "Georgia", serif;
     --font-body: "Helvetica Neue", Arial, sans-serif;
     --spacing-unit: 8px;
     --page-max-width: 800px;
   }
   ```
   A non-developer should be able to reskin the whole resume by editing only this block.

2. **Semantic HTML5 landmarks + predictable IDs/classes**: `<header id="resume-header">`,
   `<section id="experience">`, `<section id="education">`, `<section id="skills">`,
   `<footer>`. Consistent naming lets the customization guide give exact instructions
   that work across all 20 templates.

3. **Inline HTML comments at every editable spot**: `<!-- Your name -->`,
   `<!-- Add/remove one <li> per job -->`.

4. **Every template ships a `@media print` block** so the browser's "Print to PDF"
   produces a clean, page-safe résumé (no nav chrome, correct margins, no wasted
   background ink unless a template intentionally overrides this).

5. **Mobile responsive**: single-column fallback below ~600px width, no horizontal scroll.

6. **Zero external runtime dependencies**: no CDN JS frameworks, no required internet
   connection once downloaded. Local web-safe fonts, or a bundled `@font-face` file only
   when essential to a template's identity.

7. **Accessible by default**: correct heading hierarchy (one `<h1>`, then `<h2>` per
   section), WCAG AA color contrast, meaningful `alt` text on any image/photo placeholder.

8. **File size budget**: each template folder ≤ 300KB total (keeps the repo light and
   pages fast — a speed signal for SEO too).

## Deliverable
This file is the checklist referenced by every template task in `tasks/templates/` and
by [09-qa-accessibility-checklist.md](09-qa-accessibility-checklist.md).
