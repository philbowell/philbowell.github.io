# Create Colophon Page

Issue: #14

## Goal

Add a `/colophon` page that explains how the site is made, in a concise editorial style that fits the current quiet portfolio design.

## Approach

- Create `colophon.md` using the base layout and existing Markdown/HTML page pattern.
- Structure the page as a short introduction followed by focused sections for design, type, build, hosting, and source/materials.
- Keep the content specific to this site: Jekyll, GitHub Pages, single CSS file, Figtree, warm off-white palette, no JavaScript in the initial build.
- Add scoped CSS for the colophon page only where the global typography is not enough.
- Verify the page can be served locally and that the existing footer link resolves.

## Files

- `colophon.md`
- `assets/css/style.css`

## Checks

- Local static server smoke check.
- Browser check for `/colophon`.
