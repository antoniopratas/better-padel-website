# Better Padel website

Static promo site (no build step). Everything is in this folder.

## Hosting (Cloudflare Pages, connected to this repo)

- Production branch: `main`. Every push to `main` deploys the live site.
- Build command: none. Build output directory: `/` (the repo root).
- Any other branch (e.g. `preview`) gets its own preview URL, `<branch>.<project>.pages.dev`,
  so changes can be checked before they go to `main`.
- The custom domain is set in the Pages project under Custom domains; Cloudflare manages the
  DNS record and HTTPS.

## Sign-up form

Sign-ups go to Formspree (`FORM_ENDPOINT` in `index.html`). Each one has email, platform
(garmin / apple / both), watch model and date. See and export them in the Formspree dashboard.

## Colour schemes

The public page uses Night court. Add `?schemes` to the URL to show the switcher
and compare the other three (Blue turf, Green turf, Carbon).
