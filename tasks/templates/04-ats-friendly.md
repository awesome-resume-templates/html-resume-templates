# Template 04 — ATS-Friendly (`templates/04-ats-friendly/`)

## SEO angle
Targets: "ATS friendly resume template html", "ATS resume template free".

## Who it's for
Job seekers worried about applicant tracking systems failing to parse their resume.

## Layout & sections
Strict single column, no tables, no multi-column CSS grid for content, no required
icons/images. Standard section order: Summary, Experience, Education, Skills.

## Style direction
- Intentionally plain — no background colors, no text-in-images, just clean
  typographic hierarchy.

## Customization points
- Minimal by design — this template's whole point is restraint. Only the shared
  color/font variables.

## Acceptance criteria
- Follows all rules in `../02-design-system.md`.
- Passes `../09-qa-accessibility-checklist.md`, with extra rigor on semantic
  correctness (real `<h2>` per section, no `<div>` soup — this is what actually makes
  it parsable).
- A short in-folder note explains *why* it avoids graphics, for users who are curious.
