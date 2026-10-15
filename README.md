# Cornerstone docs hub

Landing page for **https://docs.cornerstonedata.org**, served by GitHub Pages from `main`.

Each dataset's docs live in their own repo and are published into a folder here by that repo's GitHub Action:

| Path | Source repo |
|---|---|
| `/eeio/` | [`cornerstone-data/eeio-docs`](https://github.com/cornerstone-data/eeio-docs) |

Don't edit dataset folders by hand; they are overwritten on each deploy. To add a dataset, create a `<dataset>-docs` repo that publishes into `<dataset>/`, give it a deploy key with write access here, and add a card to `index.html`.

## Setup

- Settings → Pages: deploy from branch `main`, folder `/`; custom domain `docs.cornerstonedata.org`; enforce HTTPS.
- DNS (managed by Watershed): `CNAME docs → cornerstone-data.github.io`.
