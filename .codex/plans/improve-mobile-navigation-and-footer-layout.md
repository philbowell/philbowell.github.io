# Improve Mobile Navigation And Footer Layout

Issue: https://github.com/philbowell/philbowell.github.io/issues/17

## Goal

Make the mobile header more flexible by replacing the stacked link row with a burger menu on the right opposite the wordmark, and tighten the mobile footer so it can use the available horizontal space more like desktop.

## Proposed Approach

- Update `_includes/nav.html` to add a mobile menu control next to the wordmark.
- Use a small amount of progressive-enhancement JavaScript in `_layouts/base.html` or a tiny inline script so the menu can open/close accessibly.
- Keep the desktop navigation visually unchanged.
- On mobile, keep the wordmark and burger button on one row.
- Present the mobile menu as a compact dropdown/panel aligned from the right, with clear tap targets and no layout shift in the header.
- Add accessible attributes/states for the menu button: `aria-expanded`, `aria-controls`, and a descriptive label.
- Add CSS for the burger icon using simple spans/pseudo-elements rather than an image asset.
- Adjust the footer mobile breakpoint so `.footer-meta` remains right-aligned when the viewport has enough room, and only stacks when genuinely narrow.
- Preserve the existing quiet visual language, spacing, type scale, colors, and no-card page structure.

## Verification

- Run a local preview.
- Check desktop nav still shows inline links and desktop footer remains unchanged.
- Check mobile width around the screenshot size: wordmark left, burger right, no nav links below the wordmark.
- Open and close the mobile menu with pointer interaction.
- Confirm menu links navigate correctly.
- Confirm footer intro and meta sit left/right where space allows, then stack cleanly at very narrow widths.
- Check console for errors.
- Check reduced-motion/accessibility basics where applicable.

## Files Likely To Change

- `_includes/nav.html`
- `_layouts/base.html`
- `assets/css/style.css`
