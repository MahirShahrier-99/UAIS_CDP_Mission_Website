# Uganda Climate Data Platform (CDP) — Mission Website

A single-page site documenting the Dream71 Technical Scoping, Co-Design and Stakeholder
Engagement Mission for the Uganda Climate Data Platform, 23–28 August 2026
(Financial Resilience in Agriculture initiative, UNDP Uganda).

Plain HTML, CSS and JavaScript — no build step, no framework, nothing to install.

## Files

```
index.html        the whole site (one page, sections linked by the nav)
css/style.css      all styling
js/main.js         mobile menu, photo lightbox, active-link highlighting
images/            all 44 photos used on the site
```

## Preview it on your computer

Just open `index.html` in a browser — double-click the file, or drag it into a browser
window. Everything is a relative path, so nothing else is needed.

## Deploy it to GitHub Pages

1. Create a new **public** repository on GitHub (e.g. `uais-cdp-mission`).
2. Upload everything in this folder to the repository, keeping the same structure
   (`index.html` at the root, alongside the `css`, `js` and `images` folders).
   - Easiest way: on the repo page, click **Add file → Upload files**, then drag in
     `index.html`, the `css` folder, the `js` folder and the `images` folder together.
   - Or, if you use git from a terminal:
     ```
     git init
     git add .
     git commit -m "Add mission website"
     git branch -M main
     git remote add origin https://github.com/<your-username>/uais-cdp-mission.git
     git push -u origin main
     ```
3. In the repository, go to **Settings → Pages**.
4. Under **Build and deployment → Source**, choose **Deploy from a branch**.
5. Under **Branch**, choose `main` and folder `/ (root)`, then **Save**.
6. GitHub takes a minute or two to publish. Your site will then be live at:
   `https://<your-username>.github.io/<repository-name>/`

Any time you want to change text or swap a photo, edit the file directly on GitHub
(pencil icon on the file page) or push a new commit — the live site updates automatically
within a minute of the push.

## Updating content

- **Text and captions**: edit the relevant section in `index.html` directly.
- **Photos**: add a new file to `images/`, then update the matching `src` and
  `data-src` attributes in `index.html` to point to it.
- **Colors**: the Ivory / Sage / Dusty Rose / Sandstone / Dusty Blue palette is defined
  once at the top of `css/style.css` under `:root` — change the values there and the
  whole site updates.

## Credits

Prepared by Mahir Shahrier, Environmental Specialist and Civil Engineer, mahirshahrier.com,
for the UNDP Uganda Financial Resilience in Agriculture (FRA) Initiative.
