# Template 18 — Designer / Visual Portfolio (`templates/18-designer-visual/`)

## SEO angle
Targets: "graphic designer resume template html".

## Who it's for
Graphic/visual designers who want a large photo and a built-in portfolio thumbnail grid.

## Layout & sections
Large circular/square photo in the header, a dedicated "Work" section as a
responsive image grid (placeholder images), Experience/Education below.

## Style direction
- Bold single accent color, generous imagery, strong grid alignment.

## Customization points
- The image grid is a simple repeatable `<figure>` block; document how to swap
  placeholder images with the user's own work samples.

## Acceptance criteria
- Follows all rules in `../02-design-system.md`.
- Passes `../09-qa-accessibility-checklist.md`.
- The portfolio image grid is simplified or excluded in `@media print` (image-heavy
  grids print poorly); state directly in-file that this template is meant primarily as
  a live web page, not a PDF.
