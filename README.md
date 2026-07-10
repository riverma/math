<!-- markdownlint-disable MD033 MD041 -->
<div align="center">

# Mental Math

**Race through arithmetic puzzles — beat the clock and chase your best score.**

[Play it live](https://math.riverma.com) · [Report a bug](https://github.com/riverma/math/issues/new?template=bug_report.md) · [Request a feature](https://github.com/riverma/math/issues/new?template=feature_request.md)

[![License: AGPL v3](https://img.shields.io/badge/License-AGPL_v3-blue.svg)](./LICENSE)
[![PWA](https://img.shields.io/badge/PWA-installable%20%C2%B7%20offline-5a5.svg)](https://math.riverma.com)

</div>

## Privacy

**No data collected · no tracking · runs entirely on your device — 100% private.** There is no backend, no analytics, and no third-party requests. Your scores and preferences live only in your browser's local storage.

## Features

- Practice times, plus, minus, divide, or a mix — at easy / medium / hard levels.
- Exact or "good enough" scoring, and runs of 5 / 10 / 20 / 50 problems.
- Streaks, a scoreboard with per-problem review, and a fast keyboard-first flow.
- **Installable PWA** — add it to your home screen and play fully offline.
- English / Spanish interface.

## Quick start

It's a static site — no build step.

```sh
git clone https://github.com/riverma/math.git
cd math
python3 -m http.server 8000   # then open http://localhost:8000
```

Serve over HTTP (not `file://`) so the service worker and manifest load.

## Contributing

Issues and pull requests are welcome — see the templates under [`.github/`](./.github). Please describe the change and keep the app dependency-free and offline-first.

## Versioning & changelog

This project uses [Semantic Versioning](https://semver.org). See [CHANGELOG.md](./CHANGELOG.md) for release history.

## License

Licensed under the [GNU Affero General Public License v3.0](./LICENSE) © Rishi Verma. Bundled third-party assets (e.g. the Nunito font) retain their own licenses.
