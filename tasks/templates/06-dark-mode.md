# Template 06 — Dark Mode (`templates/06-dark-mode/`)

## SEO angle
Targets: "dark mode resume template", "dark resume html".

## Who it's for
Anyone who wants a modern dark aesthetic for on-screen viewing/sharing (with a sane
print fallback).

## Layout & sections
Same structure as the Minimalist template, themed dark.

## Style direction
- Dark background, high-contrast accent text.
- This is the riskiest template for accessibility — verify contrast carefully, don't
  just eyeball it.

## Customization points
- `--color-bg`/`--color-text` are already inverted by default; include a commented
  "light mode override" block users can uncomment.

## Acceptance criteria
- Follows all rules in `../02-design-system.md`.
- Passes `../09-qa-accessibility-checklist.md`, with WCAG AA contrast verified
  explicitly (not assumed) given the dark palette.
- **`@media print` must force a light background + dark text — never print a dark
  background.** This is a hard requirement, not a style preference.
