# MIND method: interactive figures

Interactive figures for the de-identification, structuring and paraphrasing method for the MIND psychotherapy corpus (BIU and QMUL, CLPsych 2027).

**Live page:** `https://<your-user>.github.io/<repo-name>/` (after enabling GitHub Pages, see below)

## What is in the page

| Tab | Shows |
|---|---|
| Overview | The three parts and release, with every Agent and human role |
| Full worked example | Patient P17 followed through all 13 steps |
| De-identification | Identify → Tag → Rewrite → Verify → Sign off, with the change log |
| Sequence | State → therapist response → state, and dependency links confirmed at Checkpoint B |
| Over time | Tracks keyed to entity IDs across sessions 3, 7 and 9 |
| Paraphrasing | Paraphrasing Agent, automatic checks, BIU review, withheld turns |
| Try the change log | A small tool that applies rewriter decisions to one turn and runs basic checks |

## Files

```
index.html   the whole page (HTML, CSS and JavaScript in one file)
.nojekyll    tells GitHub Pages to serve the file as is
README.md    this file
```

There is no build step and no dependency to install. The only external resource is Google Fonts; if it is blocked, the page falls back to system fonts.

## Publish on GitHub Pages

1. Create a repository (private is recommended, see the data note below) and push these files to the `main` branch:
   ```bash
   git init
   git add .
   git commit -m "Add MIND method interactive figures"
   git branch -M main
   git remote add origin https://github.com/<your-user>/<repo-name>.git
   git push -u origin main
   ```
2. In the repository, open **Settings → Pages**.
3. Under **Build and deployment**, set **Source** to *Deploy from a branch*, choose `main` and `/ (root)`, and save.
4. After a minute the page is live at `https://<your-user>.github.io/<repo-name>/`.

Pages on private repositories need a paid GitHub plan (Pro, Team or Enterprise). On Enterprise you can also restrict the site to organisation members.

To view it locally, open `index.html` in a browser.

## Data note

The page contains short excerpts of client speech from session AA6090_9 (spans E1–E7) and illustrative turns treated as P17-S3. Check with the project leads and the BIU data agreement before making the repository or the site public. The change-log tool runs entirely in the browser; drafts are kept in the browser's local storage and nothing is sent anywhere.

## Illustrative content

The E4 reviewer correction and the P17 evaluation numbers in the worked example are illustrations, not pilot results. Replace them once the pilot has been run.
