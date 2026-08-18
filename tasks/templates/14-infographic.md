# Template 14 — Infographic (`templates/14-infographic/`)

## SEO angle
Targets: "infographic resume template html", "visual resume template with skill bars".

## Who it's for
People who want visual skill-level indicators — a very common search intent.

## Layout & sections
Standard sections plus a "Skills" section rendered as CSS-only progress bars
(`<div class="bar" style="--level:80%">`) — no images/canvas/JS required.

## Style direction
- Colorful accent bars. Icons, if used, must be plain Unicode/CSS shapes only (no
  icon-font/CDN dependency, per the zero-dependency rule).

## Customization points
- `--level` custom property per skill row, documented as "how full the bar is".

## Acceptance criteria
- Follows all rules in `../02-design-system.md`.
- Passes `../09-qa-accessibility-checklist.md`.
- Every bar also carries a text-based accessible label (e.g. `aria-label="Advanced"`),
  since a purely visual bar isn't accessible or ATS-parsable on its own — document this
  tradeoff in the template's own comments.
