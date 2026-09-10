# sleimanyara.github.io

Source for **https://sleimanyara.github.io**

Built with [Hugo Blox](https://hugoblox.com) (Academic CV theme). Every push to
`main` rebuilds and redeploys the site automatically via GitHub Actions. It goes
live about two minutes later. You do not need Hugo installed.

---

## How to update the site

### Option A — edit in the browser (no software needed)

1. Go to the file on GitHub, e.g.
   https://github.com/sleimanyara/sleimanyara.github.io/blob/main/content/authors/admin/_index.md
2. Click the pencil icon (top right)
3. Make your change
4. Click **Commit changes**

Wait ~2 minutes, then reload the site. Works from a phone.

### Option B — edit on your Mac

```bash
cd ~/Desktop/website
# edit files in content/
git add -A && git commit -m "update bio" && git push
```

### Check the deploy worked

https://github.com/sleimanyara/sleimanyara.github.io/actions — a green tick
means it's live. Red means the build failed and **the previous version stays
up**, so a mistake can't take the site down.

---

## Where things live

| What you want to change | File |
|---|---|
| Bio, photo, role, education, social links | `content/authors/admin/_index.md` |
| Homepage section order and layout | `content/_index.md` |
| Nav menu | `config/_default/menus.yaml` |
| Site title, URL | `config/_default/hugo.yaml` |
| Theme, colours, fonts | `config/_default/params.yaml` |
| Published papers | `content/publication/<name>/index.md` |
| Working papers | `content/wp/<name>/index.md` |
| Teaching | `content/teaching/<name>/index.md` |
| PDFs, CV, files to link | `static/uploads/` |

Your profile photo is `content/authors/admin/avatar.jpg` — replace that file to
change it (keep the name).

## Adding a paper

Copy an existing folder and edit it:

```bash
cp -r content/wp/Humour content/wp/my-new-paper
# then edit content/wp/my-new-paper/index.md
```

Front matter fields that matter:

```yaml
title: "Paper title"
date: "2026-09-01"          # controls ordering
publication: "Under review at Journal of Politics"
authors:
  - admin                   # lowercase 'admin' = you; links to your profile
  - Coauthor Name
doi: ""
url_pdf: "uploads/paper.pdf"   # put the PDF in static/uploads/
abstract: |
  Your abstract here.
featured: false
```

`admin` must be lowercase or it renders as a stranger called "Admin" instead of
linking to you.

### Bulk-importing from BibTeX

Drop a `publications.bib` in the repo root and push. The
`import-publications.yml` workflow converts it into publication pages and opens
a pull request for you to review. Straight export from Zotero works.

---

## Building locally (optional)

Not required — Actions handles it. If you ever want a local preview you'd need
Hugo Extended and Go installed, then `hugo server`.

---

## If something breaks

Roll back to the state before the September 2026 cleanup:

```bash
git reset --hard pre-cleanup-2026-09-10
```

## Notes

- `docs/` used to hold a committed copy of the built site. It's gone; Actions
  builds from source now. Don't re-add it.
- `public/` is the local build output and is gitignored.
