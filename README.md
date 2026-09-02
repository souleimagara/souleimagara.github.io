# Portfolio — Souleima Gara

A single static page. No build step, no dependencies, no server needed.

```
index.html                  the whole site (CSS and JS are inline)
assets/img/                 project screenshots + portrait
assets/Souleima-Gara-CV.pdf linked from the "Download CV" button
```

## Look at it locally

Double-click `index.html`.

## Put it online (any one of these)

**Netlify Drop** — go to app.netlify.com/drop and drag this whole folder onto the page.
Free, instant, gives you a URL you can rename.

**GitHub Pages** — create a repo, push this folder, then Settings → Pages → deploy from
`main` / root.

**Vercel** — `vercel` in this folder, or drag the folder into the dashboard.

Any of them will serve it as-is. A custom domain can be pointed at it later.

## Changing things

Text and colours live at the top of `index.html`:

- Colours: the `:root { … }` block near the top. `--pink`, `--teal`, `--amber` and
  `--violet` drive everything; each employer section picks one (`.era--pink` etc.), and the
  matching `--pink-soft` values are the tinted backgrounds. There is a separate dark-mode
  block below it, so change both.
- Content: search for the project title you want to edit.

To add screenshots for a project that has none (all the ZBD work), drop the images into
`assets/img/` and add them to that project's `images` list. The regenerator lives in
`../portfolio-source/build.py`.

Screenshots of client work belong to those clients; the ZBD projects are deliberately
described in words rather than shown, since that product's internals are not public.
