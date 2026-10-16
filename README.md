# Intelligent MRI Image Analysis and Automated Report Generation System

Project web page for the CMPE 491 / 492 Senior Design Project at TED University.
Plain HTML and CSS, no build step.

## Files

```
index.html        page content
style.css         styles
assets/           favicon
reports/          published reports (PDF)
vercel.json       Vercel settings
```

## Publishing a new report

1. Put the PDF in `reports/`, e.g. `reports/D2-Project-Specifications.pdf`.
2. In `index.html`, find the row for that deliverable and replace
   `<span class="pending">Not yet published</span>` with
   `<a class="doc" href="reports/D2-Project-Specifications.pdf">Download PDF</a>`.
3. Commit and push. Vercel or GitHub Pages redeploys automatically.

## Deploy on Vercel

1. Push this folder to a GitHub repository.
2. On vercel.com, choose **Add New → Project** and import the repository.
3. Framework preset: **Other**. Leave build command and output directory empty.
4. Deploy. The URL looks like `https://<project-name>.vercel.app`.

## Deploy on GitHub Pages (alternative)

1. Push this folder to a GitHub repository.
2. Repository **Settings → Pages → Source: Deploy from a branch**, branch `main`, folder `/ (root)`.
3. The site appears at `https://<username>.github.io/<repository>/`.
