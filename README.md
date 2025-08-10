# KidBeat – Netlify-Ready (Vite + React)

A friendly, privacy-first beatmaker that runs entirely in the browser. Robust Web Audio scheduler (continuous playback), swing, per-track volume, save/load, and WAV export.

## Local Dev
```bash
npm install
npm run dev
```

## Build
```bash
npm run build
```
Outputs to `dist/`.

## Deploy to Netlify
1. Push this folder to GitHub.
2. In Netlify, **Add new site → Import from Git** and select your repo.
3. **Build command:** `npm run build`
4. **Publish directory:** `dist`
5. Deploy.

This repo includes both `netlify.toml` and `public/_redirects` so SPA routes resolve to `index.html`.

## Notes
- First tap unlocks audio on iOS (browser policy).
- Patterns save locally in `localStorage` under `kidbeat_patterns`.
- WAV export uses `OfflineAudioContext` to render clean audio on-device.
