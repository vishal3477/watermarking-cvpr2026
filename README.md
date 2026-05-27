# Foundations and Frontiers of Watermarking — CVPR 2026 Tutorial

Static website for the CVPR 2026 half-day tutorial on watermarking.

**Date:** Thursday, June 4, 2026 · 1:00 PM – 5:00 PM · Denver, CO

Live site: <https://[username].github.io/watermarking-cvpr2026/> *(update once GitHub Pages is enabled)*

## Structure

```
watermarking-cvpr2026/
├── index.html       # Main page (single-page site with anchor sections)
├── styles.css       # Theme: clean academic, Newsreader + Inter
├── script.js        # Sticky-nav scroll-spy, mobile menu toggle, year stamp
├── assets/          # Logos, cover image, speaker portraits
├── LICENSE
└── README.md
```

## Local preview

This is plain static HTML/CSS/JS — no build step.

```bash
python3 -m http.server 8000
# then open http://localhost:8000
```

## Deploying via GitHub Pages

1. Push to `main`.
2. In the repo: **Settings → Pages → Source: Deploy from branch → `main` / root**.
3. The site will be served at `https://<user>.github.io/watermarking-cvpr2026/`.

## Editing the content

Most copy lives in `index.html`. Common updates:

- **Schedule:** edit `<ol class="schedule">` items (time, speaker, abstract).
- **Speakers:** edit `<article class="speaker-card">` blocks; replace `#` link placeholders with real homepage / Scholar URLs.
- **Reading list:** edit `<ul class="paper-list">` entries grouped by session in the Reading List section.
- **Materials:** when slides / code / video become available, replace the `href="#"` and `aria-disabled="true"` on each `.material-card` with the real link, and update the status pill text.
- **Venue / date:** update the `.venue-grid` items once CVPR 2026 confirms the date and room.

## Tutorial topics

- Classical watermarking foundations (spread spectrum, QIM, security)
- Modern deep-learning watermarking (encoder–decoder, perceptual & adversarial training)
- Multimodal watermarking (image, audio, video, 3D)
- Generative watermarking (Stable Signature, Tree-Ring, Gaussian Shading, sampler-level)
- Robustness benchmarking with WAVES
- Real-world authenticity: C2PA, Content Credentials, SynthID, watermark coexistence

## Speakers

- Dr. Vishal Asnani — Adobe Research
- Dr. Shruti Agarwal — Adobe Research
- Prof. Benedetta Tondi — University of Siena
- Dr. Pierre Fernandez — Meta AI (FAIR)
- Prof. Furong Huang — University of Maryland

## Contact

Questions: <vasnani@adobe.com>
