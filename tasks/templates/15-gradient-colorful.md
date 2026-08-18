# Template 15 — Gradient / Colorful (`templates/15-gradient-colorful/`)

## SEO angle
Targets: "colorful resume template html", "modern resume template with gradient".

## Who it's for
People who want a vibrant, eye-catching resume — less extreme than Template 03
(Creative Portfolio), more universally applicable.

## Layout & sections
Standard single/two-column structure; header uses a gradient background band.

## Style direction
- CSS `linear-gradient` header driven by `--color-gradient-start`/`--color-gradient-end`
  variables. The rest of the page stays clean/neutral so readability isn't compromised.

## Customization points
- The two gradient-stop variables are trivial to change to any brand colors.

## Acceptance criteria
- Follows all rules in `../02-design-system.md`.
- Passes `../09-qa-accessibility-checklist.md`.
- `@media print` forces a solid, print-safe fallback color for the header — gradients
  often print poorly and waste ink.
