# Template 16 — Print-Optimized (`templates/16-print-optimized/`)

## SEO angle
Targets: "printable resume template html", "print ready resume template".

## Who it's for
People who mainly care about a physical/PDF printout looking perfect (less concerned
with on-screen flourish).

## Layout & sections
Standard single column, tuned specifically to A4 and US-Letter page dimensions with
exact margins.

## Style direction
- Intentionally conservative on-screen styling. The differentiator is that its print
  handling is the most rigorously tuned of all 20 templates: explicit page-break
  rules, exact `@page` margins, no element ever crossing a page boundary.

## Customization points
- `--page-size: A4 | Letter` documented toggle.

## Acceptance criteria
- Follows all rules in `../02-design-system.md`.
- Passes `../09-qa-accessibility-checklist.md`.
- Serves as the reference implementation for print quality — its *approach* (not its
  code, per the self-contained-folder rule) should inform print-CSS polish on the
  other 19 templates.
