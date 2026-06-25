# Reanty — Real Estate Landing Page

Static front-end landing page for the Reanty real estate brand. No backend or database is required.

## Deliverables Checklist

| Item | Status | Notes |
|------|--------|-------|
| Source code | Included | `index.html`, `css/`, `images/` |
| Responsive (desktop + mobile) | Done | CSS breakpoints at 1170px, 900px, 768px, 576px |
| Relative paths | Done | All assets use `./` relative URLs |
| Staging / testing URL | **Deploy required** | See [Deployment](#deployment) below |
| Database / server backup | **N/A** | Static HTML/CSS site — no database |

## Project Structure

```
Test_Fastcoding/
├── index.html          # Main page
├── css/
│   ├── style.css       # Layout & components
│   └── animations.css  # Motion & CSS-only sliders
├── images/             # Icons, banners, photos
└── README.md           # This file
```

## Local Development

### Option 1 — VS Code Live Server

1. Open the project folder in VS Code.
2. Install the **Live Server** extension (if not installed).
3. Right-click `index.html` → **Open with Live Server**.
4. Browser opens at `http://127.0.0.1:5500` (port may vary).

### Option 2 — Python (built-in)

```bash
cd Test_Fastcoding
python -m http.server 8080
```

Open `http://localhost:8080` in your browser.

### Option 3 — Node.js `serve`

```bash
npx serve .
```

## Deployment (Staging URL)

Deploy the project root (folder containing `index.html`) to any static host:

### Netlify (recommended, free)

1. Sign up at [netlify.com](https://www.netlify.com).
2. Drag and drop the project folder into Netlify Drop, **or** connect a Git repo.
3. Publish directory: project root (`.`).
4. Netlify provides a URL like `https://your-site-name.netlify.app`.

### Vercel

```bash
npm i -g vercel
cd Test_Fastcoding
vercel
```

### GitHub Pages

1. Push the repo to GitHub.
2. **Settings → Pages → Source**: Deploy from branch `main`, folder `/ (root)`.
3. URL: `https://<username>.github.io/<repo-name>/`.

> **For submission:** Replace this placeholder with your live staging URL after deployment.

**Staging URL:** `_Add your deployed URL here_`

## Technical Notes

- **Stack:** HTML5, CSS3 (no JavaScript framework).
- **Fonts:** Google Fonts (Poppins, Nunito) — loaded via CDN.
- **Interactivity:** CSS-only (sliders, tabs, scroll animations).
- **Browser support:** Modern evergreen browsers (Chrome, Firefox, Safari, Edge).
- **Database:** Not applicable. Forms are presentational; wire to a backend if needed.

## Testing Checklist

- [ ] Desktop layout (≥ 1200px): header, hero, all sections
- [ ] Tablet (768px–1170px): grid columns collapse correctly
- [ ] Mobile (≤ 768px): topbar stacks, hero image on top, nav wraps
- [ ] All images load (relative paths)
- [ ] Sticky header works on scroll
- [ ] House sliders and featured tabs respond to clicks

## Contact / Handover

When submitting work, include:

1. **Source code** — this repository or a ZIP of the project folder.
2. **Staging URL** — live link from Netlify/Vercel/GitHub Pages.
3. **Database backup** — not required for this project.
