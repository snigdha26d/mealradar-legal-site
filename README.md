# MealRadar legal-site

Static legal/support pages for the **MealRadar** app, kept isolated from the app
runtime code. These are **launch-support drafts, not legal advice**, written to
match the app's current behavior (local-only data, Supabase auth, AI via a
Supabase Edge Function, in-app account deletion).

## Contents

- `index.html` — landing page linking to the resources below
- `privacy.html` — privacy policy draft
- `support.html` — support / help page
- `delete-account.html` — account & data deletion instructions
- `styles.css` — self-contained styles (no external fonts/CDNs/scripts)

## Preview locally

No build step. Just open `legal-site/index.html` in a browser (double-click it,
or drag it into a browser window), then follow the links.

## Publishing later (GitHub Pages)

These are static files, so they can be published as-is. Options when you're ready:

- **Project Pages from `/docs`:** copy this folder's contents into a `docs/`
  folder on the default branch and enable GitHub Pages → "Deploy from a branch"
  → `main` / `docs`. Pages will be served at
  `https://<user>.github.io/<repo>/`.
- **Separate repo / `gh-pages` branch:** push these files to a dedicated repo or
  branch configured for Pages.
- **`/legal` path:** if hosting elsewhere later, keep relative links (they
  already are) so the pages work under any base path.

(Do not publish until the TODOs below are done.)

## TODO before publishing

- [ ] Confirm the final public URLs for each page.
- [ ] Update the App Store Connect Privacy Policy URL.
- [ ] Update the App Store Support URL.
- [ ] Update the Google Play privacy policy URL.
- [ ] Update the Google Play account/data deletion URL (point to `delete-account.html`).
- [ ] Review with legal counsel if desired.
- [ ] Keep pages updated when app data practices change.

The real support email (`support@mealradar.xyz`) is already set in the pages.
