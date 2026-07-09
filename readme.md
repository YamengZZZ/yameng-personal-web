# Yameng Zhang Personal Website

This repository contains the source code for my personal academic website built with [Quarto](https://quarto.org/).

The website includes:

- Home page
- Publications
- News
- Academic services
- Teaching

## Tech Stack

- [Quarto](https://quarto.org/)
- SCSS for custom styling
- GitHub Pages for deployment

## Project Structure

```text
.
├── _quarto.yml
├── index.qmd
├── publications.qmd
├── news.qmd
├── styles.scss
├── images/
└── docs/
```

- `_quarto.yml`: site configuration
- `index.qmd`: homepage
- `publications.qmd`: full publication list
- `news.qmd`: news page
- `styles.scss`: custom website styles
- `docs/`: rendered site output for deployment

## Local Preview

Make sure Quarto is installed first.

Preview the website locally:

```bash
quarto preview index.qmd --no-browser --no-watch-inputs
```

Or render the full site:

```bash
quarto render
```

After rendering, the generated static files will be placed in `docs/`.

## Deployment

This website is intended to be deployed with GitHub Pages using the `docs/` folder.

Recommended steps:

1. Render the site locally with `quarto render`.
2. Commit both the source files and the generated `docs/` folder.
3. Push the repository to GitHub.
4. In the GitHub repository, go to `Settings` -> `Pages`.
5. Set the source to `Deploy from a branch`.
6. Choose your main branch and the `/docs` folder.

Once GitHub Pages finishes deployment, the site will be publicly available at your GitHub Pages URL.

## Notes

- Update `site-url` and `repo-url` in `_quarto.yml` to match your GitHub account and repository.
- If `docs/` is ignored in `.gitignore`, remove that rule before deployment.
- Video embeds and publication links can be updated directly in `index.qmd`.

## License

This project is for personal website use. Please adapt the content responsibly if you reuse the structure or styling.
