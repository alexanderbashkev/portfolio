# Oleksandr Bashkev — Portfolio

Personal site for **Oleksandr Bashkev** — AI Automation & Web Infrastructure Engineer.
Single page, no build step: static HTML / CSS / vanilla JS.

## Features
- System-aware light / dark theme with manual toggle
- Config-driven Google Tag Manager + GA4 (set your container id once)
- Fully responsive (desktop / tablet / mobile)

## Configure analytics
Open `index.html` and set your GTM container id in one place:
```js
window.SITE_CONFIG = { GTM_ID: "GTM-XXXXXXX" };
```
GA4 is wired *inside* GTM (Google Tag → GA4 with your `G-…` id), not hard-coded per page.

## Deploy (Vercel)
Static site — deploys as-is. Framework preset: **Other**, no build command, output = root.

## Run locally
Open `index.html` directly, or:
```bash
npx serve .
```
