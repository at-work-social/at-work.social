# Work Atmosphere (at-work.social)

Professional social network where people control their data and experience.

This repository contains the boilerplate landing site — static HTML & CSS with
light/dark theme support — deployable to [Cloudflare Workers](https://developers.cloudflare.com/workers/static-assets/).

## Structure

```
public/          Static assets served as the site
  index.html     Landing page
  styles.css     Theme + layout (light/dark via CSS variables)
  theme.js       Theme toggle + persistence (localStorage)
  favicon.svg
wrangler.jsonc   Cloudflare Workers config (static assets)
```

## Develop

```sh
npm install
npm run dev      # local preview at http://localhost:8787
```

## Deploy

```sh
npm run deploy   # requires a Cloudflare account (wrangler login)
```

## Theme

The site defaults to the visitor's OS preference (`prefers-color-scheme`) and
lets them override it with the toggle in the header; the choice is remembered in
`localStorage`.

## Links

- GitHub: https://github.com/at-work-social/at-work.social
- Bluesky: https://bsky.app/profile/at-work.social
