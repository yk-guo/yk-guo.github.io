# Validation — 2026-10-23

- Original source baseline: Hugo Extended 0.124.1 build passed from a temporary pristine checkout (68 pages).
- Customized production: `GOMODCACHE="$PWD/.tools/gomod" .tools/hugo --minify --destination /tmp/academic-production` passed (17 pages).
- Development: Hugo server running at http://localhost:1313/.
- Browser: reference and local screenshots compared at 1440×1000; mobile full-page screenshot at 390×844. Original theme spacing, circular avatar and responsive columns retained. Shorter biography naturally reduces section height.
- Mobile document width: 390px; viewport: 390px. No broken images. No invalid homepage internal links. Email and GitHub targets verified.
- News and Publications headings present; zero publication cards.
- Mobile navigation expands; display preference menu exposes light/dark/automatic options.
- Current content, configuration, templates and built HTML scanned for former author's identifying text; none found. Provenance documentation and Git history intentionally retain source attribution.
- MIT license and framework credit retained. go.mod versions unchanged; go.sum included for reproducibility.
- GitHub Pages workflow reviewed and restricted to yk-guo/yk-guo.github.io. Remote Actions execution/deployment NOT verified: publication has not been authorized.
- Screenshots: output/playwright/desktop.png, mobile.png, reference-desktop.png (local verification artifacts, ignored by Git).
