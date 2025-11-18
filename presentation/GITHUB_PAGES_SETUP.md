
# GitHub Pages Setup Guide

## Automated Deployment (GitHub Actions)

This repository now includes `.github/workflows/deploy-pages.yml`, which:

- Installs R + Pandoc on every push to `main`
- Runs `rmarkdown::render()` on `presentation/ai_eval_presentation.Rmd`
- Exports the result to `site/index.html`
- Publishes the rendered HTML to GitHub Pages using `actions/deploy-pages`

### Enable Pages

1. Push the workflow to GitHub.
2. In your repository, go to **Settings → Pages**.
3. Under **Build and deployment**, set **Source** to **GitHub Actions**.
4. After the first successful workflow run, GitHub shows the live URL (typically `https://<username>.github.io/<repo>/`).

> Tip: If your default branch is not `main`, update the workflow trigger in `.github/workflows/deploy-pages.yml`.

### What gets published?

All files in the generated `site/` directory are deployed. Currently that directory only contains `index.html`, which is completely self-contained:

- CSS rules (including `presentation/styles.css`) are embedded into the HTML output
- Images referenced in the slides are base64-encoded, so no additional assets are required

If you later add external assets (e.g., custom JS, images), copy them into the `site/` folder before the `upload-pages-artifact` step or adjust the workflow accordingly.

## Testing Locally

Before pushing, you can preview the rendered HTML:

```bash
cd presentations/taf-ai-eval-pre
Rscript -e "rmarkdown::render('presentation/ai_eval_presentation.Rmd', output_file = 'index.html')"
python3 -m http.server 8000
```

Then open `http://localhost:8000/presentation/index.html` (or whichever output path you used).

## Manual fallback (optional)

If you ever want to bypass GitHub Actions, you can still host manually:

1. Render locally to `presentation/ai_eval_presentation.html`.
2. Commit the HTML (or rename it to `index.html`) to the branch that GitHub Pages serves.
3. Point GitHub Pages to that branch/folder in **Settings → Pages**.

Because the presentation HTML is self-contained, no extra assets are needed for manual hosting either.
