# martinzhang03.github.io

Personal academic homepage of Jinyuan (Martin) Zhang, built with the [al-folio](https://github.com/alshedivat/al-folio) Jekyll template and deployed to GitHub Pages.

Live site: https://martinzhang03.github.io

## Common edits

| What | File |
|---|---|
| Add or edit a paper | `_bibliography/papers.bib` (a copy-paste template with all link fields is at the top of the file) |
| Bio on the home page | `_pages/about.md` |
| CV page | `_pages/cv.md` |
| Email / GitHub / Scholar / LinkedIn icons | `_data/socials.yml` |
| Profile photo | `assets/img/prof_pic.jpg` |

Every push to `main` rebuilds and redeploys the site through `.github/workflows/deploy.yml` (about 4 minutes). You can edit files directly on github.com; committing there triggers the same rebuild.
