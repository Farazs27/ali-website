# Samen Mondzorg — Dental clinic site

Multi-page static website for **Samen Mondzorg**, a dental clinic in Amsterdam-Noord.
Sage-green / cream brand palette, Fraunces serif + Inter sans, fully responsive.

## Pages
- `index.html` — Home
- `over-ons.html` — Over ons (about)
- `behandelingen.html` — Behandelingen (treatments)
- `contact.html` — Route & contact
- `afspraak.html` — Afspraak maken (booking)

Shared design system: `styles.css`. No build step — vanilla HTML/CSS.

## Local dev

```bash
python3 -m http.server 8765
# open http://localhost:8765/
```

## Brand imagery

The hero, treatment-room and waiting-corner photos in `images/` were generated with
[KIE](https://kie.ai/) `gpt-image-2-text-to-image`. To regenerate:

1. Copy `.env.example` to `.env` and set `kie_api_key=...`
2. `zsh generate_images.sh`

Prompts and aspect ratios live in `generate_images.sh`.

## Deploy

This is a static site — drop the folder into any static host. Configured for Vercel
via `vercel.json`.
