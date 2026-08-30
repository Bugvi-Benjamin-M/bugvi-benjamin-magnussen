# Búgvi Benjamin Magnussen — personal site

A single-page, minimal/modern site with a dark-mode-first design (toggle in the
header, remembers your choice). One profile, several facets: About,
Experience, Research & Publications, Music, and Contact — Music lives on the
same page as everything else rather than a separate site, so it reads as part
of the same person rather than a bolt-on.

No build step, no dependencies — just `index.html`, `styles.css`, and
`script.js`.

## What still needs your input

Everything below is a placeholder (marked in *italics* on the page or with
`#`/`example.com` links in the HTML) until you swap it in:

- **Tagline** (`index.html`, `.tagline`) — currently "Data scientist &
  researcher. Trained musician." as a starting suggestion. Change any time.
- **Hero one-liner** and **About bio** — currently placeholder text.
- **Experience timeline** — three placeholder entries; add/remove
  `<li class="timeline-item">` blocks in the `#experience` section as needed.
- **Education** — three placeholder entries (you mentioned multiple degrees);
  add/remove `<li class="edu-item">` blocks in the `#education` section with
  real degree, field, institution, and years.
- **Publications** — two placeholder entries; add/remove `<article class="pub">`
  blocks in `#research` with real titles, venues, years, links, and abstracts.
- **Music section** — intro text, plus three placeholder photos expected at
  `images/music/performance-1.jpg`, `-2.jpg`, `-3.jpg` (missing ones just
  disappear rather than showing broken images), and a "Listen" link.
- **Contact links** — currently `you@example.com`, `linkedin.com/in/your-handle`,
  a Scholar placeholder, and `github.com/your-handle`. Update the `href`s.

## Profile photo

The hero shows a full-body photo (cropped from the studio shot in
`resources/`) rather than a small headshot. Two versions swap automatically
with the color theme:

- `profile-bw.jpg` — shown in dark mode
- `profile-color.jpg` — shown in light mode

Both are 520px-wide crops trimmed to remove empty studio background; the
originals (`resources/bw.jpg`, `resources/color.jpg`) are full-resolution and
not referenced by the page. To change the crop, re-crop from the originals
and overwrite the two files above — same filenames, same aspect ratio ideally,
since `.avatar` uses `object-fit: cover`.

## Styling

- Accent color: `--color-accent` / `--color-accent-hover` in `styles.css`
  (separate values are set for dark and light mode).
- Fonts: Fraunces (headings) + Inter (body), loaded from Google Fonts —
  swap the `<link>` in `<head>` and the `--font-display` / `--font-body`
  variables together if you change them.

## Run locally

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```
