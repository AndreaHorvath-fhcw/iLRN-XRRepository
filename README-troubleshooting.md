## If issues aren't turning into PRs

1. Open **Actions** tab — do you see a run for “Add Resource PR”?
   - If not: ensure the workflow file exists at `.github/workflows/add-resource-pr.yml`.
   - Ensure **Settings → Actions → General → Workflow permissions** is set to **Read and write**.
2. Open a recent run → **Logs**. Common causes:
   - Missing required fields in the issue form.
   - Invalid URL.
3. After the PR is created, **merge** it to `main` so the page updates.
4. Pages deploys from GitHub Actions; check the “Deploy GitHub Pages” run after merge.
