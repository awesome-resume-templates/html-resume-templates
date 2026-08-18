# Template 17 — Two-Column Compact / One-Page (`templates/17-two-column-compact/`)

## SEO angle
Targets: "one page resume template html", "compact resume template".

## Who it's for
People who need to fit a lot of content onto exactly one page.

## Layout & sections
Dense two-column body grid from the top (not just a sidebar), smaller but still
accessible type scale, tight spacing.

## Style direction
- Minimal decoration — the entire space budget goes to content density, not ornament.

## Customization points
- `--spacing-unit` and a `--font-size-base` variable are the primary levers a user
  nudges to make their content fit exactly one page.

## Acceptance criteria
- Follows all rules in `../02-design-system.md`.
- Passes `../09-qa-accessibility-checklist.md`, with extra care that WCAG AA contrast
  and a sane minimum font size still hold despite the compact design.
