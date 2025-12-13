# neverneer

Personal lab, projects, experiments — all in black. This repository is the single-source for neverneer's public face: dark, animated, and unapologetically minimal.

> Never code....

---

## What this is

A purpose-built, ultra-dark personal site and project hub. The design favors pure black backgrounds, monochrome accents, and subtle motion: animated canvas particles, soft glows, and a radiant hero image (use licensed iStock assets for final visuals).

This branch (design/dark-animated) contains the experimental site shell: index.html, assets (CSS, JS, images), and this README.

---

## Preview notes

- Theme: Black-only base with white/gray accents. No color hues are intentionally used — rely on lightness, contrast, and motion.
- Hero visual: Replace assets/images/hero-radiant.jpg with a licensed iStock radiant image. Prefer images with deep blacks and directional light for dramatic glow.
- Motion: Lightweight canvas particle system (assets/js/scripts.js) drives subtle life behind the content. All motion respects prefers-reduced-motion.

---

## Local development

1. Clone the repository and check out the design branch:

```bash
git clone https://github.com/neverneer/neverneer.git
cd neverneer
git checkout design/dark-animated
```

2. Serve locally (any static server). Examples:

- Python 3:

```bash
python -m http.server 8080
# then open http://localhost:8080
```

- Node (serve package):

```bash
npx serve .
```

3. Edit files in `index.html`, `assets/css/styles.css`, and `assets/js/scripts.js`. Commit changes to the design branch.

---

## Assets & licensing

- The repo includes placeholder imagery. For production, license radiant/abstract images from iStock (or equivalent) and place them in `assets/images/`.
- Keep the images dark-first: deep blacks, controlled highlights, and minimal saturation. The CSS intentionally applies a monochrome filter; test with full-color images but prefer images that match the mood.
- If using paid assets, do not commit unlicensed originals to the public repo. Instead, add `assets/images/hero-radiant.jpg` via a secure release or host externally and reference by URL.

---

## Design choices & implementation notes

- Color system: background #000; surfaces #060606; accent whites and grays only.
- Animations: subtle — floating titles, particle canvas, image parallax/scale on hover. All animations are non-essential and disabled when a user sets reduced motion.
- Accessibility: semantic HTML, focus states inherited from system, and motion preferences respected. Run Lighthouse or axe-core for deeper audits.

---

## Deploying

- GitHub Pages: Enable Pages for the `design/dark-animated` branch (or merge to `gh-pages` or `main` as desired). The site is static and 100% compatible with Pages.

---

## Contributing

This is a personal repo — contributions are welcome but will be curated.

- Open issues for suggestions or visual assets.
- PRs should target `design/dark-animated` unless the change is a direct improvement for `main`.

---

## TODO / Roadmap

- Integrate licensed iStock radiant hero images.
- Add optional SVGO-optimized animated SVG accents (kept monochrome).
- Add a small CMS or JSON-driven lab feed for experiments.
- Automate asset release pipeline for licensed images (private release artifacts).

---

## Contact

For collabs, visuals, or questions: hello@neverneer.com

---

## License

MIT — see LICENSE file. For asset licensing (images, audio), follow vendor terms and avoid committing paid assets to the public repo.
