# philbowell.github.io — Scaffold

## Status
🟡 Planning complete. Ready to build.

---

## Decisions Log

### Technical
- **Platform**: Jekyll via GitHub Pages (native build, no local install)
- **Deployment**: Push to `main`, GitHub builds automatically
- **JavaScript**: None for initial build
- **CSS**: Single file (`assets/css/style.css`), built on custom properties for future dark mode
- **Fonts**: Figtree via Google Fonts (single request, no JS)
- **Dark mode**: Future — CSS custom properties in place from the start

### Pages (initial scope)
- Home (`index.md`)
- CV (`cv.md`)

### Visual Direction
- Aesthetic references: Karolis Kosas, Naz Hamid
- Mode: Light first
- Background: Warm off-white `#f5f3ef`
- Text: Near-black `#1c1c1a`
- Secondary text: Mid-grey `#6b6b6b`
- Accent: Muted sage-forest green `#3d7a5c` — to be confirmed on first build
- Wordmark colour: `#424649` (as per SVG)

### Assets
- Wordmark: `pbdesignlogo.svg` — horizontal lockup, dark charcoal on light background
- Profile photo: Not included in initial scope

### Content

#### Home
- Tagline: *"I design experiences that understand people and solve problems that matter."*
- Bio: *"I'm a designer and visual artist with 20 years' experience in the creative industries. I've worked across branding, web design, and UX, and I bring all of that together to understand people, tell stories, and solve problems that matter."*
- Contact: `phil@philbowell.com`

#### CV
- Content sourced from uploaded CV document
- Sections: Professional History · Key Freelance Projects · Tools & Expertise · Academic Background
- Format: Web only (no PDF download in initial scope)
- Copy: Presented as-is from source document

---

## File Structure

```
philbowell.github.io/
├── _config.yml
├── _layouts/
│   └── base.html
├── _includes/
│   ├── nav.html
│   └── footer.html
├── assets/
│   ├── css/
│   │   └── style.css
│   └── images/
│       └── pbdesignlogo.svg
├── index.md
├── cv.md
└── scaffold.md
```

---

## Build Checklist

### Setup
- [ ] `_config.yml`
- [ ] `_layouts/base.html`
- [ ] `_includes/nav.html`
- [ ] `_includes/footer.html`
- [ ] `assets/css/style.css`
- [ ] Move `pbdesignlogo.svg` to `assets/images/`

### Pages
- [ ] `index.md` — Home
- [ ] `cv.md` — CV

### Design
- [ ] Confirm accent green on first build
- [ ] Typography review (DM Sans)
- [ ] Mobile / responsive review

### Future (out of scope for now)
- [ ] Dark mode
- [ ] CV PDF download
- [ ] Work / portfolio page
- [ ] Contact form
- [ ] Profile photo
