# Espresso Fellows — Website

Static marketing site built with plain HTML/CSS/JS and bundled with [Vite](https://vitejs.dev).

## Run locally

```bash
npm install
npm run dev      # http://localhost:5173
```

## Build for production

```bash
npm run build    # outputs to dist/
npm run preview  # serve the built site locally
```

## Deploy

- **Vercel / Netlify / Cloudflare Pages:** import the repo — build command `npm run build`, output directory `dist`. (`netlify.toml` and `vercel.json` are included.)
- **Any static host:** upload the contents of `dist/`.
- **GitHub Pages under a sub-path** (e.g. `/repo-name/`): set `base: '/repo-name/'` in `vite.config.js` and change the `/images/` paths to relative.

## Structure

```
index.html          Complete page: markup, styles, content data and rendering script
public/images/      Photos, logo, favicon (served at /images/...)
package.json        Vite build scripts
vite.config.js      Vite config (output: dist/)
vercel.json         Vercel build settings
netlify.toml        Netlify build settings
```

## Editing content

All content lives in `index.html`. Branches and products are the `products` / `locations` arrays in the script at the bottom; hero image (`'Latte photo'` or `'Billboard'`) and location photo shape (`'Circle'` or `'Rounded'`) are in `config` in that same script.

## Vercel settings

Framework: Vite · Build command: `npm run build` · Output directory: `dist` · Root directory: the folder containing `package.json`.
