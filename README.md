# cmorasar.github.io

Source for my personal website: **https://cmorasar.github.io**

Built with [Jekyll](https://jekyllrb.com) and hosted on GitHub Pages. The theme
started as [Academic Pages](https://github.com/academicpages/academicpages.github.io),
a fork of [Minimal Mistakes](https://mmistakes.github.io/minimal-mistakes/)
(© Michael Rose, MIT — see `LICENSE`), and has since been trimmed down and
customized.

## Where things live

| What | File |
| --- | --- |
| Site-wide config, sidebar profile, social links | `_config.yml` |
| Top navigation bar | `_data/navigation.yml` |
| Home / about page and "Recent news" | `_pages/about.md` |
| Publications & talks list | `_pages/publications.md` |
| 404 page | `_pages/404.md` |
| Resume PDF and other downloads | `files/` |
| Images (profile photo, favicon) | `images/` |
| Page templates | `_layouts/`, `_includes/` |
| Styles | `_sass/`, `assets/css/` |

Anything dropped in `files/` is served at `https://cmorasar.github.io/files/<name>`.

## Publishing

GitHub Pages builds and deploys automatically on every push to `master`.
There is no separate build step to run — a push is a deploy, and it goes live
in roughly a minute.

## Running locally

Preview changes before pushing:

```bash
bundle install                # first time only
bundle exec jekyll serve --config _config.yml,_config.dev.yml --livereload
```

Then open http://localhost:4000. The server rebuilds on save, except for
`_config.yml` — changing that requires restarting the server.

Requires Ruby with development headers and Bundler. If `bundle install` fails,
delete `Gemfile.lock` and try again.

## Rebuilding the JavaScript bundle

Only needed if you edit `assets/js/_main.js` or anything in `assets/js/plugins/`:

```bash
npm install
npm run build:js              # regenerates assets/js/main.min.js
```
