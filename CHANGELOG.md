# Changelog

## 0.4.6 — 2026-10-12

- Package: include `migrate.ts`, which 0.4.4 imported but did not ship, so the extension failed to load with "Cannot find module './migrate.ts'".
- Themes: write only the HTML export colors Pi's theme schema accepts (`pageBg`, `cardBg`, `infoBg`).

## 0.4.5 — 2026-10-12

- Themes: write only the HTML export colors Pi's theme schema accepts (`pageBg`, `cardBg`, `infoBg`). The extra keys made Pi 1.1.0 reject every generated theme as invalid.

## 0.4.4 — 2026-10-12

- Palette data (library, backups, login, favorites, theme sync) lives in `${PRJCT_HOME:-~/.prjct}/pi-palette`. On the first session the files in Pi's folder are copied there, checked by SHA-256, and only then removed; a differing destination is never overwritten.
- Code: no `let` bindings. Tests run with temporary Pi and prjct folders. The bundled-palette count test (34 vs 35) already failed before this release.

## 0.4.3 — 2026-10-06

- Publish from an independent repository with its own checks, lockfile and declared npm dependencies. Preserve the extension history and install name.
