# Task 09 — QA & Accessibility Checklist

Run this against every template — the 20 initial ones, and any future community
contribution — before it's merged.

- [ ] Validates with the W3C HTML validator (no errors).
- [ ] One `<h1>`, logical `<h2>`/`<h3>` nesting, no skipped levels.
- [ ] Color contrast passes WCAG AA (text vs. background), including after swapping
      `--color-primary` to a different value.
- [ ] Fully usable at 320px width (mobile) and 1440px+ (desktop) — no horizontal scroll.
- [ ] `@media print` produces a clean PDF via the browser's print dialog (correct
      margins, nothing cut off, no navigation chrome).
- [ ] No console errors; no external network requests required (works fully offline
      once downloaded).
- [ ] Folder size ≤ 300KB.
- [ ] All images have meaningful `alt` text (or `alt=""` if purely decorative).
- [ ] Placeholder content is clearly marked as a placeholder (e.g. "Jane Doe", "Your
      Company Inc.") and easy to find/replace.
- [ ] `thumbnail.png` is present and accurately represents the rendered template.

This checklist is referenced by [02-design-system.md](02-design-system.md),
[06-contributing.md](06-contributing.md), and every file in `tasks/templates/`.
