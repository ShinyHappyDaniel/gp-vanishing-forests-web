# Vanishing Forests (Part 2) – web edition

Long-form web edition of the Greenpeace Nordic report *Vanishing Forests (Part 2): How Ikea drives destruction in the Boreal Forests – a Swedish case study* (October 2026).

- `index.html` – the whole report as one page (no build step, no dependencies). Chapter navigation (left rail / drawer), reading progress, client-side search (`/` opens it), footnotes as pop-ups with a full reference list (Appendix II) and back-links, light/dark theme, responsive down to phone width.
- `img/` – pictures in two sizes (800 and 1600 px wide) plus the flowchart and the printed cover.
- `GP_Vanishing_Forests_Part2.pdf` – the printed report (12 MB), linked from the PDF buttons.
- `fonts/` – Greenpeace Sans Bold and Work Sans (variable). Licensed to Greenpeace; do not redistribute outside this project.

Serve the folder with any static host (GitHub Pages works as is). Content is generated from the report manuscript; edit the text in `index.html` directly or regenerate from the layout pipeline.

Design: Shiny Happy People.

## Publishing on GitHub Pages

1. Create a **private** repository on github.com (the fonts are licensed to Greenpeace – keep the repo private, or replace `fonts/` before making it public).
2. Put the contents of this folder at the repository root (so `index.html` is at the top level) and push.
3. Settings → Pages → Build and deployment: Source "Deploy from a branch", branch `main`, folder `/ (root)`. GitHub Pages works on private repositories on paid plans; on a free plan the repository must be public.
4. The site appears at `https://<user>.github.io/<repo>/` within a minute or two. A `.nojekyll` file is included so nothing is pre-processed.

Note for Claude Code: this is a static site – no build step, no framework. Just commit the folder as is and enable Pages.
