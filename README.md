# Men's Companion

Android companion app for the **a.intimstory.ltd** directory — browsing plus a photo‑dedup intelligence layer that tells you which profiles are actually the same person.

## Screenshots

| Card‑density heatmap | "Find same" matches | Profile |
|:---:|:---:|:---:|
| ![Heatmap](docs/screenshots/heatmap.png) | ![Find same](docs/screenshots/find-same.png) | ![Profile](docs/screenshots/card.png) |
| **Browse the directory** | **Parametric search** | **Per‑card map** |
| ![Feed](docs/screenshots/feed.png) | ![Search](docs/screenshots/search.png) | ![Map](docs/screenshots/map.png) |

<p align="center">
  <img src="docs/screenshots/heatmap-cell.png" width="280" alt="Tap a heatmap cell to list its cards">
  <br><em>Tap a heatmap cell to list the cards there.</em>
</p>

## How it works

The app is a smarter front‑end for the existing **a.intimstory.ltd** website — it does **not** host or copy the directory.

- **The site is the source of all card content.** Listings and profiles are fetched live from `a.intimstory.ltd` (from your own connection) and parsed **on your device**. The app shows you the same cards the website does, just in a faster, app‑native UI.
- **You use your own site account.** Sign‑in goes **directly to the site**; the same account drives your saved list, reviews and scores. The app only acts on your behalf.
- **A small server adds the intelligence.** The one thing the website can't tell you is *which different cards are really the same person*. A backend service has fingerprinted the directory's photos (perceptual image hashing) and indexed phone numbers, so the app can answer:
  - **"Find same / Related"** — other cards that share the *same photos* (with how many photos match and how close they are), and cards that share the *same phone* across the whole site.
  - **Card‑density heatmap** — where profiles are concentrated across the city; tap a cell to list the cards in it.
  - This server returns **only relationships** (which IDs relate, match counts, coordinates) — never the card photos or text, which always come straight from the site.

In short: **content comes from the site, insight comes from the app.**

## Features

- Browse the directory (All / Elite / New / Top100 / Saved), parsed on‑device.
- **Related / "find same"** — cards that share the same photos (image fingerprint matching) or the same phone.
- Search by phone / ID, by parameters (age, bust, height, weight, price), and by **metro / area** (with optional neighbouring stations).
- Client‑side **filters** (status, price, age, bust, height, weight, location).
- **Card‑density heatmap** of the city — tap a cell to list the cards there.
- Per‑card **map** with the distance from you.
- Saved list, **reviews & scoring**, full‑screen photo viewer with zoom.

## Install

1. Download the latest `mens-companion-<version>.apk` from **[Releases](../../releases)**.
2. Open it on your phone and allow installing from your browser / file manager.
3. Requires **Android 8.0+**. Sign in with your site account for the saved list and reviews.

---
*This repository hosts the app release only — the source code is not published.*
