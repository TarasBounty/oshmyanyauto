# Автохаус «Ошмяны Авто» — website

One-page static website for Автохаус «Ошмяны Авто» (г. Ошмяны, ул. Пионерская, 60А).

## Structure

```
index.html            — the page
assets/css/style.css  — styles
assets/js/main.js     — mobile menu, footer year
assets/img/car.svg    — logo car silhouette
favicon.svg           — site icon
CLAUDE.md             — rules for Claude when making changes
```

No build step: open `index.html` in a browser to preview.

## Workflow

1. Requirements are described to Claude.
2. Claude opens a pull request with the changes.
3. The PR is reviewed and merged on GitHub.
4. `main` is deployed automatically (GitHub Pages for preview, Hostinger for production).
