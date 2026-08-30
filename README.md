# Búgvi Benjamin Magnussen — personal site

Single-page site: About, Experience, Education, Research, Music, Contact.
Dark/light toggle in the header (remembers your choice). No build step —
just `index.html`, `styles.css`, `script.js`.

## Run locally

```bash
python3 -m http.server 8000
```

## TODO

- Experience: "Software Engineer" entry needs organization + years
- Education: fill in real degrees (placeholders currently)
- Publications: fill in real papers (placeholders currently)
- Music: intro text, photos (`images/music/performance-1.jpg` etc.), listen link

## Notes

- `profile-bw.jpg` / `profile-color.jpg` (repo root) are the cropped, web-sized
  photos shown in dark/light mode. Full-res originals are in `resources/`.
- Accent color and fonts (Fraunces + Inter) are set via CSS variables at the
  top of `styles.css`.
