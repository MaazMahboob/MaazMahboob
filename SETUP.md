# Setup

## What changed from the last version

- Colors: muted warm charcoal, brass/amber and dusty teal, instead of the violet/cyan MAAZ.OS palette. No neon.
- Animation: the hero banner has small domain-words (vision, retrieval, signal, calibration, care, detection, focus) drifting slowly down the background, plus a soft breathing signal line and a bobbing arrow. All of it is time-based CSS, not hover-triggered — GitHub loads SVGs referenced in a README as static `<img>` sources, and `:hover` states inside an `<img>`-sourced SVG generally don't fire in any browser. Rather than ship a hover effect that would likely just sit there doing nothing once pushed, the interactive parts use native `<details>` / `<summary>` disclosure widgets instead (the "Research", "Projects" and "Experience" sections) — click to expand, and it's real, working interactivity.
- One SVG asset instead of six, and one external stats widget instead of two — fewer moving parts, calmer page.

## Before you push

Fill in the real contact line at the bottom of `README.md` — it currently has placeholder text (`you@example.com`, `linkedin.com/in/your-handle`).

## Push it (Windows cmd)

Assuming you extracted this delivery to `C:\Users\maazm\Downloads\MaazMahboob-profile-v3` and your repo is already cloned at `C:\Users\maazm\MaazMahboob`:

```cmd
cd C:\Users\maazm\MaazMahboob

xcopy /E /I /Y "C:\Users\maazm\Downloads\MaazMahboob-profile-v3\assets" "assets"
xcopy /E /I /Y "C:\Users\maazm\Downloads\MaazMahboob-profile-v3\.github" ".github"
copy /Y "C:\Users\maazm\Downloads\MaazMahboob-profile-v3\README.md" "README.md"
copy /Y "C:\Users\maazm\Downloads\MaazMahboob-profile-v3\SETUP.md" "SETUP.md"

dir
dir assets

git add .
git commit -m "v3: calm palette, ambient hero animation, click-to-expand sections"
git push origin main
```

`xcopy /E /I /Y` copies whole folders including subfolders, which is what `assets` and `.github` need. `dir` and `dir assets` are there so you can eyeball that the files actually landed before you `git add .` — that's the step that silently failed last time.

## About the contribution snake

The workflow in `.github/workflows/snake.yml` needs to run once before the image in the README will show anything. After you push:

1. Go to the repo's **Actions** tab.
2. Select **Generate contribution snake** on the left.
3. Click **Run workflow** to trigger it manually the first time (it also runs automatically every night after that).
4. Once it finishes, it creates (or updates) an `output` branch with the SVG the README points to. Refresh your profile page — it can take a minute for GitHub's cache to catch up.

## Verifying it rendered

Open `https://github.com/MaazMahboob` in a browser (not the repo page — your profile page). Hard-refresh with `Ctrl+Shift+R` if it looks stale.
