# Plan — Add CV Page

## Goal

Add a Jekyll CV page to the current site using the content from `/Users/phil/Sites/Personal Site/cv.html`, while discarding that page's standalone design, navigation, scripts, animation classes, and font dependency.

## Implementation

- Create `cv.md` with `layout: base` and `title: CV`.
- Convert the source CV content into semantic page markup:
  - `Curriculum Vitae`
  - `Professional history`
  - `Key freelance projects`
  - `Tools & expertise`
  - `Academic background`
- Preserve the original wording, correcting HTML entities where needed.
- Keep the existing `/cv` navigation target.
- Extend `assets/css/style.css` with CV-specific classes that use the current Figtree-based visual system, quiet spacing, subtle dividers, and responsive layouts.
- Do not add JavaScript, a burger menu, old nav links, the old `styles.css`, DM Sans, a PDF download, or portfolio/contact pages.

## Verification

- Confirm `cv.md` exists and uses the `base` layout.
- Confirm the existing nav still links to `/cv`.
- Check the rendered structure for desktop two-column role rows and mobile single-column flow.
- Run a local Jekyll build if available.

## Workflow Note

The GitHub issue and issue comments could not be created from this environment. The GitHub CLI is unavailable, and the GitHub plugin returned `403 Resource not accessible by integration` when creating the issue.
