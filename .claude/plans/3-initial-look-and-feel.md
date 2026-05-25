# Plan — Issue #3: Initial look and feel

## Goal

Get a live, styled page on GitHub Pages: Jekyll scaffold wired up, design tokens in place, Figtree loaded, home page readable.

## Files to create / modify

| File | Action |
|------|--------|
| `_config.yml` | Create |
| `_layouts/base.html` | Create |
| `_includes/nav.html` | Create |
| `_includes/footer.html` | Create |
| `assets/css/style.css` | Create |
| `assets/images/pbdesignlogo.svg` | Move from root |
| `index.md` | Create |

`cv.md` is out of scope for this issue — content is substantial and warrants its own issue.

---

## Implementation notes

### `_config.yml`
- `title: Phil Bowell`
- `url` and `baseurl` left empty (GitHub Pages user site, root domain)
- `markdown: kramdown`
- Exclude `scaffold.md`, `README.md`, `.claude/`

### `_layouts/base.html`
- `<!DOCTYPE html>` shell
- Figtree via Google Fonts: weights 300, 400, 500 + italics 300, 400
- `<meta name="viewport">` for mobile
- Includes `nav.html` and `footer.html`
- `{{ content }}` in `<main>`

### `_includes/nav.html`
- SVG wordmark linked to `/`
- Nav links: Home · CV
- No active state logic yet (can add later)

### `_includes/footer.html`
- Single line: `phil@philbowell.com`
- No additional content in initial scope

### `assets/css/style.css`
Design tokens as CSS custom properties:
```css
--color-bg: #f5f3ef;
--color-text: #1c1c1a;
--color-secondary: #6b6b6b;
--color-accent: #3d7a5c;
--color-wordmark: #424649;
```
Base styles:
- `font-family: 'Figtree', sans-serif`
- Fluid type scale using `clamp()`
- Max-width container, centred
- Nav: wordmark left, links right
- Mobile: single-column, stacked nav

### `index.md`
- Layout: `base`
- Tagline: *"I design experiences that understand people and solve problems that matter."*
- Bio: *"I'm a designer and visual artist with 20 years' experience in the creative industries. I've worked across branding, web design, and UX, and I bring all of that together to understand people, tell stories, and solve problems that matter."*
- Contact link: `phil@philbowell.com`

---

## Commit message

```
Build initial Jekyll scaffold and base styles

Closes #3
```
