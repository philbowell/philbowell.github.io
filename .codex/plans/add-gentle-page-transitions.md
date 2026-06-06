# Add Gentle Page Transitions

Issue: https://github.com/philbowell/philbowell.github.io/issues/16

## Goal

Make navigation between pages feel less choppy with a subtle transition that fits the quiet portfolio feel.

## Approach

- Use a short CSS-only fade on the main content area, keeping the site JavaScript-free.
- Scope the transition to page content so navigation feels smoother without becoming showy.
- Respect `prefers-reduced-motion` by disabling transition animation for people who request less motion.
- Keep timing short and restrained so pages still feel fast.

## Verification

- Run the site locally.
- Check Home, About, CV, and Colophon navigation in a browser.
- Confirm there are no layout regressions at desktop and mobile widths.
- Confirm reduced-motion CSS is present.
