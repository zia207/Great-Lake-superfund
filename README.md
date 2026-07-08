# Great Lakes Superfund Atlas

Interactive dashboard of EPA National Priorities List (Superfund) sites and Great Lakes Areas of Concern within the Great Lakes watershed.

## Live site

After GitHub Pages is enabled, the dashboard will be available at:

**https://zia207.github.io/Great-Lake-superfund/**

## Local preview

Open `index.html` in a browser, or run a local server:

```bash
python3 -m http.server 8000
```

Then visit http://localhost:8000

## GitHub Pages setup

1. Create a repository on GitHub named `Great-Lake-superfund` (if it does not exist yet).
2. Push this branch to GitHub:

   ```bash
   git remote add origin https://github.com/zia207/Great-Lake-superfund.git
   git push -u origin main
   ```

3. In the repository on GitHub, go to **Settings → Pages**.
4. Under **Build and deployment**, set **Source** to **GitHub Actions**.
5. Push to `main` (or re-run the **Deploy GitHub Pages** workflow). The site deploys automatically on each push.

## Files

| File | Purpose |
|------|---------|
| `index.html` | GitHub Pages entry point (same dashboard as below) |
| `great_lakes_superfund_dashboard.html` | Source dashboard file |
| `great_lakes_tributaries.geojson` | Major Great Lakes tributaries (from `great_lakes_river_network.kmz`, HUC-2 region 04) |
| `great_lakes_river_network.kmz` | Source river network layer |
| `RENEW_logo.png` | Header logo |

## Features

- Expanded chemical inventory per site (PFAS, BFR, pesticides, PPCPs, and legacy contaminants)
- Downloadable contaminant database (CSV or Excel) of all site–contaminant relationships
- Major tributaries map layer with toggle
- Prominent lake basin labels on the map
- Map export as **PDF** or **PNG** with customizable styling (basemap, watershed, rivers, symbols, lake labels)
- **USA Topographic** basemap (Esri) alongside satellite and street layers

## Creator

Zia Ahmed, PhD — Data and Visualization Scientist
