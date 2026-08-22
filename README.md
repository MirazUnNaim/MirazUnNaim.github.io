# Miraz Un Naim — Portfolio

Personal portfolio site, built as a single self-contained HTML file. All
content (name, bio, projects, skills, coursework, contact links) lives in
one `SITE_DATA` object near the top of the `<script>` tag, and the page
renders itself from that object — no build step, no server, no separate
data file. Works by double-clicking the file, from GitHub Pages, or in
any preview tool.

**Live site:** https://mirazunnaim.github.io/

## Tech
- HTML5, CSS3 (no framework)
- Vanilla JavaScript — renders the DOM from an inline data object
- Fonts: Inter, Fraunces, JetBrains Mono (Google Fonts)

## Structure

- `index.html` — markup, styling, data, and render logic (everything)
- `AI_USAGE.md` — AI tool disclosure
- `README.md` — this file

## Running locally
Just open `index.html` directly in a browser — no server needed.

## Updating content
Open `index.html`, find `const SITE_DATA = { ... }` near the top of the
`<script>` block, and edit it — add a project object to `projects.own` or
`projects.contrib`, a course to `academic.courses`, a skill to `skills`,
etc. The page re-renders itself from that data on every load.

## Sections
- **About** — background and current focus
- **Projects** — own repositories and team contributions
- **Skills** — languages, backend/APIs, systems/CS, tools, concepts
- **Academic** — enrollment info and coursework
- **Notes** — short writeups on projects
- **Contact** — email, GitHub, LinkedIn

## AI tool disclosure
See [`AI_USAGE.md`](./AI_USAGE.md) for the tools used and prompt history.
