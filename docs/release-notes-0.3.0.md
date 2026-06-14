**Men's Companion 0.3.0**

### What's new
- **Exact address on the map** — when a card lists a specific street address, the per-card map now drops a pin on the **precise spot** (using the site's own geocoding) instead of an approximate metro-area circle. Vague or partial addresses still show the area, so the pin is never misleadingly precise.
- **Zoom-adaptive density heatmap** — the city heatmap mesh now **gets finer as you zoom in** (≈1 km → 500 → 250 → 125 → 62 m), re-binning the area you're viewing so you can drill into a neighbourhood, not just the city as a whole. The current cell size is shown in the title bar.
- The card-location map also reads the site's coordinate directly, so it's robust to address-formatting variants.
- **"Locate me" button** on the card map — refreshes your current position on demand (the ♂ marker, the distance, and the map all update). Tip: grant **Precise** location so it can use GPS.

### Install
1. Download `mens-companion-0.3.0.apk` below.
2. Open it on your phone and allow installing from your browser / file manager.
3. Requires **Android 8.0+**. Sign in with your **a.intimstory.ltd** account for the saved list and reviews.

*Content always comes live from the site; credentials go directly to the site, not a third-party server. Source code is not published; this repository hosts the release only.*
