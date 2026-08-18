# Task 01 — Repo Structure

## Goal
Create the skeleton directory layout so every later task has a home.

## Structure
```
awesome-html-resume-templates/
├── README.md
├── LICENSE
├── CONTRIBUTING.md
├── .gitignore
├── .github/
│   ├── ISSUE_TEMPLATE/
│   └── PULL_REQUEST_TEMPLATE.md
├── docs/                          # GitHub Pages gallery site (tasks 05, 08)
│   ├── index.html
│   ├── assets/
│   ├── sitemap.xml
│   └── robots.txt
├── assets/
│   ├── screenshots/                # one PNG/JPG per template, used in root README
│   └── og-image.png                # social preview image
├── templates/
│   ├── 01-minimalist/
│   │   ├── index.html
│   │   ├── style.css
│   │   └── thumbnail.png
│   ├── 02-modern-sidebar/
│   ├── 03-creative-portfolio/
│   ├── 04-ats-friendly/
│   ├── 05-developer-tech/
│   ├── 06-dark-mode/
│   ├── 07-timeline/
│   ├── 08-elegant-serif/
│   ├── 09-corporate-professional/
│   ├── 10-startup-founder/
│   ├── 11-academic-cv/
│   ├── 12-student-entry-level/
│   ├── 13-executive/
│   ├── 14-infographic/
│   ├── 15-gradient-colorful/
│   ├── 16-print-optimized/
│   ├── 17-two-column-compact/
│   ├── 18-designer-visual/
│   ├── 19-freelancer-consultant/
│   └── 20-rtl-multilingual/
└── tasks/                          # this planning folder
```

## Steps
1. Create the 20 `templates/<NN>-<slug>/` folders (slugs match the filenames under
   `tasks/templates/`).
2. Create `assets/screenshots/` and `docs/` placeholders.
3. Add a root `.gitignore` (OS/editor junk only — `.DS_Store`, `.vscode/`, `*.log`;
   no build artifacts, since there's no build step).
4. Commit the skeleton as the first commit (`chore: scaffold repo structure`).

## Acceptance criteria
- `find templates -maxdepth 1 -type d | wc -l` → 21 (20 templates + the `templates` dir itself).
- Git doesn't track empty directories — add a `.gitkeep` per empty template folder if
  committing the skeleton before each template has real content.
