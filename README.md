# Shorebird Area Search – mobile data entry

A single web page that replaces the 2-page paper datasheet. It works offline once opened,
saves as you go, and exports a CSV (one row per species) via the phone's Share menu.

## Files
- `index.html` – the whole app. The area list, species list and send-to address are at the top of the `<script>` (CONFIG section).
- `sw.js` – offline cache. **Bump `VERSION` whenever you edit any file** so phones pick up changes.
- `manifest.webmanifest`, `icon*.png`, `icon.svg` – home-screen install.

## Hosting (pick one; needs https for offline mode)
- **Netlify Drop** (easiest): go to app.netlify.com/drop and drag this `app` folder in.
- **GitHub Pages**: push this folder to a repo, Settings → Pages → deploy from branch.

## Volunteer setup (once, with signal)
- iPhone: open the link in Safari → Share → *Add to Home Screen*.
- Android: open in Chrome → ⋮ → *Add to Home screen* / *Install app*.

## Test locally
    python3 -m http.server 8765 --directory app
