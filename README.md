# After the Songs — By KP

GitHub Pages website for **After the Songs**, with Chapters 1–5 published and Chapters 6–10 shown as forthcoming.

## Update existing repository

Repository: https://github.com/kpnovix-max/after-the-songs

1. Extract this ZIP. The extracted folder contains `assets/`, `scripts/`, `manuscript/`, `dist/`, `.github/`, `package.json`, and this README.
2. In your existing repository on GitHub, choose **Add file → Upload files**. Upload **the contents of the extracted folder** to the **repository root**, not into a new folder. Include all subfolders and their contents.
3. Commit to `main`. Existing files with matching paths must be replaced. If the GitHub uploader says it cannot replace files, edit/update the matching files instead; do not create duplicates.
4. Verify `.github/workflows/pages.yml` is present. Hidden dotfolders can be omitted by some file browsers. If it is already there and not updated, replace it with this package's workflow.
5. In **Settings → Pages**, verify **Build and deployment → GitHub Actions** is selected. The workflow **Publish After the Songs** should run on the `main` commit.
6. Visit https://kpnovix-max.github.io/after-the-songs/ and check that Chapter 5 opens and Chapters 6–10 say 'Forthcoming'.

The pre-built `dist/` folder is included, so it can also be deployed as static content; however, the configured GitHub Actions workflow generates `dist/` from Markdown on every commit.

**Publishing note:** The published site will change only when you commit the files into your repository and a Pages deployment succeeds; this ZIP itself does not alter GitHub.

## Contents

- `manuscript/`: Five continuity-corrected chapters. Chapter 1 unchanged.
- `scripts/build.mjs`: Generates the reader and navigation links from available chapters.
- `assets/`: Existing light/dark theme, typography and reader tools.
- `.github/workflows/pages.yml`: Automatic GitHub Pages deployment on push to `main`.
- `dist/`: Fully built and checked static website for chapters 1–5.

## Future chapters

Add chapter files named `06-...md`, `07-...md`, etc., to `manuscript/` and commit. A fresh deployment updates the index and navigation automatically.
