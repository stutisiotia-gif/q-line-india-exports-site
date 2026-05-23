# Garment Manufacturing & Exports — Company Website

A clean, modern B2B website for an Indian garment manufacturing and exports business. Built as a single-page HTML site — no frameworks, no build tools, no dependencies beyond Google Fonts.

## Structure

```
garment-website/
├── index.html        ← The entire website (HTML + CSS + JS)
├── images/           ← Drop your images in here (see guide below)
└── README.md
```

## How to publish on GitHub Pages

1. Push this repository to GitHub
2. Go to **Settings → Pages**
3. Under *Source*, select **Deploy from a branch**
4. Choose `main` branch, `/ (root)` folder
5. Click **Save** — your site will be live at `https://yourusername.github.io/repo-name`

## Replacing placeholder images

Every image slot in the site has a labelled placeholder. To swap one in, find the relevant `<div class="... -img ...">` block and replace it with a standard `<img>` tag:

```html
<!-- BEFORE (placeholder) -->
<div class="hero-img-placeholder">
  <div class="img-placeholder-icon">...</div>
  <span class="img-placeholder-label">Hero image — factory / fabric</span>
</div>

<!-- AFTER (real image) -->
<img src="images/hero.jpg" alt="Factory floor" style="width:100%; height:100%; object-fit:cover;" />
```

### Image slots and suggested filenames

| Location | Placeholder label | Suggested filename |
|---|---|---|
| Hero (right half) | Hero image — factory / fabric | `images/hero.jpg` |
| Process section | Quality testing image | `images/quality-testing.jpg` |
| Indian Oil project card | Indian Oil uniforms | `images/project-indian-oil.jpg` |
| Taj Group project card | Taj Group uniforms | `images/project-taj.jpg` |
| School uniforms project card | School uniform programme | `images/project-schools.jpg` |

Images work best at these dimensions:
- Hero: **1200 × 900px** minimum, landscape
- Process detail: **800 × 600px**, landscape
- Project cards: **600 × 400px**, landscape

## Things to customise before going live

Open `index.html` and search for these placeholders:

| Placeholder | What to change it to |
|---|---|
| `ThreadsIndia` (nav + footer logo) | Actual business name |
| `Est. [Year]` | Founding year |
| `info@threadsindia.com` | Real email address |
| `+91 [number]` | Real phone number |
| `© 2025 ThreadsIndia` | Business name + correct year |
| `30+`, `50+`, `10K+` (hero stats) | Real figures from the owner |

## Translations

The site has English, Hindi, and Arabic language switching built in. The English copy is complete. The Hindi and Arabic body copy is currently machine-translated — have a native speaker review and correct it before publishing.

## Tech notes

- Pure HTML/CSS/JS — no React, no build step, no npm
- Fonts loaded from Google Fonts (Cormorant Garamond + DM Sans)
- Scroll animations use the native `IntersectionObserver` API
- Fully responsive down to mobile (breakpoint at 900px)
- Works on all modern browsers
