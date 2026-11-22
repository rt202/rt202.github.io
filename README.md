# rt202.github.io

A project hub for [github.com/rt202](https://github.com/rt202), served by GitHub Pages at **https://rt202.github.io**. The full portfolio lives at [ronak.mlprep.org](https://ronak.mlprep.org).

The site is static HTML styled with Tailwind CSS v4, using the `tw:` prefix. The design is based on the [Jamie portfolio template](https://github.com/PaulleDemon/awesome-landing-pages/tree/main/src/portfolio/Jamie-portfolio) by PaulleDemon (MIT, see `LICENSE-template.txt`).

## Editing

- Content lives in `index.html`. Each project is one `<article>` card in the `#projects` section.
- Custom styles are in `css/index.css`. Tailwind's entry point is `css/tailwind.css`.

## Rebuilding CSS

`css/tailwind-build.css` is committed, so GitHub Pages serves it without a build step. Rebuild it after adding new Tailwind classes:

```bash
npm install
npm run build:css
```

## Local preview

```bash
python3 -m http.server 4173
```

## Deploying

Push to `main`. In repo Settings → Pages, the source is **Deploy from a branch → `main` / root**. `.nojekyll` turns off Jekyll processing.
