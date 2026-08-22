# Setup

I don't have push access to your GitHub account, so here's how to ship this.

## 1. Push the files

```bash
git clone https://github.com/MaazMahboob/MaazMahboob.git
cd MaazMahboob
# copy README.md, assets/, .github/ from this delivery into the repo root
git add .
git commit -m "Rebuild profile as MAAZ.OS system"
git push origin main
```

## 2. Let the snake workflow run once

Go to **Actions → Generate Snake Contribution Animation → Run workflow** (or just wait for the next push).
It creates an `output` branch with `snake-dark.svg` / `snake-light.svg`, which the README already links to.
Nothing breaks before that — the images will just 404 silently in most renderers until the first run completes.

## 3. Sanity-check the stats service

`github-readme-stats.vercel.app` is the standard self-hostable stats widget and generally reliable, but if it's
ever down or rate-limited for you, either wait it out or deploy your own instance (the project's README covers
this) and swap the URL in the README's Activity section.

## 4. What was verified vs. left out

Everything in the README is backed by your resume, memory context, or the flagship repo's actual file tree
(`ChestXrayApp/`, `BalancedChestXray/`, `data.yaml`, training/app notebooks — confirmed by inspecting the repo
directly). No metrics, benchmark numbers, or claims were invented. If you later have hard numbers you're
confident defending in an interview (mAP, precision/recall, dataset size), those are worth adding to the
flagship section — right now it deliberately describes *what the system does* rather than inventing performance
numbers that weren't in the source material.

## 5. Note on citations

I don't have live access to verify how Google Scholar / arXiv / Springer currently list your papers — if you
want direct links added next to each entry in the Research Core table, send them over and I'll wire them in.
