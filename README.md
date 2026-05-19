# devo-legal — SUNSET 2026-05-19

**This repo is no longer the canonical legal-page host.** All legal pages migrated to `devo.fyi/*` on apex 2026-05-19. The HTML files in this repo are now redirect shells that send visitors to the new location.

New canonical URLs:
- Privacy: https://devo.fyi/privacy.html
- Terms: https://devo.fyi/terms.html
- Support: https://devo.fyi/support.html
- Delete account: https://devo.fyi/delete-account.html
- Landing: https://devo.fyi/

Canonical source repo for legal HTML: https://github.com/morningdewll/devo-site

## Why the migration

- Apex `devo.fyi` is now the marketing landing page
- Single-domain footprint reads more professionally in app store listings
- Removes the awkward `morningdewll.github.io/devo-legal/*` URL in app metadata
- Path-based on apex (B1 — flat `.html` paths) chosen over `legal.devo.fyi` subdomain (original deferred spec) since the apex is occupied

## Old contents preserved

The full legal text (privacy + terms + support + delete-account) was copied to `devo-site` before the redirect shells overwrote this repo's HTML. Use the new repo for any future edits.

## App store URL swap

After Apple v1.0 approval + Play production-promote, swap the legal URLs in:
- ASC → App Information → Privacy Policy URL → `https://devo.fyi/privacy.html`
- Play Console → Store presence → Main store listing → Privacy Policy → `https://devo.fyi/privacy.html`

Until that swap happens, both old (`morningdewll.github.io/devo-legal/*` → redirects via this repo) and new URLs serve the same content via the redirect shells.

## Repo retention

Keeping this repo live (not archiving) so the redirect URLs continue to function until Apple + Play metadata is updated. Once both stores point to the new URLs, this repo can be archived as read-only.
