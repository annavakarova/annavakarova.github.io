# Anna Vakarova — academic website

A Quarto website deployed with GitHub Actions to GitHub Pages.

## Before publishing
1. Replace `YOUR-USERNAME` in `_quarto.yml` with your GitHub username (or adjust `site-url` if you use a different repository name).
2. Replace `YOUR-EMAIL@example.com` in `index.qmd` with your professional email address.
3. Put your headshot at `images/profile.jpg` and change `images/profile-placeholder.svg` in `index.qmd` to `images/profile.jpg`.
4. Add your CV as `files/cv.pdf` and your papers to `files/`; update links in `research.qmd`.
5. Verify and update the job-market paper title, description, and teaching dates.

## Preview locally (optional)
Install Quarto from https://quarto.org/docs/get-started/ and run:

```bash
quarto preview
```

## Publish on GitHub Pages
1. Create a new PUBLIC GitHub repository named `annavakarova` (or another name).
2. Upload the contents of this folder to the root of the repository, including `.github/workflows/publish.yml`. The `.github` directory may be hidden in some file browsers; ensure it is included.
3. In GitHub repository **Settings → Pages → Build and deployment**, select **GitHub Actions** as the source.
4. Commit to the `main` branch. Under **Actions**, watch the `Publish Quarto website` workflow. Once it succeeds, visit `https://YOUR-USERNAME.github.io/annavakarova/`.
5. To use a custom domain later, configure it in **Settings → Pages → Custom domain**, add the DNS records requested by GitHub, enable HTTPS, and update `site-url` in `_quarto.yml` to your custom domain. If the custom domain is attached, update the deployment workflow/site paths as necessary.

Note: `files/cv.pdf` is not included yet. Add it before sharing the site publicly, or temporarily remove the CV links.
