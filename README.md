# Priyabrata Das Academic Portfolio

A free, static academic portfolio built with HTML5, CSS3, and vanilla JavaScript. It has no build step, backend, database, API keys, analytics, or paid services, and is designed for GitHub Pages.

## Files

```
index.html  about.html  research.html  experience.html  publications.html
skills.html  cv.html  contact.html  404.html
styles.css  script.js  data.js  favicon.svg  robots.txt  sitemap.xml
assets/images/  assets/documents/
```

## Edit content

Open `data.js` in any text editor. It is the single source for profile text, biography, research interests, projects, experience, publications, skills, achievements, social links, image paths, CV path, and featured items. Move project objects to reorder them; set `featured: true` to show one on Home; set `visible: false` to hide unfinished content. Add publications to the applicable category and keep their status accurate. Add a social URL only when it is verified; blank links remain hidden.

Update the biography in `profile.bio`, the availability statement in `profile.availability`, and the palette only in the CSS variables at the top of `styles.css`. To modify navigation or add a page, copy an existing page, add its navigation link consistently, and add it to `sitemap.xml`.

## Images and CV

Add a square/portrait profile photograph (at least 800 × 800 px) as `assets/images/profile.jpg`. Project images should be approximately 1600 × 900 px and use the filenames in `data.js`. JPG or WebP is suitable for photographs; PNG or SVG is suitable for figures. Compress files before uploading. Do not upload confidential, unpublished, or unapproved data. Missing images intentionally show accessible placeholders.

Add your verified CV as `assets/documents/Priyabrata_Das_CV.pdf`. The CV page will then show its viewer. If it remains missing, a clear fallback appears instead.

## Preview and check links

Double-click `index.html` for a basic preview. For a better local preview in VS Code, install the free Live Server extension, right-click `index.html`, and choose **Open with Live Server**. Check every navigation item and use the browser’s developer tools to confirm any new paths. GitHub Pages serves files from the root, so retain the filenames and relative paths.

## Publish on GitHub Pages

First create an empty **public** GitHub repository named exactly `PriyabrataDas1.github.io`. Then, in this folder, run:

```bash
git init
git add .
git commit -m "Create academic portfolio website"
git branch -M main
git remote add origin https://github.com/PriyabrataDas1/PriyabrataDas1.github.io.git
git push -u origin main
```

Open the repository → **Settings** → **Pages**. Under **Build and deployment**, choose **Deploy from a branch**, select branch `main`, folder `/ (root)`, and save. A repository named `PriyabrataDas1.github.io` may publish automatically depending on GitHub’s current interface. The intended URL is `https://priyabratadas1.github.io`.

For later updates, edit files, run `git add .`, commit with a clear message, and push again. A custom domain is optional and can cost money; GitHub Pages itself does not require a paid service. Keep publication status, affiliations, figures, and research claims accurate; remove or hide anything not ready for public sharing.

## Troubleshooting

- Missing image: confirm spelling/case and that the file is inside `assets/images/`.
- Missing CV: confirm the PDF filename and location match `data.js`.
- GitHub Pages issue: ensure the repository is public, Pages uses `main` and `/ (root)`, and wait briefly after pushing.
