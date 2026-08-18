# Web design demos

Concept websites built for local Tulsa-metro businesses that don't currently have a real website, used as cold-outreach pitch material.

Live site (once GitHub Pages is enabled): `https://<your-github-username>.github.io/web-design-demos/`

## Structure

Each business gets its own folder containing a self-contained `index.html` (all CSS/JS inline, no build step). The root `index.html` is a simple landing page linking to each one.

```
web-design-demos/
  index.html              <- landing page listing all demos
  crescent-cafe/
    index.html             <- live at /crescent-cafe/
  <next-business-slug>/
    index.html             <- live at /<next-business-slug>/
```

## Adding a new demo

1. Create a new folder using a lowercase, hyphenated slug of the business name, e.g. `silver-skillet/`.
2. Drop a self-contained `index.html` inside it.
3. Add a link to it in the root `index.html`'s list.
4. Commit and push — GitHub Pages redeploys automatically.

## Hosting on GitHub Pages

1. Push this repo to GitHub (see steps below).
2. In the repo on GitHub: **Settings -> Pages**.
3. Under **Build and deployment -> Source**, choose **Deploy from a branch**.
4. Branch: `main`, folder: `/ (root)`. Save.
5. GitHub gives you a URL like `https://<username>.github.io/web-design-demos/` within a minute or two.
6. Each demo is then reachable at `.../web-design-demos/crescent-cafe/`.

## Pushing this repo to GitHub for the first time

From this folder:

```bash
git add -A
git commit -m "Add Crescent Cafe demo"
git branch -M main
git remote add origin https://github.com/<your-username>/web-design-demos.git
git push -u origin main
```

(Create the empty repo on GitHub first at github.com/new, named `web-design-demos`, before running the commands above.)
