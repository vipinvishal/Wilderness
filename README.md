# WILDERNESS — Forest Landing Page

A cinematic single-page forest brand site. Designed & published by [Orbit AI Labs](https://orbitailabs.in/).

## How to view it
Just open `index.html` in any browser. That's it — no build step, no install.

## Techniques used
- **CSS `mix-blend-mode`** — the "WILDERNESS" / "BREATHE IN" headlines fuse with the video
- **GSAP ScrollTrigger** — hero pins while content scrolls over it
- **Splitting.js** — title arrives letter by letter on load
- **`<video autoplay muted loop playsinline>`** — living forest background
- **CSS `clamp()`** — fluid typography, zero media queries
- **`linear-gradient` overlay** — text stays readable at any brightness
- Animated CSS forest fallback so the hero is never blank while the video loads

## Swapping the background video
The hero uses a Coverr CDN clip. If it doesn't load (some CDNs block hotlinking),
the animated CSS forest stays visible — by design.

To use your own footage:
1. Download a forest .mp4 from pexels.com/videos or coverr.co
2. Drop it in this folder (e.g. `forest.mp4`)
3. In `index.html`, find the hero `<video>` near `id="heroVideo"` and change:
   `data-src="https://cdn.coverr.co/..."` → `data-src="forest.mp4"`
   (Do the same for `id="bandVideo"` if you want.)

## Deploy
- **Vercel / Netlify:** drag this folder onto the dashboard. Done.
- Or any static host — it's a single HTML file with CDN-loaded fonts and scripts.

All external resources (fonts, GSAP, Splitting.js) load from CDNs, so an internet
connection is needed the first time it loads.
# Wilderness
