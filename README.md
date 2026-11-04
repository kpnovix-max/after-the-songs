# After the Songs — By KP

Companion reading site to *Before the Songs*. The original cover fonts, styles, reader controls and GitHub Pages workflow are retained.

## Publish on GitHub (first time)

1. Create a **public** repository named `after-the-songs` under the `kpnovix-max` account. Do **not** initialize it with a README, licence, or `.gitignore`.
2. Unzip the downloaded package on your computer. **Upload the contents of the `after-the-songs` folder, not the enclosing folder or ZIP**, into the root of your new GitHub repository. The root must show `package.json`, `assets/`, `scripts/`, `manuscript/`, and `.github/`.
3. GitHub web upload sometimes skips hidden `.github` folders. Verify that `.github/workflows/pages.yml` exists. If missing, use GitHub's **Add file → Create new file**, enter `.github/workflows/pages.yml`, and paste the workflow file from this package.
4. Go to **Settings → Pages → Build and deployment → Source** and select **GitHub Actions**.
5. Go to **Actions** and wait for **Publish After the Songs** to complete. If needed, open that workflow and select **Run workflow**.
6. Open `https://kpnovix-max.github.io/after-the-songs/`. Initial deployment may take a few minutes.

## Update a chapter later

Add a new Markdown file in `manuscript/` with a two-digit prefix (`02-...md`, etc.) and the first two headings `# Chapter Two` and `## The Other Shore`. Commit the file. The build automatically publishes it and unlocks its index link.

**Important:** The website rebuilds from `scripts/build.mjs` and `manuscript/`; do not edit `dist/` as a lasting change.

**Chapter 1 is locked.** Chapter 2 onwards should portray the girl's quietness in contrast to her talkative childhood with her father.
