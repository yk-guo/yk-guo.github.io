# Project instructions

- Use Hugo Extended 0.124.1 and Hugo Blox Bootstrap v5.9.7; preserve module versions.
- Match the reference academic layout. Prefer configuration changes; no React migration, redesign, backend, or unnecessary CSS.
- Build: `GOMODCACHE="$PWD/.tools/gomod" .tools/hugo --minify`.
- Preview: `GOMODCACHE="$PWD/.tools/gomod" .tools/hugo server --bind 127.0.0.1`.
- Never invent publications, dates, supervisors, honors, news or CV content.
- Keep empty News and Publications headings. Add only confirmed content.
- Preserve MIT licenses, copyright notices and framework attribution.
- Keep public/, resources/, .tools/ and output/ out of commits.
- Do not create a remote repository or push without explicit user authorization.
- Verify desktop (1440px) and mobile (390px), image loading, internal links, SEO, and absence of previous personal data after changes.
