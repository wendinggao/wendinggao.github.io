# Wending Gao

Personal academic homepage built with [al-folio](https://github.com/alshedivat/al-folio) v1.

## Current stage

The site currently contains an English home page, a portrait, news, selected publications, and an email contact link supplied by Wending Gao. CV, LinkedIn, and Google Scholar icons are displayed without destinations until their details are provided. Projects and a CV can be added in later stages.

## Edit the site

- Personal information and site settings: `_config.yml`
- Home page: `_pages/about.md`
- Academic and contact links: `_data/socials.yml`
- Publications: `_bibliography/papers.bib`
- Images: `assets/img/`
- CV PDF: `assets/pdf/`

When adding a new section, create its page under `_pages/` and set `nav: true` in its front matter to show it in the navigation.

## Preview locally

The upstream starter requires Ruby 3.3, Bundler, and Node.js 20. With these installed:

```sh
bundle install
npm ci
bundle exec jekyll serve --livereload
```

Open <http://localhost:4000/>. See the upstream [installation guide](https://github.com/alshedivat/al-folio/blob/main/docs/INSTALL.md) for alternatives.

## Publish with GitHub Pages

The site is configured for <https://wendinggao.github.io/> with an empty `baseurl`. The workflow in `.github/workflows/deploy.yml` builds the site and publishes a GitHub Pages artifact whenever `main` is updated. Set the repository's Pages source to **GitHub Actions**.

The upstream al-folio project is licensed under MIT; see `LICENSE`.
