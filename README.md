# Blanchard — Art Gallery (Landing Page)

🔗 **[Live Demo](https://blanchar.netlify.app/)**  

A static landing page built per **design mockup** and **technical specification** with a focus on **mobile responsiveness**, **semantic HTML**, **cross‑browser support**, and **pixel‑perfect** layout.

> Built according to the course technical brief (RU): see the *Blanchard — artistic gallery* requirements. fileciteturn1file0

## ✨ Features

- **Responsive layout** (desktop → tablet → mobile), pixel‑perfect (±1–3px)
- **Semantic HTML5** + basic **a11y** (landmarks, headings, ARIA on interactive controls)
- **Cross‑browser compatibility** (Chrome, Firefox, Safari, Opera, Edge) with Normalize.css
- **Vanilla JS**, no external dependencies
- **Smooth anchor navigation** from header menu
- **Content sections:**
  - **About** — title + description
  - **Gallery** — title, note, responsive images via `<picture>`/`srcset`
  - **Catalog** — artist cards with image, title, dates (`<time>`)
  - **Events** — cards (image, place/date, description, “Read more”)
  - **Projects** — partner logos
  - **Contacts** — address, validated form (name/phone patterns), WhatsApp/Telegram links
- **Assets & performance basics:**
  - Separate `style.css` and `media.css`
  - Optimized images for breakpoints (`*-320/768/1024/1920`)
  - Local webfonts **Open Sans** (`woff/woff2`)
  - Favicon set (`favicon.ico`)

## 🛠 Tech Stack

- HTML5
- CSS3 (Flexbox, media queries, BEM-ish naming)
- JavaScript (ES6+, small modules)
- Normalize.css
- Local fonts (Open Sans `woff/woff2`)

## 🗂 Project Structure

```
.
├─ index.html
├─ .editorconfig
├─ .vscode/settings.json
├─ css/
│  ├─ normalize.css
│  ├─ style.css
│  ├─ media.css
│  └─ font_face.css
├─ img/               # responsive assets, SVG icons
├─ fonts/             # Open Sans (woff/woff2)
└─ favicon/
   └─ favicon.ico
```

## 🧩 Key Implementation Notes

- **Responsive images** with `<picture>` and multiple `srcset` sizes
- **Header nav** anchors provide **smooth scroll** to sections
- **Form validation** via HTML `pattern` (letters for name, digits for phone)
- **Accessibility**:
  - Informative `alt` text on images
  - Keyboard‑focusable controls with clear focus styles
  - ARIA labels where appropriate
- **BEM‑style class naming** and minimized media query set, per spec. fileciteturn1file0

## 🚀 Run Locally

No build step required.

**Option 1 — open as file:**  
- Double‑click `index.html` (note: some browsers restrict features on `file://`)

**Option 2 — local server (recommended):**
```bash
# Python
python -m http.server 5500

# or Node
npx http-server -p 5500

# open
http://localhost:5500
```

## 📦 Deploy

Any static hosting works:

- **GitHub Pages** (enable Pages on `main`)
- **Netlify** / **Vercel** (drag‑and‑drop folder or connect repo)

## ✅ Cross‑Browser & QA Checklist

- Tested on latest Chrome/Firefox/Safari/Edge/Opera (per brief) fileciteturn1file0
- Validate HTML with W3C Validator
- Check portrait/landscape on mobile/tablet
- Ensure hover vs. `:active` behavior on touch devices (per brief) fileciteturn1file0
- Lighthouse pass (Performance/A11y/Best Practices/SEO)

## 🗺 Roadmap / Ideas

- [ ] Enhance keyboard focus management for interactive blocks
- [ ] Add JS‑side form validation and success/failure UI
- [ ] Respect `prefers-reduced-motion` for transitions
- [ ] Add tests for anchor scrolling and section visibility

## 🖋 License


