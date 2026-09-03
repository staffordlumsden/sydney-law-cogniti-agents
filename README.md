# Sydney Law School Cogniti Agent Hub

A static GitHub Pages site bringing together Sydney Law School Cogniti agents and practical resources for legal education.

## Site contents

- `index.html` — standalone responsive landing page
- supplied agent artwork is embedded directly into `index.html` for a genuinely standalone page
- `resources/` — supplied guides and web-readable curriculum-mapping resources
- `DESIGN.md` — design-system specification used for the page
- `.github/workflows/pages.yml` — optional GitHub Pages deployment workflow

## Publishing on GitHub Pages

This repository is configured as a static GitHub Pages site. The included workflow deploys the root of the `main` branch using GitHub Actions. If Pages has not yet been enabled for the repository, open **Settings → Pages** and set the source to **GitHub Actions**.

The static page itself requires no build step.

## Content note

The active general-purpose agent is labelled **ChatGPT 5.4 for Sydney Law School**. Some supplied guides were authored for an earlier ChatGPT4o configuration and are retained as legacy workflow resources; their historical model naming has not been silently rewritten.
