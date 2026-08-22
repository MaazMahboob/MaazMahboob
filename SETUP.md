# Setup — v2

Same drill as before, just with the corrected/upgraded files. Copy everything from this
folder into your local `MaazMahboob` repo clone, replacing the old versions:

```cmd
cd C:\Users\maazm\MaazMahboob

xcopy /E /I /Y "C:\path\to\this\folder\assets" "assets"
xcopy /E /I /Y "C:\path\to\this\folder\.github" ".github"
copy /Y "C:\path\to\this\folder\README.md" "README.md"
copy /Y "C:\path\to\this\folder\SETUP.md" "SETUP.md"

git add .
git commit -m "v2: fix hallucinated CTGAN attribution, equal-weight CV/RAG, real metrics, premium visual pass"
git push origin main
```

## What changed from v1

- **Fixed hallucination**: CTGAN was incorrectly attributed to the chest X-ray flagship project.
  It's actually from the GNCIPL stroke-risk project — now correctly placed there, with the
  synthetic-to-real generalization gap called out honestly (that's a credibility signal, not
  a weakness to hide).
- **LLM/RAG work promoted to equal billing** with the computer vision system — both shown as
  full-width flagship cards side by side, both with real benchmark numbers (83.7% win rate on
  TimeQA v2, 78.0% on MMLU Global Facts).
- **AI Engineering & Deployment added as its own category** — FastAPI, Pydantic, JWT/OAuth2,
  PostgreSQL, Alembic, Celery, Docker Compose. This was completely missing before and it's the
  part that signals "this person ships production systems," not just notebooks.
- **All research entries now have real titles, venues, and metrics** pulled directly from your
  resume, instead of vague one-line descriptions.
- **Visual pass**: layered glass-panel cards with real drop shadows, staggered fade/rise reveal
  timing on the hero instead of everything appearing at once, metric-chip badges, consistent
  gradient system, better typographic hierarchy.

## Still open

- If you have live links for the arXiv paper and IGI Global DOI, send them and I'll wire them
  into the README/SVG text directly instead of the placeholder "→ arxiv.org" / "→ DOI link" labels.
- The PubMedBERT paper is marked "Under Review" per your resume — update that the moment it's
  accepted, since publication status is one of the first things a technical reviewer checks.
