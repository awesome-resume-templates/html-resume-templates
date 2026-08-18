# Contributing

Thanks for wanting to improve this collection. Here's how to add a new
template or fix an existing one.

## Adding a new template

1. **Open an issue first** describing the style you'd like to add (e.g. "brutalist / neo-brutalist template") so we can make sure it doesn't overlap heavily with an existing one.
2. **Create a new folder** at `templates/NN-slug/`, where `NN` is the next available two-digit index and `slug` is a short kebab-case name (e.g. `templates/21-brutalist/`).
3. **Add three files** to that folder:
   - `index.html` — the template markup
   - `style.css` — the template's styles
   - `thumbnail.png` — a screenshot of the rendered template, roughly 800×1035 (portrait, matches the aspect ratio used across the gallery), showing it full-page on a white/neutral background
4. **Follow the shared conventions** in [`tasks/02-design-system.md`](tasks/02-design-system.md):
   - Theme via CSS custom properties (`--color-primary`, `--font-heading`, etc.) declared at the top of `style.css`
   - Semantic HTML5 with predictable IDs (`#resume-header`, `#experience`, `#education`, `#skills`)
   - Inline HTML comments marking every editable spot
   - A `@media print` block that produces a clean PDF
   - A single-column responsive fallback under ~600px
   - Zero external runtime dependencies (no CDN fonts/JS, no build step)
   - One `<h1>`, correct heading hierarchy, WCAG AA color contrast
   - Folder size ≤ 300KB total
5. **Run the checklist** in [`tasks/09-qa-accessibility-checklist.md`](tasks/09-qa-accessibility-checklist.md) before opening a PR.
6. **Add your template to the gallery**: a new row in the table in `README.md`, and a new card in `docs/index.html`.

Each template folder is self-contained on purpose — don't add shared CSS/JS
files that multiple templates depend on. Copy-paste between templates is
expected and fine.

## Reporting a bug

Open an issue with:
- Which template
- What you expected vs. what happened
- Browser/OS if it's a rendering issue
- A screenshot if it's visual

## Pull request checklist

- [ ] Follows the folder structure and design-system conventions above
- [ ] `index.html` validates with the [W3C HTML validator](https://validator.w3.org/) (no errors)
- [ ] Works with no console errors and no external network requests
- [ ] Responsive at 320px and up, no horizontal scroll
- [ ] `@media print` produces a clean, uncut print-to-PDF result
- [ ] Placeholder content is clearly placeholder (e.g. "Jane Doe") and easy to find/replace
- [ ] `thumbnail.png` added and accurate
- [ ] README gallery table and `docs/index.html` both updated

## Code of conduct

Be respectful, keep discussion focused on the work, and no spam PRs. That's it.
