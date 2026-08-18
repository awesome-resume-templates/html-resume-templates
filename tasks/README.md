# Project Task Breakdown

Implementation plan for **awesome-html-resume-templates**, split into small, independent
tasks. Work through the core tasks roughly in order; the 20 template tasks in
`templates/` can be done in any order, in parallel, or by different contributors.

## Core tasks

1. [00-overview.md](00-overview.md) — goals, tech decision, success criteria
2. [01-repo-structure.md](01-repo-structure.md) — folder/file layout for the whole repo
3. [02-design-system.md](02-design-system.md) — shared conventions every template must follow
4. [03-template-customization-guide.md](03-template-customization-guide.md) — end-user "how to customize" doc
5. [04-readme-seo.md](04-readme-seo.md) — SEO-optimized root README content plan
6. [05-gallery-index-page.md](05-gallery-index-page.md) — live demo gallery site (GitHub Pages)
7. [06-contributing.md](06-contributing.md) — contribution guide for new templates
8. [07-license-and-meta-files.md](07-license-and-meta-files.md) — LICENSE, issue/PR templates, social preview
9. [08-github-pages-deployment.md](08-github-pages-deployment.md) — hosting + sitemap/robots for SEO crawling
10. [09-qa-accessibility-checklist.md](09-qa-accessibility-checklist.md) — pre-merge checklist for every template

## Template tasks (20)

See [templates/](templates/) — one file per resume template, `01-minimalist.md` through
`20-rtl-multilingual.md`. Each is independently buildable and lists its own SEO keyword
target, layout, style direction, and acceptance criteria, on top of the shared rules in
`02-design-system.md`.

## Suggested order

`00 → 01 → 02 → 03`, then build templates 1–3 as a proof of concept against those
conventions, then `04–09` (README/gallery/infra) can proceed in parallel with the
remaining 17 templates.
