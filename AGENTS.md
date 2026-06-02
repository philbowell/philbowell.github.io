# AGENTS.md — philbowell.github.io

## Project

Personal site and portfolio. Jekyll via GitHub Pages — push to `main`, GitHub builds automatically. No local Jekyll install required.

**Pages (initial scope):** Home (`index.md`) · CV (`cv.md`)

See `scaffold.md` for full decisions log, visual direction, content, and build checklist.

---

## How We Work

### Issues are the source of truth

Every piece of work has a GitHub Issue. Nothing gets built without one.

**Label taxonomy**

Where: `home` · `cv` · `global` (nav, footer, CSS, config)

What: `design` · `content` · `infrastructure`

### Plans live in the repo

Before building, write a plan to `.Codex/plans/<issue-slug>.md` and link it from the issue as a comment.

### Commits close issues

Use `Closes #N` in commit messages to auto-close issues on merge to `main`.

Do not commit or push changes until Phil explicitly gives permission. Build and verify the work first, then wait for approval before staging, committing, or pushing.

### Issues get a closing comment

When work is done, comment on the issue with the commit link and a one-line summary of what changed.

### State tracking

Open/closed issue state only — no GitHub Project board.

---

## Workflow in Practice

1. Agree a task
2. Create a GitHub Issue with appropriate labels
3. Write a plan to `.Codex/plans/<issue-slug>.md`
4. Link the plan from the issue as a comment
5. Build and verify the change
6. Wait for Phil's explicit permission before staging, committing, or pushing
7. Commit with `Closes #N`
8. Comment on the issue with the commit link and a one-line summary

---

## Tech Stack

- **Platform:** Jekyll via GitHub Pages
- **Deployment:** Push to `main`
- **JavaScript:** None (initial build)
- **CSS:** `assets/css/style.css` — single file, built on CSS custom properties
- **Fonts:** Figtree via Google Fonts

## Design Tokens

- Background: `#f5f3ef`
- Text: `#1c1c1a`
- Secondary text: `#6b6b6b`
- Accent: `#3d7a5c` (muted sage-forest green — confirm on first build)
- Wordmark: `#424649`

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
└── cv.md
```
