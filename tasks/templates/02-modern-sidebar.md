# Template 02 — Modern Sidebar (`templates/02-modern-sidebar/`)

## SEO angle
Targets: "modern html resume template", "resume template with photo html".

## Who it's for
General professionals who want a photo plus an at-a-glance contact/skills panel.

## Layout & sections
Fixed-width left sidebar (photo, contact info, skills, languages) + main content
(summary, experience, education) on the right. Sidebar stacks on top of main content
on mobile.

## Style direction
- Colors: one strong accent color as the sidebar background.
- Skills shown as small rounded tags.

## Customization points
- Sidebar width and photo shape (circle vs. square, via a CSS class toggle) are the
  main levers.

## Acceptance criteria
- Follows all rules in `../02-design-system.md`.
- Passes `../09-qa-accessibility-checklist.md`.
- In `@media print`, the sidebar becomes a top block (not hidden) — nothing in it may
  be lost when printed.
