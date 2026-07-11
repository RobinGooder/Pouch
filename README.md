# $POUCH — Robinhood Chain memecoin site

Static one-page site for **$POUCH**. No build step, no framework — just `index.html` and image assets. Deploys as-is to GitHub Pages, Netlify, or Vercel.

## Files
```
index.html              the whole site (HTML + CSS + JS inline)
favicon.png             browser tab icon (the pouch)
apple-touch-icon.png    home-screen icon (iOS)
assets/
  pouch.png             hero pouch artwork (transparent)
  coin.png              coin used in the loot counter + tap animation
  logo.png              1000x1000 logo on black — use for the NOXA launchpad + socials
  logo-transparent.png  1000x1000 logo, transparent background
  og.png                social share/link-preview image (1200x630)
```

## Deploy

### GitHub
1. Create a new repo (e.g. `pouch-site`).
2. Upload every file **keeping the `assets/` folder** (drag the whole folder in on desktop, or add files preserving paths on mobile).

### Netlify
- New site → Import from GitHub → pick the repo.
- Build command: *(leave empty)*  ·  Publish directory: `/`  → Deploy.

### Vercel
- Add New Project → import the repo → Framework preset: **Other** → Deploy. (No config needed.)

### GitHub Pages (optional)
- Repo Settings → Pages → Source: `main` / root → Save.

## After you launch the coin
Open `index.html` and:
1. Find `const CA = ""` near the bottom → paste your $POUCH contract address between the quotes.
2. In the footer, replace the `#` links with your real **X** and **Telegram** URLs.
3. (Optional) Wire the "View chart" button to your DexScreener/GeckoTerminal link.

## Notes
- The price/percentage in the header is a **playful gag** that ticks up when you tap the pouch — it is not live data.
- If the favicon doesn't update after deploy, it's browser cache: hard-refresh or open a private tab.
- $POUCH is a memecoin / community art project. Not affiliated with Robinhood Markets, Inc. or NOXA. Not financial advice.
