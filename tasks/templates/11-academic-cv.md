# Template 11 — Academic CV (`templates/11-academic-cv/`)

## SEO angle
Targets: "academic cv template html", "cv template html free".

## Who it's for
Researchers/academics who need a longer, multi-page CV, not a 1-page resume.

## Layout & sections
Education, Publications, Research Experience, Teaching, Grants/Awards, Conferences —
explicitly denser and longer than the other 19 templates.

## Style direction
- Formal, serif or neutral sans; a numbered/citation-style list for publications.

## Customization points
- Publications list is a simple ordered list users paste citations directly into.

## Acceptance criteria
- Follows all rules in `../02-design-system.md`.
- Passes `../09-qa-accessibility-checklist.md`.
- Must be explicitly tested for correct multi-page `@media print` pagination — use
  `break-inside: avoid` on list items so an entry never splits mid-way across a page break.
