# Task 08 — GitHub Pages Deployment & Crawlability

## Goal
Host the `docs/` gallery site publicly and make sure search engines can find and index it.

## Steps
1. Repo Settings → Pages → deploy from `main` branch, `/docs` folder.
2. Add `docs/sitemap.xml` listing the gallery page plus every template's live URL.
3. Add `docs/robots.txt` allowing all crawlers and pointing at the sitemap.
4. Add the live Pages URL to the README badges/intro and to the GitHub repo's "About"
   website field (an actual SEO/traffic signal, not just cosmetic).
5. Verify indexing with Google Search Console — this is a manual step for the repo
   owner (requires their Google account), just document it here; not something Claude
   can perform.

## Acceptance criteria
- `https://<org>.github.io/awesome-html-resume-templates/` loads the gallery.
- `sitemap.xml` and `robots.txt` are both reachable and valid.
