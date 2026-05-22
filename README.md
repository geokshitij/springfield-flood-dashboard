# Springfield Township Flood Dashboard

Static, single-page dashboard summarizing the AGU Thriving Earth Exchange
flood-risk findings for Springfield Township, Bucks County, PA.

**Live site:** https://geokshitij.github.io/springfield-flood-dashboard/

This repository contains only the published dashboard (HTML, CSS, figures,
embedded interactive map). The underlying analysis code and raw data live
in a separate private repository maintained by the project team; data and
code are shared on request through the Contact section of the dashboard.

```
springfield-flood-dashboard/
├── index.html                    one-page dashboard
├── css/style.css                 styling
└── assets/
    ├── susceptibility_map.png    static map (D1)
    ├── susceptibility_map.html   interactive Leaflet map (D1)
    ├── precip_summary.png        precipitation extremes (D2)
    ├── sensitivity_bars.png      AHP weight sensitivity (D1)
    ├── flood_points_ranked.png   6-site ranking (D3)
    └── cmip6_uplift.png          CMIP6 climate uplift (D4)
```

Total ~3 MB. No JavaScript dependencies beyond the embedded Leaflet in
`susceptibility_map.html` (loaded from a CDN).

## Preview locally

```bash
python3 -m http.server 8000
# open http://localhost:8000
```

## GitHub Pages

Pages serves the contents of this repository's `main` branch root. After
push, GitHub builds the site at the URL above within about a minute.

To enable Pages on a fresh clone:

```
Settings → Pages → Source: "Deploy from a branch" → Branch: main, folder: /
```

## Updates

This repo is regenerated from the private source repo. The maintainer
copies in the latest `site/` contents and pushes; nothing is built here.

## Contact

The Contact section on the live dashboard lists the project team. Data
and code requests should go through those addresses.
