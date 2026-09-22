# Root Cause Analysis Report

Static single-page dashboard (`index.html`) for corrective maintenance
work orders — License Plate Service Section.

## Live data source
Data can come from either:
1. A Google Sheet via an Apps Script Web App (see `Code.gs` in the parent
   project / chat history) — set the URL in `CONFIG.GOOGLE_SHEET_API_URL`
   near the top of the `<script>` block in `index.html`.
2. Manual Excel import (the "Import Excel File" menu item) as a fallback.

## Deploy
This is a static site with no build step.
1. Push this repo to GitHub.
2. On vercel.com: **New Project** → **Import Git Repository** → select this repo.
3. Framework preset: **Other** (no build command needed).
4. Deploy.

Every push to the main branch redeploys automatically.
