# Yunkun GUO — Academic Homepage

English academic homepage based on the original Academic CV site, retaining Hugo Blox Bootstrap **v5.9.7** and **Hugo Extended 0.124.1**. Go is required for module downloads. No backend or Node build is required.

## Local preview

The downloaded macOS binary is at `.tools/hugo` (ignored by Git). On other machines install Hugo Extended 0.124.1 and substitute `hugo` below.

```sh
GOMODCACHE="$PWD/.tools/gomod" .tools/hugo server --bind 127.0.0.1
# http://localhost:1313/
GOMODCACHE="$PWD/.tools/gomod" .tools/hugo --minify
```

Production output is `public/`, excluded from Git. Internet access is needed on the first build to fetch pinned modules. Do not upgrade the theme to resolve unrelated build issues.

See [customization](docs/CUSTOMIZATION.md) for avatar, biography, news, papers, and CV. The current biography is provisional; no research history or publication claims have been added.

## GitHub Pages

Publication was authorized on 2026-10-27. Target: https://yk-guo.github.io/ . The following steps document setup for a fresh checkout:

1. Create an empty `yk-guo/yk-guo.github.io` repository on GitHub.
2. Set Settings → Pages → Source to **GitHub Actions**.
3. Review `git status` and ensure personal files and generated output are excluded.
4. Run:

```sh
git branch -M main
git remote add origin https://github.com/yk-guo/yk-guo.github.io.git
git add .
git commit -m "Customize academic homepage for Yunkun GUO"
git push -u origin main
```

The workflow uses Hugo Extended 0.124.1, builds the root site URL and deploys the artifact. Deployment status is available in the repository Actions tab. Never push to the reference repository.

## Attribution

Adapted from https://github.com/jiarui-liu/jiarui-liu.github.io using Hugo Blox Academic CV. Original MIT license is retained in `LICENSE.md`; template license comments and framework footer credits remain. Upstream Git history is retained for provenance; removed personal files are absent from the current source and output, but remain in that historical history.
