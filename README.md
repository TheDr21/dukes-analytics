# Lady Dukes Analytics

Static site for WPA Lady Dukes 10U stats dashboards.

## Files

| File | Description |
|------|-------------|
| `index.html` | Landing page / hub |
| `lady_dukes_10u_stats_dashboard.html` | Season overview |
| `lady_dukes_deep_dive.html` | Deep dive (6 tabs) |
| `lady_dukes_ultra_deep.html` | Ultra deep analytics |
| `dukes_lineup_and_11u_projection.html` | Lineup + 11U projection |

## How to deploy on GitHub Pages

1. Go to [github.com](https://github.com) and create a free account
2. Click **New repository** → name it `dukes-analytics` → set to **Public** → click **Create**
3. Click **Add file → Upload files** and drag ALL the HTML files in at once
4. Click **Commit changes**
5. Go to **Settings → Pages**
6. Under "Source" select **Deploy from a branch**, choose `main`, folder `/root`, click **Save**
7. Wait ~60 seconds, then visit `https://yourusername.github.io/dukes-analytics`

## Adding a new dashboard

1. Save the new HTML file from Claude
2. Upload it to the repo (drag into GitHub)
3. Open `index.html`, copy any `<a class="dash-card">` block, update the `href`, title, and description
4. Commit — live in under a minute

## Viewing locally

```bash
# From the folder containing your HTML files:
python -m http.server 8000
# Then open http://localhost:8000 in your browser
```
