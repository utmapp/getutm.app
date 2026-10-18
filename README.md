# UTM Homepage

Official site for [UTM](https://getutm.app), covering UTM for macOS, UTM SE and UTM Remote for iOS.

Built with Jekyll 4. The landing page is `index.html`; `licenses.md` and `privacy.md` are Markdown pages using the `page` layout; the remaining `.md` files at the root are redirects handled by `jekyll-redirect-from`.

## Develop

```sh
bundle install
bundle exec jekyll serve --livereload
```

## Deploy

`.github/workflows/pages.yml` builds the site with GitHub Actions and publishes it to GitHub Pages on every push to `main`. In the repository settings, set Pages → Source to **GitHub Actions**.

## Layout

- `_layouts/default.html` – document shell, header and footer
- `_layouts/page.html` – prose layout for Markdown pages
- `assets/css/main.css` – the theme
- `assets/img/`, `assets/video/` – landing page media
