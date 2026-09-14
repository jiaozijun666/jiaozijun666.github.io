# jiaozijun666.github.io

Personal academic website for Zijun Jiao, built on the
[al-folio](https://github.com/alshedivat/al-folio) Jekyll theme.

## Where the content lives

| What you want to change | File |
| --- | --- |
| Front-page bio, subtitle, education block | `_pages/about.md` |
| News items on the front page | `_news/` — one file per item, `YYYY-MM-DD-slug.md`. See `_news/_TEMPLATE.md.example` |
| Research / project entries | `_projects/` — one file per project; `importance` sets the order inside a category, `category` picks the section |
| CV contents | `_data/cv.yml` |
| Email, GitHub, LinkedIn, CV PDF link | `_data/socials.yml` |
| Name, site title, description, favicon | `_config.yml` (top of file) |
| Images | `assets/img/` |
| CV PDF for download | put it in `assets/pdf/` and uncomment `cv_pdf` in `_data/socials.yml` and `_pages/cv.md` |

## Publishing

Pushing to `master` runs `.github/workflows/deploy.yml`, which builds the site and
pushes the result to the `gh-pages` branch. **GitHub Pages must be set to serve from
`gh-pages` / root** (Settings → Pages → Build and deployment → Deploy from a branch).
This is a one-time setting; the previous site served straight from `master`, which
will not work for this theme.

## Previewing locally

With Docker:

```bash
docker compose up
# → http://localhost:8080/
```

Or with Ruby installed:

```bash
bundle install
bundle exec jekyll serve
# → http://localhost:4000/
```
