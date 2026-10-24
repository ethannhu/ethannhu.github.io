# Zihang Hu — Personal Academic Homepage

A responsive academic homepage built with [Eleventy](https://www.11ty.dev/) and Nunjucks templates. The published site is static HTML and CSS; there is no browser-side JavaScript or external runtime service.

## Develop locally

Requires Node.js 22 or newer.

```sh
npm ci
npm start
```

Eleventy serves the generated site locally. To create a production build:

```sh
npm run build
```

The output is written to `_site/`.

## Publish to GitHub Pages

`.github/workflows/pages.yml` builds and deploys `_site/` on pushes to `main` or `master`, and can also be started manually from the repository's **Actions** tab. The workflow runs in the `node:22-slim` Docker image.

For the first deployment, open **Settings → Pages** and select **GitHub Actions** as the deployment source.

## Content and templates

Page content lives in `src/`. Shared page chrome is maintained in `src/_includes/layouts/base.njk` and `src/_includes/components/`; global site identity and navigation are in `src/_data/site.json`. Styles are in `src/assets/css/style.css`.

The project, research, and notes listings link to the corresponding public GitHub repositories and CSDN articles. Contact details and publication records still need to be supplied. The affiliation is listed as Smart Software Engineering Lab (ECNU). Replace the remaining marked prompts with verified public information and update `site.updated` when the site content changes.
