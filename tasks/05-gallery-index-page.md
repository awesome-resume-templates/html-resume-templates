# Task 05 — Live Gallery / Demo Site

## Goal
Build `docs/index.html`: a single static page listing all 20 templates as cards
(thumbnail, name, tags, "View live" + "Get code" buttons), deployed via GitHub Pages.
This is the crawlable, linkable "product" of the repo — a live, fast, indexable page
ranks better than a README alone, and it lets people preview before downloading.

## Requirements
- Plain HTML/CSS, same zero-build-step philosophy as the templates themselves.
- Responsive card grid.
- Each card links to the live-hosted template (e.g.
  `templates/<slug>/index.html` relative to the Pages root) plus a link to the folder
  on GitHub for the source.
- `<title>` and `<meta name="description">` optimized for "html resume templates".
- Open Graph tags (`og:title`, `og:description`, `og:image` → `assets/og-image.png`)
  so shared links render well on social/Slack/Twitter.
- Optional vanilla-JS client-side filter by tag (e.g. "dark", "ATS-friendly",
  "one-page") — nice to have, not a hard requirement.

## Acceptance criteria
- Page lists all 20 templates with working live-preview links.
- Passes a basic Lighthouse SEO + performance check (nothing blocking, no oversized assets).
