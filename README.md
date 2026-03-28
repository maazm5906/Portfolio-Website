# Muhammad Maaz — Portfolio

A **single-page portfolio** with a dark, editorial layout: animated sections, project grid, achievements, skills, and contact. Built as a static site you can host anywhere.

**Repository:** [github.com/maazm5906/Portfolio-Website](https://github.com/maazm5906/Portfolio-Website)

![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?logo=react&logoColor=61DAFB)
![Vite](https://img.shields.io/badge/Vite-646CFF?logo=vite&logoColor=white)

---

## What’s in this folder

| Path | Role |
|------|------|
| `index.html` | Entry point; mounts the React app on `#root` |
| `assets/index-BvSJQQrT.js` | Production JavaScript bundle (React + animations + sections) |
| `assets/index-BJU7kQDh.css` | Compiled styles (Tailwind / design tokens) |

This repo holds the **built output** of a Vite + React project (source files are not included). Edits to copy, links, or section data are done by carefully updating the minified bundle, or by rebuilding from the original source project if you still have it.

---

## Run it locally

Any static file server works. Examples:

```bash
# Node 18+ (no install)
npx --yes serve .

# Or Python
python -m http.server 8080
```

Then open the URL shown in the terminal (e.g. `http://localhost:3000` or `http://localhost:8080`).

> Use a server instead of opening `index.html` directly so module scripts and asset paths resolve correctly.

---

## Assets next to `index.html`

Place optional media in the **same directory as `index.html`** (or paths that match your bundle). Examples referenced by the site:

- **CV:** `Maaz Europass CV.pdf` (or the filename encoded in the bundle)
- **Hero portrait:** `hero-portrait.jpeg`
- **Project thumbnails:** e.g. `Vibran Eat.jpeg`, `AI Doctor.png`, `Plant Doctor.png`, `mask detection.png`, `LLM-Agents.png`, `hand written digit generation.png`
- **Certificates / community:** PDFs and PNGs as linked in Achievements (URL-encoded names for spaces)

If an image 404s, check **exact filename** and **encoding** in `index-BvSJQQrT.js` (spaces → `%20`).

---

## Deploy

1. Upload the folder (at minimum `index.html` + `assets/` + your media files).
2. Set the host’s root to this folder.
3. Examples: **GitHub Pages**, **Netlify**, **Cloudflare Pages**, **Vercel** (static), or any nginx/Apache static host.

No build step is required on the server if you deploy this bundle as-is.

---

## Customization notes

- **Text & links** live inside `assets/index-BvSJQQrT.js`. Search for visible strings (e.g. email, GitHub username, project titles) and replace in one pass; keep quotes and commas valid JavaScript.
- **Styles** are in `assets/index-BJU7kQDh.css` (large, minified). Prefer changing the source Tailwind/theme and rebuilding if you have it.
- **Title / meta:** edit `index.html` `<title>` and add `<meta name="description">` for SEO.

---

## License

Personal portfolio — © Muhammad Maaz. Code/bundle usage: keep attribution unless you own the rights to replace it.

---

<p align="center">
  <sub>Built with care for clarity, motion, and a strong first impression.</sub>
</p>
