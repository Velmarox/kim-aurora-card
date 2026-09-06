# Kim Allen — Aurora digital business card

Single-page card (`index.html`) for Kim Allen, Casino Attendant at Aurora Casino.
Deployed to Firebase Hosting. Live at v1.0.0 — PREVIEW badge is off.

**Live at:** kim-aurora.web.app
**Firebase project:** kim-aurora
**Current version:** see `CHANGELOG.txt` and `<meta name="version">` in `index.html`
**Built from:** Aurora Employee Card template tpl-v1.0.0

## Layout

- `index.html` — the whole card. Front, back sheet, promos, vCard, artwork.
- `assets/` — source images the inline artwork came from. Not deployed.
- `firebase.json` — hosting config; `index.html` is served no-cache.
- `CHANGELOG.txt` — release log, newest on top.
- `_version_archive/` — frozen copies of outgoing versions. Never edit these.

## Differences from the template

- No Email tab. The contact row is Call / Text only and the vCard carries no
  EMAIL line. If a later employee wants email back, take it from the template
  rather than un-deleting it here.

## Editing

Everything person-specific is in the **EDIT ME** block at the top of the
`<script>` in `index.html`. Below the **STOP EDITING** line is Aurora's shared
data — if that needs to change, change the template in
`Studio\00 Templates\Aurora Employee Card` first, then re-copy.

## Saving a change

1. Copy the current `index.html` into
   `_version_archive/card_v<current version>/` (skip if it's already there).
2. Make the edit.
3. Bump `<meta name="version">` and add a CHANGELOG entry.
4. Commit and push, or run `firebase deploy`.
