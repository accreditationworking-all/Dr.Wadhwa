# Dr. Lalit Kumar Wadhwa — Personal Website

A single-page, static website (no build step). Works on GitHub Pages, Netlify, or any web host.

## Files
- `index.html` — the whole site (styles + scripts inline)
- `assets/photo.jpg` — profile photo (replace with a higher-resolution square photo for a sharper look; keep the same file name)

## Deploy on GitHub Pages (new account)
1. Sign in to the GitHub account you want to use and create a **new public repository** (e.g. `lalitwadhwa` or `<username>.github.io`).
2. Click **Add file → Upload files**, drag in `index.html`, `README.md` and the `assets` folder, then **Commit changes**.
3. Go to **Settings → Pages**. Under *Build and deployment* choose **Deploy from a branch**, branch **main**, folder **/ (root)**, then **Save**.
4. After 1–2 minutes the site is live at:
   - `https://<username>.github.io/<repo-name>/`, or
   - `https://<username>.github.io/` if the repo is named `<username>.github.io`.

## Editing content
All lists live in the `<script>` at the bottom of `index.html`:
- `career` — leadership journey
- `svcs` — the 9 areas of university support
- `P` — publications (`'J'` journal, `'C'` conference, `'B'` book)
- `pats` — patents · `aws` — awards · `ws` — workshops
- Citations chart: `cites` array (update yearly from Google Scholar)

The contact form opens the visitor's email app addressed to wadhwalalitkumar@gmail.com (cc director.iqac@vupune.ac.in), so no server is needed.

## Chat assistant
The floating chat button runs entirely in the browser (no API key, no server, nothing sent anywhere).
Its answers live in the `KB` array in `index.html` — each entry is a keyword pattern (`k`) and a reply (`a`).
Questions like "papers on ZigBee" are answered by searching the publication list automatically.

## Visualisations
- Research topics donut — topics are assigned by keyword rules in `TOPICS`
- Collaboration constellation — co-authors listed in `COS`
- Publications by year, career ribbon (`RB`), citations chart, readiness radar

## Intro video
`assets/intro.mp4` (71 s, 1280×720, narrated, ~4 MB), captions in `assets/intro.vtt`, with poster `assets/intro-poster.jpg`. Chapter times are in the `CH` array in `index.html`.

## Palettes & extras
- Colour palettes: Iris (default), Ocean, Blossom — palette button in the top bar; tokens at the top of the `<style>` block
- Chat assistant: voice input (mic) and read-aloud answers where the browser supports it
- QR code in Contact points to https://accreditationworking-all.github.io/Dr.Wadhwa/
