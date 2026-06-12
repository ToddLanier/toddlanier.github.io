# tllester.info

All things Todd Lanier Lester. Hugo static site, deployed on GitHub Pages.

## Local Development

```bash
hugo server -D
```

Open <http://localhost:1313>.

## Build

```bash
hugo --gc --minify
```

Output in `public/`.

## Deploy

Push to `main` → GitHub Actions builds and deploys to GitHub Pages at [tllester.info](https://tllester.info).

Any other branch → deploys a preview to `https://tllester.info/preview/<branch>/`.
