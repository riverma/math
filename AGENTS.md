# Agent guide — Mental Math

A dependency-free, offline-first static PWA served at `math.riverma.com` via GitHub Pages (deploy from the default branch, root). Files live at the repo root; the app is served at the subdomain root, so keep all asset paths relative.

## Release discipline — do this on EVERY commit

1. **Pick the SemVer bump** for the change (see https://semver.org):
   - `patch` — bug fix / copy tweak / no behavior change.
   - `minor` — new backward-compatible feature.
   - `major` — breaking change to behavior or saved-data format.
2. **Update `CHANGELOG.md`** — move items out of `[Unreleased]` into a new `vX.Y.Z` section (Keep a Changelog format), dated today.
3. **Update the version string in three places so they always match:**
   - the footer label in `index.html` (`<span class="app-version">vX.Y.Z</span>`),
   - `const VERSION` in `sw.js` (this busts the offline cache so users get the update),
   - the `[X.Y.Z]` compare/link footer in `CHANGELOG.md`.
4. **Cut a GitHub release on every major or minor bump** (patch releases optional):

   ```sh
   git commit -am "…"; git push
   gh release create vX.Y.Z --title "vX.Y.Z" --notes-from-tag   # or --generate-notes
   ```

## Guardrails
- **Offline-first:** no CDNs, no third-party requests, no analytics. Self-host every asset.
- **Security:** run a security review of the diff before pushing; never commit secrets.
- If you add/remove any asset, update the `ASSETS` precache list in `sw.js`.
