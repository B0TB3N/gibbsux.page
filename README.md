# INIT0 — Minecraft Server Site

Astro site for a self-hosted Fabric Minecraft server.
Pages: Home, How to Join, Mods, Rules, Gallery, FAQ. Live server status via mcsrvstat.us.

## Editing

All server details live in one place: `src/consts.ts`
(address, Discord link, version, max players). Change them there and every page updates.

- Pages: `src/pages/*.astro`
- Shared layout / nav / footer: `src/layouts/`, `src/components/`
- Styling: `src/styles/global.css`

## Local development

```
npm install
npm run dev      # http://localhost:4321
npm run build    # outputs to dist/
```

## Deploying to Cloudflare

Connect this repo in Cloudflare Pages with:

- Framework preset: **Astro**
- Build command: `npm run build`
- Build output directory: `dist`

Every push to `main` redeploys automatically.

## Screenshots

Drop images into `public/shots/` and replace the placeholder blocks in
`src/pages/gallery.astro` with `<img src="/shots/yourfile.png" alt="" />`.
