# Avionics 🎧

**A bird vocalization quiz app.** Train your ear to identify birds by their calls and songs using real field recordings.

🌐 **Live site:** [falsemisfortune.github.io/Avionics](https://falsemisfortune.github.io/Avionics)

---

## Features

- Real recordings pulled live from [xeno-canto.org](https://xeno-canto.org) (quality A only)
- Optional [eBird API](https://ebird.org/api/keygen) integration for taxonomy-aware distractors
- Three difficulty levels:
  - **Easy** — distractors from different families
  - **Medium** — distractors from the same family
  - **Hard** — distractors from the same order + 15-second autoplay timer
- 8 regions: North America, UK & Ireland, Europe, Australia, India, South Africa, Brazil, Mexico
- Installs as a PWA — add to home screen on iOS/Android for a native-like experience
- No server, no account required — runs entirely in the browser

## Data Sources

| Source | What it provides |
|--------|-----------------|
| [xeno-canto](https://xeno-canto.org) | Bird audio recordings (CC licensed) |
| [eBird API](https://ebird.org/developer/api) | Regional species lists + taxonomy (free key required) |

## Using the eBird Key

The app works without a key using built-in fallback species lists. To unlock smarter distractors based on real taxonomy (same family/order grouping):

1. Register at [ebird.org/api/keygen](https://ebird.org/api/keygen) — it's free and instant
2. Paste your key into the key field in the app
3. The app will fetch the real species checklist for your selected region

## Running Locally

No build step required — it's a single HTML file.

```bash
git clone https://github.com/falsemisfortune/Avionics.git
cd Avionics
# open index.html in your browser, or serve with:
npx serve .
```

## Deployment

Hosted via GitHub Pages from the `main` branch root.

To deploy your own fork:
1. Fork this repo
2. Go to Settings → Pages → Source: `main` branch, `/ (root)`
3. Your site will be live at `https://YOUR_USERNAME.github.io/Avionics`

## Credits

- Recordings © their respective recordists via [xeno-canto.org](https://xeno-canto.org)
- Species data © [Cornell Lab of Ornithology / eBird](https://ebird.org)

## License

MIT — do whatever you like with the code. Respect xeno-canto and eBird's own terms for their data.
