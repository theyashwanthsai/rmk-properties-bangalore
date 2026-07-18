# RMK Properties Bangalore

A static property listings site for RMK Properties — residential and rental income properties across South-East Bangalore (Electronic City, Sarjapur Road, HSR Layout, ITI Layout, Gattahalli).

## Features

- 5 property listings with photos, specs, and rental income details
- Live filtering by keyword, property type, and area
- Expandable "View Details" specs on each card (khata, water source, units, legal status)
- Fully responsive, single-file site — no build step, no dependencies

## Structure

```
index.html    — the entire site (HTML + CSS + JS)
images/       — hero banner and property thumbnails
```

## Run locally

Just open `index.html` in a browser, or:

```
python3 -m http.server 3000
```

## Deploy on Vercel

1. Go to [vercel.com/new](https://vercel.com/new) and import this repository
2. Framework preset: **Other** — no build command, no output directory needed
3. Deploy

Or with the CLI:

```
npx vercel --prod
```

## Adding / editing properties

Each listing is an `<article class="card">` block in `index.html`. Copy an existing block, update the text, drop a photo into `images/`, and point the `<img src>` at it. The `data-type` and `data-text` attributes drive the filters.
