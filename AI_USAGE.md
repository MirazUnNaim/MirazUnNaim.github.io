# AI Tool Usage Disclosure

## Tool used
**Claude** (Anthropic) — web chat interface (claude.ai)

## Summary
Claude was used to convert a static single-page portfolio design into a
data-driven site, where all content (name, bio, projects, skills,
coursework, contact links) lives in a single JavaScript object inside
`index.html` and is rendered into the page on load. This makes the site
easy to extend as new projects, coursework, and achievements are added
over the next semesters — only that data object needs editing.

## Prompt history (chronological)

1. Shared an earlier Claude conversation containing the original static
   portfolio HTML/CSS design.
2. "I want the html file dynamic and retrieve all necessary info from it"
3. "fetch other info from the chat"
4. "can u do it for me" (requesting the JS object be extracted into an
   external `data.json` file, fetched at runtime)
5. Request for guidance on assembling the full assignment deliverables
   (GitHub repo, GitHub Pages deployment, AI disclosure).
6. Step-by-step walkthrough of creating the repo and uploading files,
   requested one step at a time.
7. "index.html not working" — debugging a 404 on `data.json` after upload.
8. "just make it runnable from anywhere" — request to remove the external
   `data.json` dependency entirely and embed all content directly inside
   `index.html`.
9. "have u checked references I gave u" — asked Claude to review the
   assignment's example portfolios (Chris Olah, Andrej Karpathy, Gazi
   Jarin) and compare against the current design.
10. "Idk about anything on portfolio, I am leaving it to u" — requested
    Claude use its judgment to finalize remaining content, resulting in
    the addition of a "Notes & writing" section.
11. "colour looks almost same, have any better color ideas" — requested
    a distinct color palette; Claude proposed and applied a warm
    amber/terracotta accent on a warm charcoal background, replacing the
    original violet/cool-blue theme.
12. "what's your opinion as I have 0 knowledge" / "how good is it
    comparing with most wanted portfolios" — requested Claude's honest
    assessment of the design relative to reference portfolios.
13. "do it but don't stray away from the deliverables..." — requested
    small polish upgrades (scroll progress bar, active nav highlighting,
    hover glow on project cards) within existing scope.
14. "Iut is in Dhaka divison but gazipur district" — corrected a factual
    detail; Claude updated the Academic section to read "Gazipur, Dhaka
    Division, Bangladesh."
15. Follow-up guidance on pushing files to GitHub and enabling GitHub
    Pages, given one step at a time.

## What Claude produced
- Refactored the static `index.html` into a template that renders all
  sections (hero, about, projects, skills, academic, notes, contact,
  footer) from a single JavaScript render layer, driven by one data
  object (`SITE_DATA`) embedded directly in the file.
- Reviewed reference portfolios (colah.github.io, karpathy.ai,
  gazijarin.com) and proposed adding a "Notes & writing" section.
- Authored placeholder content for the Notes section based on existing
  project details already present on the site.
- Proposed and implemented a distinct warm amber/terracotta color theme
  in place of the original violet/blue theme.
- Added minor UI polish: scroll progress indicator, active-section nav
  highlighting, hover glow on project cards.
- Provided step-by-step instructions for creating the GitHub repository,
  uploading files, and enabling GitHub Pages.
- Drafted this disclosure document and the project README.

## What was done manually / by the author
- Original visual design direction (typography, layout, section
  structure) and all factual content (name, project descriptions,
  coursework, skills, contact details).
- Creating the actual GitHub repository, uploading files, and enabling
  GitHub Pages in repo settings.
- Correcting factual details (e.g. IUT's district/division).
- Ongoing edits to `SITE_DATA` inside `index.html` as new projects,
  coursework, and notes are added in future semesters.
- Should personally review and rewrite the Notes section content before
  final submission, as it was drafted by Claude based on existing
  project descriptions rather than the author's own original writing.
