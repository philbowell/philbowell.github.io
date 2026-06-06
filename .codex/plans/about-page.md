# About Page

Issue: #8

## Goal

Turn the new `about.md` draft and profile image into a finished `/about` page that fits the site's quiet personal portfolio style and gives visitors a warmer biographical view alongside the home page and CV.

## Current Context

- `about.md` exists but currently has no Jekyll front matter, so it is not yet wired into the site layout.
- Two new image assets exist:
  - `assets/images/philbowell.jpg` — original, 4037x3488.
  - `assets/images/philbowell-optim.jpg` — optimized, 2020x1744.
- The site currently has top-level Home, CV, and Colophon pages, with navigation showing Home and CV only.
- The design system is deliberately restrained: warm off-white background, near-black text, muted secondary text, sage accent, Figtree, generous spacing, no JavaScript.

## Proposed Approach

- Add Jekyll front matter to `about.md` using the existing `base` layout and `About` title.
- Shape the page as an editorial biography rather than a generic profile page:
  - a short hero/introduction area,
  - the provided portrait image,
  - the existing biographical copy in readable sections,
  - a closing link onward to the CV.
- Use `assets/images/philbowell-optim.jpg` in the page so the served asset is lighter than the original.
- Add an About link to `_includes/nav.html` if you want About to be a primary page alongside Home and CV.
- Add scoped About styles in `assets/css/style.css`, reusing the existing spacing, type, colour, and responsive patterns.
- Keep the implementation static: no JavaScript, no new dependencies, no local Jekyll requirement.

## Detail Notes

- The current draft has a natural chronological arc: Southwell, early interest in drawing/design, exploring spatial design, graphic design education, career evolution, and purpose-led work.
- The phrase "next step in to Higher Education" likely wants a copy check before publishing. I will not change meaning without confirmation.
- The portrait aspect ratio is close to square/landscape. The layout should avoid awkward face cropping and should be checked on mobile before considering it done.
- The page should stay visually consistent with the Colophon and CV pages without introducing a heavy card layout.

## Files

- `about.md`
- `_includes/nav.html`
- `assets/css/style.css`

## Verification

- Serve the site locally with `python3 -m http.server` or another static smoke check suitable for the current Jekyll-free setup.
- Open `/about/` or `/about` in the browser and check:
  - page renders through the base layout,
  - portrait loads correctly,
  - nav link resolves if added,
  - desktop layout has a clear hierarchy,
  - mobile layout does not crop or overlap text/image awkwardly.
- Re-check Home, CV, and Colophon quickly to make sure shared CSS/nav changes do not regress existing pages.

## Questions Before Build

- Should About be added to the main nav now, between Home and CV?
- Are you happy for me to lightly edit the copy for flow, punctuation, and the "in to Higher Education" wording, while preserving your voice?
- Should the page use the optimized image only, leaving the original in the repo, or should the original be excluded/removed later if it is not needed?
