# paulas.world — Business Strategy Portfolio

**Version 3.0** — Bilingual (EN/FR) portfolio website targeting master's programs in Business Strategy and Finance in Paris. Program-agnostic. September 2028 entry.

---

## Quick Deploy to Netlify

### Option 1: Drag and Drop (Fastest)

1. Go to [Netlify Drop](https://app.netlify.com/drop)
2. Drag the folder containing `index.html`, `README.md`, and `_redirects`
3. Your site goes live in seconds

### Option 2: GitHub + Netlify (Recommended for ongoing updates)

**Step 1 — Push to GitHub:**

```bash
git add index.html README.md _redirects
git commit -m "Portfolio v3.0 — program-agnostic strategy focus"
git push origin main
```

**Step 2 — Connect Netlify:**

1. Go to [app.netlify.com](https://app.netlify.com)
2. Click "Add new site" then "Import an existing project"
3. Choose GitHub and select your repository
4. Build settings: leave blank (static site, no build command needed)
5. Click "Deploy site"

**Step 3 — Custom Domain:**

1. In Netlify: Site settings → Domain management
2. Add custom domain: `paulas.world`
3. Follow Netlify's DNS instructions (propagation takes 24–48 hours)

---

## File Structure

```
paulas.world/
├── index.html              # Main bilingual site (EN/FR toggle)
├── cv-paula-zambrano.pdf   # Your CV — add this file before deploying
├── README.md               # This file
└── _redirects              # Netlify routing configuration
```

---

## Adding Your CV

Before your first deployment, add your CV to the root directory:

1. Export your CV as a PDF
2. Name it exactly: `cv-paula-zambrano.pdf`
3. Place it in the same folder as `index.html`
4. The "Download CV (PDF)" button will work automatically

---

## Content Overview

### Sections

1. **Hero** — Tagline: "Golf Operations → Business Strategy" with Paris 2028 framing
2. **Portfolio** — Three quantitative projects (GitHub placeholder links ready to update)
3. **About** — NYU background, Puerto Los Cabos operations, trilingual, consulting target
4. **Skills** — Technical, Business, Languages and Certifications (including planned GMAT and DELF B2)
5. **Blog** — Two upcoming posts (May and June 2026)
6. **Contact** — Netlify form integration + email
7. **Footer** — Navigation links and social

### Language Toggle

- Default: English
- Toggle: EN / FR button in the navigation bar
- All sections fully translated into French

---

## Updating Content

All text content lives in the `translations` object near the top of the `<script>` block in `index.html`.

### To update project GitHub links (when repos are ready):

Find this section in the `en` translations:

```javascript
projects: [
  {
    num: "01",
    name: "Golf Club Financial Analysis",
    github: "#",   // Replace with: "https://github.com/YOUR-USERNAME/golf-financial-analysis"
    report: "#"    // Replace with: "/portfolio/golf-analysis.html" or external link
  },
  ...
]
```

Repeat the same update in the `fr` translations block.

### To update blog post links (when posts are published):

```javascript
posts: [
  {
    // ...
    link: "/blog/fairways-to-finance.html"  // Add this field when ready
  }
]
```

---

## Design System

### Color Palette

| Name    | Hex       | Usage                          |
|---------|-----------|--------------------------------|
| Cream   | `#FAF7F2` | Backgrounds, hero right panel  |
| Rose    | `#E8C5B5` | Cursor, orb ring, accents      |
| Sage    | `#9DAD91` | Tag borders                    |
| Brown   | `#5B3B1E` | Primary text, buttons, grid    |
| Navy    | `#2E5090` | Section labels, highlights, CTA hover |
| Linen   | `#EDE8E0` | Borders, separators            |

### Typography

- **Headings:** Krona One (Google Fonts)
- **Body:** Space Grotesk (Google Fonts)

### Animations

- Custom magnetic cursor (rose dot, grows on hover)
- Floating hero orb (CSS keyframe)
- Fade-up scroll animations (IntersectionObserver)
- Marquee ticker strip

---

## Responsive Breakpoints

- **Desktop:** > 968px — two-column layouts
- **Mobile/Tablet:** ≤ 968px — single column, stacked sections

---

## Netlify Features

### Contact Form

The contact form uses Netlify's built-in form handling (`data-netlify="true"`). To receive email notifications:

1. Deploy the site to Netlify
2. Go to Site Settings → Forms
3. Add notification email: `paulazmbrn@outlook.com`

Form submissions appear in your Netlify dashboard under "Forms."

### Redirects

The `_redirects` file handles:
- SPA fallback routing (`/* → /index.html`)
- Contact form redirect

---

## Phase Roadmap

### Now (March 2026)
- Deploy v3.0 to Netlify via GitHub push
- Add `cv-paula-zambrano.pdf` to repository
- Test language toggle and contact form

### April–May 2026
- Build Project 1 (Golf Financial Analysis) in Python/Excel
- Create GitHub repository with real code
- Update portfolio GitHub link
- Draft Blog Post 1 ("From Fairways to Finance")

### June–July 2026
- Complete DELF B2 exam (planned June 2026)
- Complete Projects 2 and 3
- Publish Blog Post 1
- Draft Blog Post 2 ("Luxury Brand Management")
- Begin GMAT preparation (exam planned July 2026)

### August 2026 onward
- Add professional headshot (replace "P" placeholder)
- Add Google Analytics
- Share blog posts on LinkedIn
- Refine copy with feedback from alumni and mentors

---

## Troubleshooting

**Contact form not submitting:** Forms only work on Netlify (not on localhost). Deploy first, then test.

**Language toggle not switching:** React loads via CDN — check internet connection and browser console for errors.

**Custom domain not working:** DNS propagation takes 24–48 hours after pointing records to Netlify.

**CV download not working:** Confirm `cv-paula-zambrano.pdf` exists in the root directory of your deployed site.

---

## Application Integration

When submitting applications, reference the site as:

- **CV header:** `paulas.world | LinkedIn | GitHub`
- **Statement of Purpose:** Reference specific projects by name as evidence of quantitative and strategic skills
- **Interview:** Pull up the portfolio to walk through project methodology

---

**Version:** 3.0 (Program-Agnostic Strategy Focus)
**Last Updated:** March 2026
**Next Review:** After Project 1 completion — May 2026
# Paulas-Portfolio
