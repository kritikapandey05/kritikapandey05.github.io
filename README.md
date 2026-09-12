# kritikapandey05.github.io

A small custom Jekyll site — no theme gem, just a layout + one stylesheet, so it builds on GitHub Pages with zero setup.

## Files

- `_config.yml` — site title/description
- `_layouts/default.html` — shared header, nav, footer for every page
- `assets/css/style.css` — all styling
- `index.md` — About Me (site root, `/`)
- `research.md` — Research (`/research/`)
- `blog.md` — Blogs (`/blog/`)

## Before you push

1. **CV link** — `index.md` currently points to `/assets/Kritika_Pandey_CV.pdf`, which doesn't exist yet. Drop your resume PDF into `assets/` under that name, or edit the link in `index.md` to wherever you're hosting it.
2. **LinkedIn URL** — double-check the LinkedIn link in `index.md` is your current profile URL.
3. Skim `research.md` for the exact dates/venues on IndicClaimVer and PM-JAY — I filled these in from what you'd written, but you know the details best.

## Deploying

1. In your `kritikapandey05.github.io` repo, delete the old `index.md` and `_config.yml`, and remove any leftover `Gemfile`/minima references if present.
2. Copy every file from this folder into the repo root, preserving the folder structure (`_layouts/`, `assets/css/`).
3. Commit and push to `main`. GitHub Pages rebuilds automatically — check the **Actions** tab or **Settings → Pages** for build status.
4. Visit `https://kritikapandey05.github.io/` once the build finishes (usually under a minute).

## Editing later

- To tweak colors, edit the `:root` variables at the top of `assets/css/style.css`.
- To add a new research entry, copy one `<div class="entry">...</div>` block in `research.md` and edit it.
- To publish your first post, replace the empty state in `blog.md` with your post content (or split posts into their own files later if the list grows).
