# Dinithi Jayasuriya — Personal Website

A single-file, dependency-free portfolio site. Just `index.html` plus your résumé PDF.

## Preview locally
Open the file in any browser:
```
xdg-open index.html      # Linux
```
Or run a tiny local server (better, so the PDF download works the same as in production):
```
cd portfolio
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Files
- `index.html` — the whole website (HTML + CSS + JS inline)
- `Dinithi_Jayasuriya_Resume.pdf` — linked by the "Download résumé" button

## Deploy free on GitHub Pages
1. Create a repo named **`<your-username>.github.io`** (e.g. `dinithi-j.github.io`).
2. Push these two files to it:
   ```
   git init
   git add index.html Dinithi_Jayasuriya_Resume.pdf
   git commit -m "Add personal website"
   git branch -M main
   git remote add origin https://github.com/<your-username>/<your-username>.github.io.git
   git push -u origin main
   ```
3. In the repo: **Settings → Pages → Source: `main` / root** → Save.
4. Your site goes live at `https://<your-username>.github.io` within a minute or two.

> Prefer drag-and-drop? Go to https://app.netlify.com/drop and drop the `portfolio` folder — you get a live URL instantly, and can add a custom domain later.

## Before you publish — things to update
These are placeholders I couldn't confirm from the résumé:
- **Google Scholar link** — replace `https://scholar.google.com/` (2 spots) with your real profile URL.
- **LinkedIn** — confirm `https://www.linkedin.com/in/dinithi-jayasuriya` is correct.
- **arXiv link** — confirm `arxiv.org/abs/2604.18834` resolves once the paper is posted.
- **GitHub** — your résumé shows a GitHub icon; add the URL if you want a GitHub button.
- **"Open to roles" banner** — edit the text in the hero (`.eyebrow`) to match your timeline.
- **Photo** — optional; I left it text-only for a clean academic/tech look. Easy to add.

Everything else (stats, publications, experience, projects) is pulled straight from your April résumé.
