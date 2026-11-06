# sarasti2.github.io

Personal academic website of Alejandro Sarasti Sierra, built with [Hugo](https://gohugo.io) and the [PaperMod](https://github.com/adityatelange/hugo-PaperMod) theme, with a blue palette.

## Where things live

| What | File |
|---|---|
| Name, bio, buttons, icons, menu | `hugo.yaml` |
| Colours | `assets/css/extended/blue.css` |
| Publications (one file each) | `content/papers/*.md` |
| Work in progress (one file each) | `content/wip/*.md` |
| Experience page | `content/experience.md` |
| Teaching page | `content/teaching.md` |
| Photo and CV | `static/photo.jpg`, `static/cv.pdf` |

## Add a paper

Copy any file in `content/papers/` (or `content/wip/`), rename it, and edit the header:

```
---
title: "Paper title"
date: 2027-01-01          # controls the order; only the year is shown
summary: "with Coauthor · Journal, vol(issue)"
---

Body of the paper page: abstract, citation, links.
<a class="pill" href="https://...">PDF</a>
```

## Preview locally

```
hugo server
```

Open http://localhost:1313. The page reloads as you save.

## Publish

```
git add .
git commit -m "Update site"
git push
```

GitHub Actions builds and publishes the site in about a minute (see the Actions tab).
