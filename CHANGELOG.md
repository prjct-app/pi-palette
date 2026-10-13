# Changelog

## 0.4.4 — 2026-10-12

- Palette data (library, backups, login, favorites, theme sync) lives in `${PRJCT_HOME:-~/.prjct}/pi-palette`. On the first session the files in Pi's folder are copied there, checked by SHA-256, and only then removed; a differing destination is never overwritten.
- Code: no `let` bindings. Tests run with temporary Pi and prjct folders. The bundled-palette count test (34 vs 35) already failed before this release.

## 0.4.3 — 2026-10-06

- Publish from an independent repository with its own checks, lockfile and declared npm dependencies. Preserve the extension history and install name.
