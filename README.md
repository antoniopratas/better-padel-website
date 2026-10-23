# Better Padel website

Static promo site (no build step). Everything is in this folder.

## Hosting on GitHub Pages (free, repo must be public)

1. Repo Settings → Pages → Source: Deploy from a branch → `main` / `(root)` → Save.
2. Custom domain: type e.g. `padel.yourdomain.com` and save (this adds a `CNAME` file).
3. In Cloudflare DNS add a CNAME record: name `padel`, target `antoniopratas.github.io`,
   proxy **DNS only** (grey cloud) until GitHub shows the certificate is issued, then tick
   "Enforce HTTPS". You can turn the orange cloud on afterwards (SSL mode: Full).

Every push to `main` redeploys the site.

## Sign-up form

Sign-ups go to Formspree (`FORM_ENDPOINT` in `index.html`). Each one has email, platform
(garmin / apple / both), watch model and date. See and export them in the Formspree dashboard.

## Colour schemes

The public page uses Night court. Add `?schemes` to the URL to show the switcher
and compare the other three (Blue turf, Green turf, Carbon).
