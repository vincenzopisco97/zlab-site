# Z Lab — Website (linked build, production-ready)

Multi-page static site. Lightweight HTML pages sharing one external `style.css` and logo assets. No build step, no dependencies.

## Files (deploy ALL together, same folder)

index.html · sectors.html · capabilities.html · company.html · careers.html · contact.html
style.css · logo-light.png · logo-dark.png · favicon.png · .nojekyll

The logo (top-left) links to index.html on every page. Mega-menu sub-links jump to anchors within Sectors / Capabilities / Company.

## Deploy on GitHub Pages (free)

1. Create a public repo, e.g. `zlab-site`.
2. From this folder:
   ```bash
   git init
   git add .
   git commit -m "Z Lab site"
   git branch -M main
   git remote add origin https://github.com/<YOUR-USER>/zlab-site.git
   git push -u origin main
   ```
3. GitHub → Settings → Pages → Source: Deploy from a branch → main / (root) → Save.
4. Live at https://<YOUR-USER>.github.io/zlab-site/

## Edit

- Styling: edit `style.css` once → applies to all pages.
- Logo: replace `logo-light.png` (for white backgrounds) and `logo-dark.png` (for dark backgrounds), keep same filenames.

## Placeholders to finalise

- Client list (`// Client list to be finalised`)
- Careers open roles (`// Specific open roles to be added`)
- Confirm ISO 17025 / accreditation wording on company.html

## Note on local preview

Open `index.html` by double-click: styling and navigation work because all files sit together.
Opening a single page in an isolated sandbox (with no sibling files) will show it unstyled — that is expected, not a bug.
