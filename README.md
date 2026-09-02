# tavantzish.github.io

Personal academic website of **Theocharis Tavantzis** — PhD Fellow, Department of
Computer Science, Aalborg University.

Live at <https://tavantzish.github.io>

## Structure

```
index.html                 all content lives here
style.css                  design tokens at the top of the file
assets/photo.jpg           portrait (720×720)
assets/CV_..._.pdf         downloadable CV
.nojekyll                  tells GitHub Pages to serve the files as-is
```

## Editing

**Add a publication** — copy an existing `<li>` inside `<ol class="pubs">` in
`index.html`, change the year, title, authors, venue and DOI. Newest first.

**Add a committee** — copy an `<li>` inside the relevant `<ul class="service">`.

**Update the CV** — replace `assets/CV_Theocharis_Tavantzis.pdf` (keep the
filename) and update the timeline entries in the `#cv` section.

**Change the colour** — edit `--accent`, `--accent-ink` and `--accent-soft` in
the `:root` block of `style.css`. The `@media (prefers-color-scheme: dark)`
block below it holds the dark-mode equivalents.

## Publishing

```bash
git add -A && git commit -m "Update site" && git push
```

GitHub Pages redeploys in under a minute.
