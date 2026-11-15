# PORTFOLIO

My portfolio. It turns sideways, one page at a time: an introduction, four
projects, four research threads, three internships and the degree, with a
single line running underneath that changes shape as the chapters change.

Live at <https://anshikarana.github.io/PORTFOLIO/>

## What is in here

```
index.html          the whole page: markup and all of the CSS
data.js             the content: projects, research, internships, courses
app.js              rendering and behaviour: page turning, pop-ups, the signal line
assets/             images, all WebP; share-card.png is the link preview
resume.pdf          my CV (both resume links point at it)
favicon.svg         the mark in the browser tab
apple-touch-icon.png
404.html            a page in the same palette for anything that is not the portfolio
.nojekyll           tells GitHub Pages to serve the files as they are
robots.txt, sitemap.xml
```

Nothing is built or compiled. Editing `data.js` is enough to change almost all
of the content.

## Changing the content

| What | Where |
|---|---|
| A project, research entry or internship | the `PROJECTS`, `RESEARCH`, `INTERNSHIPS` objects in `data.js` |
| A course's syllabus | the `COURSES` object in `data.js` |
| The course list of a semester | `SEMS` at the top of `app.js` |
| Name, introduction, contact links | `index.html` |
| Colours, type, spacing | the `:root` block at the top of `index.html` |

## Running it locally

```bash
python3 -m http.server 8000
```

then visit <http://localhost:8000>.
