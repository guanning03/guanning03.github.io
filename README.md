# guanning03.github.io

Personal academic homepage of Guanning Zeng, built with Jekyll and the
[Minimal Light](https://github.com/yaoyao-liu/minimal-light) theme and served by GitHub Pages.

## Editing

- `_config.yml` — name, position, email, avatar and social links.
- `index.md` — About Me, Research Interests, News, Research Experience, Honors.
- `_data/publications.yml` — publication list. Every entry gets a "Paper" button (`pdf`) and a
  "Project Page" button (`page`, falling back to `code`, then `pdf`). Optional: `notes`, and
  `image` (a 2:1 teaser in `assets/img/papers/`; without it only the venue badge is shown).
- `assets/img/` — avatar, favicons and paper teasers.

Pushing to `main` redeploys the site automatically.

## Local preview

```sh
bundle install
bundle exec jekyll serve
```
