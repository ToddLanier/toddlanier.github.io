# tllester.info

Personal portfolio for Todd Lanier Lester. Hugo static site, deployed on Netlify.

## Local Development

Requires Hugo `0.154.5` (matches `netlify.toml`).

```bash
hugo server -D
```

Open <http://localhost:1313>.

## Build

```bash
hugo --gc --minify
```

Output in `public/`.

## Pagefind Search Index

```bash
npm_config_yes=true npx pagefind --site "public" --output-subdir ../static/pagefind
```

## Deploy

Push to `main`. Netlify builds via `hugo --gc --minify --baseURL "${baseURL}"` (see `netlify.toml`).
