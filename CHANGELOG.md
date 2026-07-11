# Changelog

All notable changes to this project are documented here.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [1.0.2] - 2026-07-10

### Added
- Install helper: opening the app with `#install` (from apps.riverma.com) shows an install prompt or Add-to-Home-Screen guidance, so the launcher's Install button installs this app correctly.

## [1.0.1] - 2026-07-10

### Changed
- Footer privacy line now uses a period instead of an em dash, for consistency across the apps.

## [1.0.0] - 2026-07-10

### Added
- First independent release of Mental Math, extracted from `riverma.github.io` into its own repository and published at [math.riverma.com](https://math.riverma.com).
- Installable **Progressive Web App**: web manifest, app icons, and a cache-first service worker so the app is installable and runs fully offline.
- Self-hosted **Nunito** font (latin subset) — removed the Google Fonts CDN dependency; the app now makes zero third-party network requests.
- In-app footer with a privacy statement, version, and source/license link.
- AGPL-3.0 license.

### Changed
- "Back to home" link now points to `https://riverma.com/`.

[Unreleased]: https://github.com/riverma/math/compare/v1.0.2...HEAD
[1.0.2]: https://github.com/riverma/math/compare/v1.0.1...v1.0.2
[1.0.1]: https://github.com/riverma/math/compare/v1.0.0...v1.0.1
[1.0.0]: https://github.com/riverma/math/releases/tag/v1.0.0
