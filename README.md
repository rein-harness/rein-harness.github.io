# rein-harness.github.io

Hosts the Rein documentation at **https://rein-harness.github.io/**.

The site's source lives in the main repo, [DarKnight1346/rein-harness](https://github.com/DarKnight1346/rein-harness), under `site/`. Edit the docs there, not here.
This repo holds only the deploy workflow (`.github/workflows/pages.yml`). It builds `site/` from the main
repo's `main` branch:

- when the main repo's Docs workflow dispatches `docs-updated` (requires the `SITE_DISPATCH_TOKEN` secret there),
- daily at 06:17 UTC,
- or by hand: Actions → Deploy site → Run workflow (you can pick a branch to preview).
