# The Scoville Atlas

Interactive Mapbox map plotting the origin of 166 chili pepper varieties, colored by Scoville heat (yellow → red on a log scale).

## Files

- `index.html` — the map (Mapbox GL JS, styled with the `primateco` custom style)
- `chilis.geojson` — the underlying dataset (name, species, origin, coordinates, Scoville min/max/avg, source URL)

## Deploy (GitHub Pages)

```bash
# from this folder
git init
git add .
git commit -m "Initial commit: Scoville Atlas map"
git branch -M main
git remote add origin https://github.com/<your-username>/<repo-name>.git
git push -u origin main
```

Then on GitHub: **Settings → Pages → Source: Deploy from branch → Branch: main, folder: / (root) → Save**.
The site will be live at `https://<your-username>.github.io/<repo-name>/` within a minute or two.

## Data

The source-of-truth spreadsheet lives in Google Sheets. If you edit it there, re-export as CSV/GeoJSON and replace `chilis.geojson` in this repo, then commit + push to update the live map.
