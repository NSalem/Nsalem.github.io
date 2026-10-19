# Nahuel Salem-Garcia — personal site

Static researcher homepage for GitHub Pages.

**Live URL (once deployed):** https://Nsalem.github.io

## Contents

- `index.html` — About, Publications, CV
- `styles.css` — layout and visual styles
- `assets/` — place your photo and CV here

## Add your photo and CV

1. Save a portrait as `assets/photo.jpg` (JPEG or replace the `src` in `index.html` if you use PNG/WebP).
2. Save your CV as `assets/cv.pdf`.

The photo area shows a placeholder until the image file exists. The CV section already links to `assets/cv.pdf`.

## Edit content

- Bio and links: `#about` and the hero block in `index.html`
- Publications: `#publications` list in `index.html`
- Colors/type: CSS variables at the top of `styles.css`

## Preview locally

Open `index.html` in a browser, or from this folder:

```bash
python3 -m http.server 8000
```

Then visit http://localhost:8000

## Deploy to GitHub Pages

1. Create a **public** GitHub repository named exactly `Nsalem.github.io` under the `Nsalem` account (if it does not exist yet).
2. From this folder, initialize git (if needed), commit, and push:

```bash
cd /home/nahuel/projects/Nsalem.github.io
git init
git branch -M main
git remote add origin https://github.com/Nsalem/Nsalem.github.io.git
git add .
git commit -m "Add personal researcher site"
git push -u origin main
```

3. On GitHub: **Settings → Pages → Build and deployment**
   - Source: **Deploy from a branch**
   - Branch: `main` / folder `/ (root)`
4. After a minute or two, open https://Nsalem.github.io

Optional: use `gh repo create Nsalem.github.io --public --source=. --remote=origin --push` if the [GitHub CLI](https://cli.github.com/) is installed and authenticated.
