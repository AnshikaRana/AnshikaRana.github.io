# PORTFOLIO

My portfolio. One page that reads sideways: projects, research, internships
and the degree, with a single line running underneath that changes shape as
the chapters change.

Live at <https://anshikarana.github.io/PORTFOLIO/>

## What is in here

```
index.html          the whole page: markup and all of the CSS
data.js             the content: projects, research, internships, courses, semesters
app.js              rendering and behaviour: the rail, the pop-ups, the signal line
assets/             images, all WebP; share-card.png is the link preview
resume.pdf          my CV (add this file; both resume links point at it)
favicon.svg         the mark in the browser tab
apple-touch-icon.png
404.html            a page in the same palette for anything that is not the portfolio
.nojekyll           tells GitHub Pages to serve the files as they are
robots.txt, sitemap.xml
```

Nothing is built or compiled. The three files at the top are the source, and
they are also what is served. Editing `data.js` is enough to change almost all
of the content.

## Changing the content

| What | Where |
|---|---|
| A project, research entry or internship | the `PROJECTS`, `RESEARCH`, `INTERNSHIPS` objects in `data.js` |
| A course or a semester | the `COURSES` and `SEMS` objects in `data.js` |
| Name, opening paragraph, contact links | `index.html` |
| Colours, type, spacing | the `:root` block at the top of `index.html` |

Images live in `assets/` and are referenced from `data.js` by filename.

## Running it locally

Opening `index.html` by double-clicking works for most of the page. To see it
exactly as it is served:

```bash
python3 -m http.server 8000
```

then visit <http://localhost:8000>.
