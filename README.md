# guanning03.github.io

Personal academic homepage of Guanning Zeng, built with Jekyll and the
[Minimal Light](https://github.com/yaoyao-liu/minimal-light) theme and served by GitHub Pages.

## Editing

- `_config.yml` — name, position, email, avatar and social links (Google Scholar / CV are commented out).
- `index.md` — About Me, Research Interests, News, Research Experience, Education, Honors.
- `_data/publications.yml` — publication list. Optional fields: `code`, `page`, `bibtex`, `notes`,
  and `image` (a teaser picture; without it the venue badge is shown on the left).
- `assets/img/` — avatar and favicons.

Pushing to `main` redeploys the site automatically.

## Local preview

```sh
bundle install
bundle exec jekyll serve
```
