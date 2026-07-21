## What's Automated

1. `Refresh F1 Data` runs every 30 minutes (and on manual dispatch).
2. It updates `data/content.json` from the Ergast API.
3. If content changed, it commits/pushes to `main`.
4. `Deploy Static Site to GitHub Pages` runs on:
   - direct push to `main`
   - successful completion of `Refresh F1 Data`
5. Pages is redeployed automatically.

## Manual Run

From GitHub Actions tab, run:
- `Refresh F1 Data` to pull latest data now.
- `Deploy Static Site to GitHub Pages` to redeploy now.
