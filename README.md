# Xiaowei Qian — Academic Homepage

Personal academic website: [xweiq.github.io](https://xweiq.github.io/).

Built with Jekyll and published through GitHub Pages. The current layout is adapted from [Arvid's Academic Homepage Template](https://github.com/Arvid-pku/Academic-Homepage-Template), with custom typography, publication lists, and a burgundy / ink-blue palette.

[中文说明](docs/README-zh.md)

## Content and structure

- `_pages/about.md`: profile, biography, selected publications, education, and service.
- `_data/publications.yml`: all papers, authors, venues, years, links, and distinctions. Set `selected: true` to include a paper on the homepage.
- `_includes/arvid-paper.html`: shared publication entry, ordered as title, authors, then venue/year, distinction, and links.
- `_pages/publications.html`: full publication list, grouped into Preprints and Conference.
- `_pages/projects.html`, `_pages/cv.html`: intentionally empty apart from headings. Blogs and Photography retain navigation entries and placeholders.
- `_config.yml`: identity, email, social links, and site metadata.

## Appearance

`assets/css/arvid/typography.css` contains the shared settings:

- `--nav-color` / `--nav-active-color`: navigation, name, page and section headings, full-list link, and distinctions.
- `--primary-color` / `--secondary-color`: publication titles and other content links.
- `--font-heading`, `--font-body`, `--font-ui`: Palatino headings/body and Gill Sans interface text.
- `--title-size`, `--section-size`, `--body-size`: type scale.

`assets/css/arvid/shared-styles.css` controls the common page width and gutters; `homepage.css` controls profile and education layout.

Dark mode is temporarily disabled: the toggle is commented out in `assets/js/arvid/site-shell.js`, and `initializeDarkMode()` is commented out in both `_layouts/home.html` and `_layouts/arvid-page.html`. Restore both to re-enable it; the saved dark palette should be reviewed alongside any new light palette.

## Local preview

With Ruby, Bundler, and Jekyll dependencies installed:

```sh
bundle install
bundle exec jekyll serve --host 127.0.0.1 --port 4000
```

For the existing local environment with Jekyll already installed:

```sh
JEKYLL_NO_BUNDLER_REQUIRE=true jekyll serve \
  --destination /Users/silver/.cache/blog-preview/manual-site \
  --host 127.0.0.1 --port 4001
```

Open the corresponding localhost port. The watch server rebuilds after edits; refresh the browser to see changes.

## Publishing

Commit and push to `main`; check the repository's **pages build and deployment** run in GitHub Actions. CSS and JavaScript URLs contain a build timestamp so a new deployment requests fresh assets. If an already-open page still looks old, reload it (macOS: Command–Shift–R).

## Sources and licenses

See [upstream and adaptation notes](assets/css/arvid/UPSTREAM.md). The current design is based on Arvid, while some Jekyll infrastructure was retained from the earlier AcadHomepage-based site. Historical copyright notices remain in [LICENSE](LICENSE). Bundled ET Book files retain their own [license](assets/fonts/et-book/LICENSE); they are available for experiments and are not the current default font.
