# MealRadar legal-site

Static legal/support pages for the **MealRadar** app, kept isolated from the app
runtime code. They are written to match the app's current behavior (local-first
data with platform backups outside our control, Supabase auth, AI via a Supabase
Edge Function, in-app account deletion, subscriptions via Apple App Store and
Google Play).

These pages are public and referenced from the App Store and Google Play
listings. Keep them accurate: when app data practices change, update the pages
and the dates in the same change.

## Contents

- `index.html` — landing page linking to the resources below
- `privacy.html` — privacy policy
- `terms.html` — terms of use
- `support.html` — support / help page
- `delete-account.html` — account & data deletion instructions
- `styles.css` — self-contained styles (no external fonts/CDNs/scripts)

## Preview locally

No build step. Just open `index.html` in a browser (double-click it, or drag it
into a browser window), then follow the links. All links are relative, so the
pages work from any base path.

## Publishing (GitHub Pages)

This repo is served by GitHub Pages. Pushing to `main` publishes — there is no
separate build or deploy step, and no staging environment, so review before you
push.

The Pages source is configured in the repo's **Settings → Pages**, not in this
repo, so confirm it there if a push ever appears not to take effect. If the
setup changes later, the alternatives are "Deploy from a branch" using `main` /
`docs`, or a dedicated `gh-pages` branch.

## Dates

`privacy.html` carries both an effective date and a last-updated date;
`terms.html` carries a last-updated date. Update the last-updated date whenever
page content changes.

## Maintenance checklist

Items below are verification steps. Confirm each against the live site and the
store consoles rather than assuming — this repo cannot prove any of them.

- [ ] Verify the public URL for each page resolves.
- [ ] Verify the App Store Connect Privacy Policy URL points to `privacy.html`.
- [ ] Verify the App Store Support URL points to `support.html`.
- [ ] Verify the Google Play privacy policy URL points to `privacy.html`.
- [ ] Verify the Google Play account/data deletion URL points to
      `delete-account.html`.
- [ ] Verify page content still matches actual app behavior after each release.
- [ ] Review with legal counsel if desired.

The real support email (`support@mealradar.xyz`) is already set in the pages.
