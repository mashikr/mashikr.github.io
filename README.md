# Portfolio — Md Ashikur Rahman

Static personal portfolio site: full-stack software engineering profile, projects, academic background (education, publications, honors), downloadable CVs, and contact links.

**Live preview:** [mdashikur567.github.io](https://mdashikur567.github.io)

## Features

- Responsive layout with sidebar navigation and tab-style content sections
- Sections: About, Skills, Experience, Projects, Education, Publications, Honors & Awards, Resume downloads, Contact
- Dark mode toggle
- Mobile-friendly navigation (drawer menu with outside-click close)
- Sass-based styles (`@use` modules), compiled to `css/style.css`

## Tech stack

- HTML5, CSS (compiled from Sass/SCSS)
- [Dart Sass](https://sass-lang.com/) for styles
- [Font Awesome](https://fontawesome.com/) (bundled CSS in `css/`)
- Vanilla JavaScript for tabs, theme toggle, and mobile nav behavior

## Project structure

```
├── index.html          # Main page
├── sass/               # SCSS sources (main entry: main.scss)
├── css/                # Compiled stylesheet (style.css) + vendor CSS
├── img/                # Images and assets
├── doc/                # CV PDFs and thesis PDFs (optional local files)
├── package.json        # npm scripts + sass dev dependency
└── README.md
```

## Prerequisites

- [Node.js](https://nodejs.org/) (LTS recommended) — only needed to compile Sass

## Setup

```bash
git clone https://github.com/mdashikur567/grid-with-sass-website.git
cd grid-with-sass-website
npm ci
```

Use `npm install` if you do not have a lockfile.

## Styles (Sass)

- **One-off build (compressed output to `css/style.css`):**

  ```bash
  npm run compress:css
  ```

- **Watch mode** (recompiles when SCSS changes):

  ```bash
  npm run watch
  ```

Edit files under `sass/`; the site loads `css/style.css` from `index.html`.

## Deployment

This is a static site: deploy the repository root (or build output) to any static host (e.g. GitHub Pages, Netlify). Ensure `css/style.css` is up to date before publishing if you changed SCSS.

## License

ISC (see `package.json`).
