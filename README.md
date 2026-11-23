# Alex Henson: GIS Portfolio

Static HTML/CSS site for GitHub Pages. No build step.

## Files

- `index.html`: home page (name, portfolio title, About, project list, Contact)
- `projects.html`: the Projects page, one section per map with a description
- `style.css`: all styling for both pages
- `images/`: full-size maps, plus `thumbs/` for the home page list and the hero crop
- `fonts/`: Archivo and Source Serif 4, self-hosted (SIL Open Font License, see the .txt files)

## Still to fill in

Text highlighted in yellow on the site is placeholder. Search `index.html` for
`mark class="todo"` to find it all:

- Year and major, your goal after graduation, and any other GIS tools (Python, R)
- Your email address
- Your headshot: save it as `images/headshot.jpg` and follow the comment in the About section

The three project descriptions in `projects.html` are drafts. Edit them so they say what
you actually did, and add the data source for the two Portland maps (there are comments
marking where).

## Replacing a map with a higher-resolution export

The assignment asks for exports at 150 dpi or higher. Export from ArcGIS Pro
(Share > Export Layout), save the file over the old one with the same name, then update the
pixel size shown next to "Open image" on `projects.html`. The page sizes the map for you.

## Adding another map

1. Put the image in `images/` (lowercase file name, no spaces).
2. In `projects.html`, copy one `<article>` block, then change the `id`, title, image
   path, `width`/`height`, description, and facts.
3. Add a matching row to the Projects list in `index.html`, with a thumbnail about
   480 px wide in `images/thumbs/`.

## Previewing locally

```
python3 -m http.server 8000
```

Then open http://localhost:8000.
