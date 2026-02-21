# FITVERSE Landing Page

A premium, mobile-first landing page for FITVERSE — the AI-powered trend intelligence app for fitness creators.

## Design Features

- **Dark theme** with #0a0a0a background and #10a37f green accent
- **Mobile-first responsive** design optimized for Instagram traffic
- **Single-page application** with smooth scroll animations
- **No frameworks** — pure HTML, CSS, and vanilla JavaScript
- **Fast loading** — optimized for < 2 second load times
- **Grid pattern background** with subtle visual depth

## Content Sections

1. **Hero Section** — FITVERSE branding with dual CTAs
2. **Today's Briefing Preview** — Live algo intelligence teaser
3. **Features Grid** — 6 core features in responsive grid
4. **Social Proof** — Creator-focused stats and testimonials
5. **How It Works** — Simple 3-step process
6. **Pricing Preview** — Free, Pro, and Autopilot tiers
7. **Email Capture** — Beta signup with lifetime pro offer
8. **Footer** — Clean branding and social links

## Deployment Instructions

### GitHub Pages Setup

1. **Create Repository**
   ```bash
   git init
   git add .
   git commit -m "Initial commit: FITVERSE landing page"
   git branch -M main
   git remote add origin https://github.com/yourusername/fitverse-site.git
   git push -u origin main
   ```

2. **Enable GitHub Pages**
   - Go to repository Settings > Pages
   - Set source to "Deploy from a branch"
   - Select branch: `main`
   - Select folder: `/docs`
   - Click Save

3. **Custom Domain Setup**
   - The CNAME file is already included in `/docs/`
   - Point your DNS A records to GitHub Pages:
     ```
     185.199.108.153
     185.199.109.153
     185.199.110.153
     185.199.111.153
     ```
   - Or use CNAME record pointing to: `yourusername.github.io`

### Local Development

1. **Simple HTTP Server**
   ```bash
   cd docs/
   python3 -m http.server 8000
   # Visit http://localhost:8000
   ```

2. **Live Reload (Optional)**
   ```bash
   npx live-server docs/
   ```

## File Structure

```
fitverse-site/
├── docs/                 # GitHub Pages source
│   ├── index.html       # Main landing page
│   └── CNAME           # Custom domain config
├── README.md           # This file
└── .gitignore         # Git ignore rules
```

## Browser Support

- **Modern browsers** (Chrome, Firefox, Safari, Edge)
- **Mobile optimized** for iOS Safari and Chrome on Android
- **Progressive enhancement** — core functionality works without JavaScript

## Performance

- **No external dependencies** — everything is embedded
- **Optimized images** — use modern formats (WebP, AVIF) when adding assets
- **CSS animations** — hardware accelerated transforms
- **Lazy loading** — intersection observer for scroll reveals

## Customization

### Colors
Edit CSS custom properties in the `:root` selector:
```css
:root {
    --bg-primary: #0a0a0a;      /* Main background */
    --bg-secondary: #111111;     /* Card backgrounds */
    --accent-green: #10a37f;     /* Primary accent */
    --text-primary: #ffffff;     /* Main text */
    --text-secondary: #999999;   /* Muted text */
}
```

### Content
All content is directly in the HTML file for easy editing. Key sections:
- Hero tagline and subtitle
- Today's briefing preview data
- Feature descriptions
- Pricing tiers
- Social proof stats

### Email Collection
Currently uses `mailto:` for form submission. For production:
- Integrate with Formspree, Netlify Forms, or ConvertKit
- Replace the form action and add proper handling

## SEO & Meta

- **Open Graph** tags configured
- **Twitter Card** meta tags
- **Structured data** ready for schema.org markup
- **Semantic HTML** with proper heading hierarchy
- **Alt tags** placeholders for future images

## Brand Voice

- **Lowercase everything** — matches gym bro aesthetic
- **Direct and confident** — no corporate fluff
- **Data-driven language** — "velocity", "intelligence", "optimize"
- **Aspirational but realistic** — "stop guessing" vs "get rich quick"

## Next Steps

1. **Add analytics** — Google Analytics or Plausible
2. **A/B testing** — headlines, CTAs, pricing
3. **Form integration** — proper email collection backend
4. **Image optimization** — hero graphics, feature icons
5. **Blog/content** — SEO content strategy

---

**Built by @mind2muscle.app • © 2026 fitverse**