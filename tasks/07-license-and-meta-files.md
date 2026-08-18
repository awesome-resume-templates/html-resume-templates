# Task 07 — License & Repo Meta Files

## Goal
Add the small files that make the repo look professional, legally clear, and
trustworthy — a trust/ranking signal, and required for others to legally reuse the templates.

## Deliverables
- `LICENSE` — MIT (permissive, matches the "free to use" promise in the README).
- `.gitignore` — OS/editor cruft only (`.DS_Store`, `.vscode/`, `*.log`); no build
  artifacts needed given the no-build-step decision.
- `.github/ISSUE_TEMPLATE/template-submission.md` — structured form for "I want to add a template".
- `.github/ISSUE_TEMPLATE/bug-report.md` — for reporting a broken template.
- `.github/PULL_REQUEST_TEMPLATE.md` — checklist referencing
  [09-qa-accessibility-checklist.md](09-qa-accessibility-checklist.md).
- `assets/og-image.png` — 1200×630 social preview image, used by the gallery page's
  Open Graph tags and by the GitHub repo's own social preview setting.

## Acceptance criteria
- GitHub repo Settings → Social preview image is set.
- Opening a new issue in the GitHub UI shows the template-submission/bug-report forms.
