# Template 20 — RTL / Multilingual-Ready (`templates/20-rtl-multilingual/`)

## SEO angle
Targets: "rtl resume template html", "arabic resume template", "persian cv template html".

## Who it's for
Users writing in right-to-left languages (Arabic, Persian, Hebrew), or anyone who
wants an easy-to-translate base template.

## Layout & sections
Structurally similar to Minimalist/Modern Sidebar, but built with CSS logical
properties (`margin-inline-start`, `text-align: start`, etc.) instead of physical
left/right, so it flips correctly under `dir="rtl"`.

## Style direction
- Neutral styling that works with both Latin and Arabic/Persian web fonts — font
  stack includes a suitable fallback, e.g. `"Vazirmatn", "Noto Naskh Arabic", sans-serif`.

## Customization points
- A single `dir="ltr"|"rtl"` attribute on `<html>` flips the whole layout; document
  this at the top of `index.html` in a comment.

## Acceptance criteria
- Follows all rules in `../02-design-system.md`.
- Passes `../09-qa-accessibility-checklist.md`.
- Explicitly tested rendering in both `dir="ltr"` and `dir="rtl"` before merging — this
  extra check is not covered by the generic checklist, so call it out here.
