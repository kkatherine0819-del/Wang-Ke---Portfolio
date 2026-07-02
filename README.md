# Ke Wang (王柯) — Personal Portfolio

Clean, modern, mobile-responsive bilingual portfolio for Ke Wang, HKU BBA student double-majoring in Marketing & Finance with strong interests in strategy consulting and sustainable marketing.

**Live preview**: Open `index.html` in any browser.

## Features

- **Hero** with custom-generated professional portrait
- **About, Education, Experience, Projects, Skills, Contact**
- **Bilingual ready**: English primary with seamless 中文 toggle (persists)
- **4 key project cards** with custom Grok Imagine visuals (academic yet dynamic style)
- **Fully responsive** (mobile hamburger, fluid grids, touch-friendly)
- **Smooth navigation** + active section scroll-spy
- **Interactive project modals** (bilingual)
- **Downloadable resume** (authentic PDF)
- **Functional contact form** (mailto integration + toast)
- Minimalist deep blue + fresh green palette
- Self-contained (Tailwind CDN + vanilla JS)

## Quick Start

```bash
# From the portfolio folder
cd wangke-portfolio

# Simple local server (Python)
python3 -m http.server 8000

# Or
npx serve .

# Open http://localhost:8000
```

## Structure

```
wangke-portfolio/
├── index.html              # Everything lives here (single-file friendly)
├── assets/
│   ├── images/
│   │   ├── hero-portrait.jpg
│   │   ├── project-ow.jpg
│   │   ├── project-ipsos.jpg
│   │   ├── project-meituan.jpg
│   │   └── project-sustainable-fashion.jpg
│   └── resume/
│       └── Wang_Ke_Resume.pdf
└── README.md
```

## Customization

**Bilingual content**
- All strings live in the `translations` object inside `<script>` in `index.html`.
- Add new keys under both `en` and `zh` and use `data-i18n="your.key"` on elements.

**Projects**
- Edit the `projects` JS array (title, short, full, details, image paths).
- To add a 5th project, duplicate a card in HTML + entry in the array + update the modal function.

**Images**
- Hero + 4 project visuals were generated with Grok Imagine using targeted academic-dynamic prompts.
- Replace by dropping new images into `assets/images/` and updating `src` attributes.
- Recommended aspects: hero ~3:4 or square, projects 16:9 or 1:1.

**Colors**
- Deep navy: `#0F172A`, `#1E3A5F`
- Fresh green: `#059669`, `#10B981`
- Edit in the `<style>` tag or Tailwind classes.

**Resume**
- Current PDF is the authentic version from applications.
- To generate a new / bilingual version, use your preferred tool and replace the file in `assets/resume/`.

## Deployment

**GitHub Pages (easiest)**
1. Push to a repo (e.g. `username/ke-wang-portfolio`)
2. Settings → Pages → Source: Deploy from `main` branch / root
3. Done. Update social links / email as needed.

**Netlify / Vercel**
- Drag & drop the whole folder or connect the repo. Zero-config.

**Single-file**
- The site works great when opened directly. For production, consider inlining the Tailwind CDN if you prefer offline.

## Notes

- Form submits via `mailto:` (best for static). Replace with Formspree / Netlify Forms if desired.
- Images were generated via Grok Imagine. Always review generated assets for brand / likeness accuracy before sharing widely.
- No backend or tracking included by design.

## Credits

Built for Ke Wang (王柯) — HKU BBA (Marketing & Finance).

Content derived from real experience including:
- Roland Berger NEV strategy project
- Ipsos medical aesthetics consumer research
- Oliver Wyman IMPACT case competition
- Meituan Business Analytics Competition (Team Lead)

---

Questions or updates? Reach out via the contact section on the site.