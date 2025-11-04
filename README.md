# iLRN-XRRepository

A searchable, filterable directory of XR resources hosted on **GitHub Pages**.

## Live site
After enabling Pages, your site will be at: **https://AndreaHorvath-fhcw.github.io/iLRN-XRRepository/**

## How it works
- Static site in `index.html` uses [Tabulator] to render `data/resources.json`.
- Users click **Add Resource** (GitHub Issue Form).
- The **Add Resource PR** workflow reads the issue and opens a PR that appends to `data/resources.json`.
- Merging to `main` triggers the **Deploy GitHub Pages** workflow.

## Setup

1. **Upload these files** to the repo root (keep the same structure).
2. In GitHub: **Settings → Pages**:
   - Set **Build and deployment** → **Source: GitHub Actions** (the included workflow will deploy).
3. (Optional) Customize categories in `.github/ISSUE_TEMPLATE/add-resource.yml`.
4. Add initial data to `data/resources.json` if you wish.

## Manual edits
You can also directly edit `data/resources.json` and commit to `main`—the site will redeploy automatically.
