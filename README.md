# Gracious Path website

The public website for the Gracious Path iPhone and iPad app, served free
with GitHub Pages. The app itself lives in a private repository.

| Page | Address |
| --- | --- |
| Home (landing page) | `/` |
| Privacy policy and terms | `/privacy/` (the URL to give Apple) |

The site makes no requests to anyone else: fonts and images are served
from here, and there are no analytics or trackers.

## Pointing graciouspath.app here (once it is registered)

1. At the domain registrar, add these DNS records for `graciouspath.app`:
   - four `A` records: 185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153
   - a `CNAME` record for `www` pointing to `bubblycornflakes.github.io`
2. In this repository on GitHub: Settings → Pages → Custom domain →
   `graciouspath.app` → Save, then tick "Enforce HTTPS" once offered
   (.app addresses only work over HTTPS).
3. Update the `og:url` and `og:image` addresses at the top of `index.html`
   to `https://graciouspath.app/`.
4. Give Apple `https://graciouspath.app/privacy/` as the privacy policy URL.

## When the app is live

Replace the two "Coming soon to the App Store" badges in `index.html` with
links to the App Store page (Apple's official badge artwork and rules are
at developer.apple.com/app-store/marketing/guidelines).
