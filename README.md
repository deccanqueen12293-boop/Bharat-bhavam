# Bhava Sambandha · भाव सम्बन्ध

An offline, single-file Vedic astrology lab for studying how houses relate to each other. Cast a chart from birth details, pick two or more houses, and read the possible outcomes by area of life — job, health, children, marriage, wealth and more.

**Live app:** `https://<your-username>.github.io/bhava-sambandha/`

## What it does

- **Chart** — cast from date, time and place of birth (Lahiri ayanamsa, mean or true node, whole-sign houses), or enter planets by hand, by planet or by house. North Indian diamond chart; tap houses to select them.
- **Analyse** — finds how the chosen houses are linked (exchange, lord placement, conjunction, aspect, nakshatra-lord and dispositor links), scores each link, flags yogas, and lists outcomes per life area with the matching BPHS verses.
- **Dasha** — Vimshottari from Mahadasha down to Prana, with a date checker. Send any dasha lord's houses straight to Analyse.
- **Compare** — up to four houses, planets, rashis or nakshatras side by side, with a combination reading for each pair.
- **Library** — houses (with 600 significations), planets, rashis, nakshatras, all 144 lord-in-house verses, benefics by lagna, and your own notes.
- **Web** — search Google, Wikipedia, Wisdom Library or Archive.org; Wikipedia summaries load inside the app when online.

Light and dark themes. Works fully offline; charts and notes stay in the browser's local storage.

## Sources

- Brihat Parashara Hora Shastra, G.C. Sharma translation (lord-in-house verses)
- Personal study notes: planets and houses, Bhavat Bhavam lord notes
- Vedic 600 house significations and 30-attribute tables for planets, rashis and nakshatras
- Astronomy engine from Grahakosha Journal: Meeus ch. 47 Moon, Meeus ch. 25 Sun, JPL Keplerian elements for planets with precession to date

## Accuracy

Sun and Moon are within arc-seconds. Planets use JPL approximate elements — typically within a few arc-minutes, and Jupiter or Saturn can be off by up to about 10′. Check key charts against a reference such as AstroSage before relying on degree-sensitive results.

Readings are traditional interpretations, not certainties.

## Deploy on GitHub Pages

1. Create a repository named `bhava-sambandha` and upload `index.html`, `README.md` and `.nojekyll`.
2. Go to **Settings → Pages**, set **Source** to *Deploy from a branch*, branch `main`, folder `/ (root)`, and save.
3. The app appears at `https://<your-username>.github.io/bhava-sambandha/` within a minute or two.

## Android

To wrap it as an APK, load `index.html` in a WebView through `WebViewAssetLoader` (served over `https://`) so local storage persists.
