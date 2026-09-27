# The Threshold Collection — DUT Academic Library

Academic digital library for ICTB301 (Department of Information Systems, DUT).
31 open-access items in 4 collections, each described with Dublin Core metadata.

## Folder contents
- `index.html` — the whole website (catalogue, search, browse, metadata records)
- `docs/` — 13 PDF/EPUB files stored with the site (all Creative Commons or public government documents)
- `netlify.toml` — tells Netlify to publish this folder and download files in `docs/`
- `threshold_dublin_core.csv` — the same metadata as a CSV (can be imported into Omeka)

## Put it on GitHub
1. Create a new repository on github.com (e.g. `threshold-collection`).
2. Click **Add file → Upload files** and drag in everything in this folder (keep the `docs` folder).
3. Click **Commit changes**.

## Connect GitHub to the existing Netlify site
1. app.netlify.com → open **reliable-belekoy-2a2d21**.
2. **Site configuration → Build & deploy → Continuous deployment → Link repository**.
3. Pick GitHub → your repository. Branch `main`, build command empty, publish directory `.` → **Deploy**.
The link stays the same. Every future commit redeploys automatically.

## Add an item
Open `index.html`, search for `HOW TO ADD AN ITEM`, copy one `{ ... }` block and edit it.
If you have the PDF, put it in `docs/` and set `pdf:"docs/FileName.pdf", local:true`.
Only add files whose licence allows sharing (CC BY, CC BY-SA, CC BY-NC, CC BY-NC-SA, public domain).
