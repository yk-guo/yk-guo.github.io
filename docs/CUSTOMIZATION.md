# Customization

## Profile and avatar

Edit `content/authors/admin/_index.md` for name, role, organization, interests, education and the Markdown biography following the closing `---`. The current biography is temporary. Do not add education dates until confirmed.

Replace `content/authors/admin/avatar.png` with a square portrait. Keep only one `avatar.*` file. Hugo applies the original circular crop. Replace `assets/media/icon.png` separately for the site favicon (currently the YG placeholder; the profile uses the supplied cityscape).

## News

In `content/_index.md`, find the Markdown block titled `News📢`. Replace `text: ''` with a YAML multiline Markdown value, for example:

```yaml
      text: |-
        - [Month Year] Your confirmed announcement.
```

The empty block keeps its heading and original two-column styling.

## Publications

Create `content/publication/<slug>/index.md` with real paper metadata. Keep `content/publication/_index.md`. Required fields for the existing featured collection include:

```yaml
---
title: 'Confirmed paper title'
date: '2026-01-01' # replace with the actual date
publishDate: '2026-01-01' # replace with the actual date
authors: ['Yunkun GUO'] # replace with the actual author list
publication: 'Confirmed venue'
publication_types: ['2']
featured: true
url_pdf: ''
---
```

Do not copy this example as an actual publication. The existing `community/citation_pub` view remains active and renders newly added featured papers automatically. Zero papers produces no cards. Add contribution notes only when needed and confirmed.

## CV

Put the real PDF at `static/docs/Yunkun_GUO_CV.pdf` (create directories). Add a CV entry to `config/_default/menus.yaml` with `url: /docs/Yunkun_GUO_CV.pdf`, and optionally an `ai` / `cv` social entry in the author profile. Do not enable links before the file exists.

## Site configuration

Title and canonical URL: `config/_default/hugo.yaml`.
SEO, themes, avatar shape and footer: `config/_default/params.yaml`.
Navigation: `config/_default/menus.yaml`.
Keep `https://yk-guo.github.io/` as the root baseURL. Run the production build and inspect the site after every edit.
